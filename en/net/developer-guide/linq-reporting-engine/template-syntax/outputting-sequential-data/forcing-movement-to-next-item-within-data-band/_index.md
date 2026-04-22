---
title: Forcing Movement to Next Item within Data Band in C#
second_title: Aspose.Words for .NET
articleTitle: Forcing Movement to Next Item within Data Band
linktitle: Forcing Movement to Next Item within Data Band
description: "Force movement to the next item within a data band when building a report in C#."
type: docs
weight: 70
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/forcing-movement-to-next-item-within-data-band/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

## Purpose Summary

This page describes how to force movement to the next item within a data band in reporting templates.

{{% /alert %}}

You can instruct the engine to force movement to the next item within a data band using a `next` tag. This feature is useful in label-print-like scenarios when you need to output data about a fixed number of items in a single table row like in the following example. Given that `Clients` is a `DataTable` instance having a field named "Name", you can use the following template to output three client names per table row while outputting names of all clients in a single table.

<table class="outputting-sequential-data">
	<tbody>
		<tr>
			<td>&lt;&lt;foreach [c in Clients]>>&lt;&lt;[c.Name]>></td>
			<td>&lt;&lt;next>>&lt;&lt;[c.Name]>></td>
			<td>&lt;&lt;next>>&lt;&lt;[c.Name]>> &lt;&lt;/foreach>></td>
		</tr>
	</tbody>
</table>

In this case, the engine produces a report as follows.

| A Company   | B Ltd.           | C & D       |
| :---------- | :--------------- | :---------- |
| **E Corp.** | **F & Partners** | **G & Co.** |
| **H Group** | **I & Sons**     | **J Ent.**  |

## Related APIs

------

## FAQ

1. **Q:** What does the `next` tag do inside a data band?  
   **A:** The `next` tag tells the reporting engine to move the cursor to the next column (or cell) of the current data band row before inserting the following field value. It enables you to place multiple items from the same data source into separate columns of a single row.

2. **Q:** How many `next` tags can I place in one row?  
   **A:** You can use as many `next` tags as there are columns in the row. Each `next` advances the cursor by one column, so the number of `next` tags should not exceed the number of columns you have defined in the table row.

3. **Q:** Can the `next` tag be combined with other template tags such as `if` or `foreach`?  
   **A:** Yes. The `next` tag works together with other tags. For example, you can wrap a series of `next`‑separated fields inside a `foreach` loop, or place an `if` condition before a `next` to output a value only when a condition is met.

4. **Q:** Why does the `next` tag sometimes appear to be ignored and all data ends up in the first column?  
   **A:** This usually happens when the table row does not contain enough cells to accommodate the `next` movements, or when the template syntax is malformed (e.g., missing closing `>>`). Ensure the HTML table row has a `<td>` element for each `next` you use and that all tags are correctly closed. Also verify that the data source actually contains enough items for the loop.