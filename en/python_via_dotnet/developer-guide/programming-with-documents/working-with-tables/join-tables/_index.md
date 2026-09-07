---
title: Join Tables
second_title: Aspose.Words for Python via .NET
articleTitle: Join Tables
linktitle: Join Tables
description: "Join tables in a document using Python. How to merge two tables into one in Python."
type: docs
weight: 90
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/join-tables/
aliases: 
- /python/joining-and-splitting-tables/
- /python-net/joining-and-splitting-tables/
timestamp: 2026-02-03-11-08-55
---

{{% alert color="grey" %}}
*Purpose Summary. What is this page about?*

This page shows how to join two tables in a Word document using Aspose.Words for Python via .NET by moving rows from the second table to the first and then removing the second table's container.
{{% /alert %}}

A table, represented in the Aspose.Words Document Object Model, is made up of independent rows and cells, making it easy to join tables.

To manipulate a table to join with another table, we just need to move the rows from the second table to the end of the first one and remove the second table's container.

The following code example shows how to merge rows from two tables into one:

{{< gist "aspose-words-gists" "58600aa383a4cba01a02603683e30fd3" "combine-rows.py" >}}

## Related APIs

- `aspose.words.tables.Table` — Represents a table in the document.
- `aspose.words.tables.Row` — Represents a table row.
- `document.import_node(node, True)` — Imports a node from another document, preserving formatting when the second argument is `True`.
- `row_collection.add(node)` — Adds a row to the table's row collection.
- `node.remove()` — Removes the node from the document.