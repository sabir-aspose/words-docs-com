---
title: Merge Table Cells
second_title: Aspose.Words for Node.js via .NET
articleTitle: Merge Table Cells
linktitle: Merge Table Cells
description: "How to merge table cells in Node.js. Check if cells in a table are merged using Node.js."
type: docs
weight: 40
ai_search_scope: words_nodejs
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nodejs-net/working-with-merged-cells/
timestamp: 2025-07-09-10-05-05
---

Sometimes certain rows in a table require a heading or large blocks of text that take up the full width of the table. For proper design of the table, the user can merge several table cells into one. Aspose.Words supports merged cells when working with all input formats, including importing HTML content.

## How to Merge Table Cells

In Aspose.Words, merged cells are represented by the following properties of the [CellFormat](https://reference.aspose.com/words/nodejs-net/aspose.words.tables/cellformat/) class:

- [horizontalMerge](https://reference.aspose.com/words/nodejs-net/aspose.words.tables/cellformat/horizontalMerge/) which describes if the cell is a part of a horizontal merge of cells
- [verticalMerge](https://reference.aspose.com/words/nodejs-net/aspose.words.tables/cellformat/verticalMerge/) which describes if the cell is a part of a vertical merge of cells

The values of these properties determine the merge behavior of cells:

- The first cell in a sequence of merged cells will have [CellMerge.First](https://reference.aspose.com/words/nodejs-net/aspose.words.tables/cellmerge/)
- Any subsequently merged cells will have [CellMerge.Previous](https://reference.aspose.com/words/nodejs-net/aspose.words.tables/cellmerge/)
- A cell that is not merged will have [CellMerge.None](https://reference.aspose.com/words/nodejs-net/aspose.words.tables/cellmerge/)

{{% alert color="primary" %}}

Sometimes, when loading existing document cells in a table, they will appear merged. However, it can actually be one long cell – sometimes Microsoft Word exports merged cells this way. This can be confusing when attempting to work with individual cells, but there doesn't seem to be any particular pattern as to when this happens.

{{% /alert %}}

## Check if Cell is Merged

To check if a cell is part of a sequence of merged cells, we simply check the **HorizontalMerge** and **VerticalMerge** properties.

The following code example shows how to print the horizontal and vertical cell merge type:

{{< gist "aspose-words-gists" "93de23a2f74a7f2e4971ed203874c983" "check-cells-merged.cs" >}}

{{% alert color="primary" %}}

You can download the sample file of this example from [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Node.js-via-.NET/tree/main/Data/Table%20with%20merged%20cells.docx).

{{% /alert %}}

## Merge Table Cells When Using DocumentBuilder

To merge cells in a table created with the [DocumentBuilder](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/), you need to set the appropriate merge type for each cell where the merge is expected – first **CellMerge.First** and then **CellMerge.Previous**.

Also, you must remember to clear the merge setting for those cells where no merge is required – this can be done by setting the first non-merge cell to **CellMerge.None**. If this is not done, all cells in the table will be merged.

The following code example shows how to create a table with two rows where the cells in the first row are merged horizontally:

{{< gist "aspose-words-gists" "93de23a2f74a7f2e4971ed203874c983" "horizontal-merge.cs" >}}

The following code example shows how to create a two-column table where the cells in the first column are vertically merged:

{{< gist "aspose-words-gists" "93de23a2f74a7f2e4971ed203874c983" "vertical-merge.cs" >}}

## Merge Table Cells in Other Cases

In other situations where the **DocumentBuilder** is not used, such as in an existing table, merging cells in the previous way may not be as easy. Instead, we can wrap the basic operations involved in applying merge properties to cells in a method that makes the task much easier. This method is similar to the Merge automation method, which is called to merge a range of cells in a table.

The code below will merge the table cells in the specified range, starting at the given cell and ending at the end cell. In this case, the range can span multiple rows or columns:

{{< gist "aspose-words-gists" "93de23a2f74a7f2e4971ed203874c983" "merge-cells.cs" >}}

The following code example shows how to merge a range of cells between two specified cells:

{{< gist "aspose-words-gists" "93de23a2f74a7f2e4971ed203874c983" "merge-cell-range.cs" >}}

{{% alert color="primary" %}}

You can download the sample file of this example from [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Node.js-via-.NET/tree/main/Data/Table%20with%20merged%20cells.docx).

{{% /alert %}}

Depending on the version of the Framework you are using, you may want to refine this method by turning it into an extension method. In this case, you can call this method directly on a cell to merge a range of cells, such as `cell1.Merge(cell2)`.

## Convert to Horizontally Merged Cells

Sometimes it is not possible to detect which cells are merged because some newer versions of Microsoft Word no longer use the merge flags when cells are merged horizontally. But for situations where cells are merged into a cell horizontally by their width using merge flags, Aspose.Words provides the `ConvertToHorizontallyMergedCells` method to convert cells. This method simply transforms the table and adds new cells as needed.

The following code example shows the above method in operation:

{{< gist "aspose-words-gists" "93de23a2f74a7f2e4971ed203874c983" "convert-to-horizontally-merged-cells.cs" >}}
