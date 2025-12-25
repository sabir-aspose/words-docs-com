---
title: Work with Text in a Table
second_title: Aspose.Words for .NET
articleTitle: Work with Text in a Table
linktitle: Work with Text in a Table
description: "Replace text in a table in C#. Extract Plain Text from Table or Cell using C#."
type: docs
weight: 60
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/work-with-text-in-a-table/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*What is this page about?*

This page explains how to work with text inside a table, including formatting and extraction.

{{% /alert %}}

As mentioned in previous articles, a table usually contains plain text, although other content such as images or even other tables can be placed in table cells.

Adding text or other content to the table is carried out using the appropriate methods of the [DocumentBuilder](https://reference.aspose.com/words/net/aspose.words/documentbuilder/) class and is described in the **"Create a Table"** article. In this article, we will talk about how to work with text in an already existing table.

## Replace Text in a Table

The table, like any other node in Aspose.Words, has access to the [Range](https://reference.aspose.com/words/net/aspose.words/range/) object. Using the table range object, you can replace text in a table.

The ability to use special characters when replacing is currently supported, so it is possible to replace existing text with multi-paragraph text. To do this, you need to use the special metacharacters described in the corresponding [Replace](https://reference.aspose.com/words/net/aspose.words/range/replace/) method.

{{% alert color="primary" %}}

Typically, text replacement should be done at the cell level (per cell) or at the paragraph level.

{{% /alert %}}

The following code example shows how to replace all instances of a string of text in the cells of an entire table:

{{< gist "aspose-words-gists" "458eb4fd5bd1de8b06fab4d1ef1acdc6" "replace-text.cs" >}}

## Extract Plain Text from Table or Cell

Using the **Range** object, you can also call methods on the entire table range and extract the table as plain text. To do this, use the [Text](https://reference.aspose.com/words/net/aspose.words/range/text/) property. 

The following code example shows how to print the text range of a table:

{{< gist "aspose-words-gists" "458eb4fd5bd1de8b06fab4d1ef1acdc6" "extract-text.cs" >}}

The same technique is used to extract content from individual table cells only.

The following code example shows how to print a text range of row and table elements:

{{< gist "aspose-words-gists" "458eb4fd5bd1de8b06fab4d1ef1acdc6" "print-text-range-row-and-table.cs" >}}

## Working with Alternative Table Text

Microsoft Word tables have a `table title` and `table description` that provide an alternative textual representation of the information contained in the table.

In Aspose.Words, you can also add a table title and description using the [Title](https://reference.aspose.com/words/net/aspose.words.tables/table/title/) and [Description](https://reference.aspose.com/words/net/aspose.words.tables/table/description/) properties. These properties are meaningful for DOCX documents conforming to the ISO/IEC 29500. When saving in formats earlier than ISO/IEC 29500, these properties are ignored.

The following code example shows how to set the title and description properties of a table:

{{< gist "aspose-words-gists" "458eb4fd5bd1de8b06fab4d1ef1acdc6" "table-title-and-description.cs" >}}

---

## FAQ

1. **Q:** How can I replace a specific string in all cells of a table?  
   **A:** Retrieve the table’s `Range` object and call `Range.Replace("oldText", "newText")`. This operation scans every cell, paragraph, and run within the table and substitutes the matching text.

2. **Q:** How do I extract plain text from an entire table versus a single cell?  
   **A:** For the whole table, use `Table.Range.Text`. For a particular cell, access `Cell.Range.Text`. Both properties return the textual content without any formatting or markup.

3. **Q:** Can I replace text with line breaks or multiple paragraphs inside a cell?  
   **A:** Yes. Include the special metacharacters `\r` (paragraph break) and `\v` (line break) in the replacement string when calling `Range.Replace`. Aspose.Words will insert the appropriate breaks during the replacement.

4. **Q:** How can I add a title or description to a table for accessibility purposes?  
   **A:** Set the `Table.Title` and `Table.Description` properties. These are stored in the DOCX file according to the ISO/IEC 29500 standard and are ignored when saving to older Word formats.

5. **Q:** I need to replace text but keep the original formatting; how can I achieve that?  
   **A:** Use `Range.Replace` together with a `FindReplaceOptions` object where `PreserveFormatting` is set to `true`. This ensures that only the text changes while the original font, style, and other formatting remain intact.