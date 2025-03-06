---
title: Merging Table Cells in C#
second_title: Aspose.Words for .NET
articleTitle: Merging Table Cells
linktitle: Merging Table Cells
description: "How to merge table cells using LINQ Reporting Engine in C#."
type: docs
weight: 120
url: /net/merging-table-cells/
---

Merging table cells allows for the consolidation of related information into a single cell, which can help clarify
the relationships between data points and reduce visual clutter. This technique is particularly beneficial for creating
headers or grouping related data, making the table more organized and easier for users to read and understand. You can
build a table with merged cells using LINQ Reporting Engine in C#.

## How to Merge Table Cells Vertically

{{% alert %}}

This guide deals with a table with rows bound to a collection. However, you can apply a similar approach to tables of any type
including ones with static structure.

{{% /alert %}}

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-cells-merged-vertically-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a
table](https://support.microsoft.com/en-us/office/insert-a-table-a138f745-73ef-4879-b99a-2f3d38be612a#platform=Windows)
with a necessary number of columns and [format its
elements](https://support.microsoft.com/en-us/office/format-a-table-e6e77bc6-1f4e-467e-b818-2e2acc488006)
to use it as a template.

3. Add static content like headers to the table, if needed.

4. Bind the table to a data collection by adding an opening `foreach` tag to the beginning of a row to be repeated for every
item of the collection as per the example:
{{< highlight "c#" >}}
<<foreach [in items]>>
{{< /highlight >}}

5. Add a closing `foreach` tag to the end of a row to be repeated for every item of the collection like so:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

{{% alert %}}

Opening and closing `foreach` tags can be located in a single row or different rows of a single table to capture one or more
rows for repeating.

{{% /alert %}}

6. Within the range between the opening and closing `foreach` tags, bind cells of the table to values calculated upon an item
of the collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[location]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[productName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[quantity]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[lastUpdated]:"dd\/MM\/yyyy">>
{{< /highlight >}}

7. For cells to be merged vertically in a result table, append `cellMerge` tags this way:
{{< highlight "c#" >}}
<<cellMerge>>
{{< /highlight >}}

{{% alert %}}

In order to vertically merge two or more neighbor cells, all the cells should contain a `cellMerge` tag without any switches,
have equal textual contents in a result table (ignoring surrounding whitespaces), and be not already merged horizontally.

{{% /alert %}}

8. Review your table template before saving, it should look like this:\
\
<img src="table-with-cells-merged-vertically-template.png"
  alt="Table with cells merged vertically template for LINQ Reporting Engine in C#."
  style="width:625px"/>

9. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "0d477de87c617d7dbbe4b710a0271568" "merging-table-cells-vertically.cs" >}}

## Table with Cells Merged Vertically Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-cells-merged-vertically-report.png"
  alt="Table with cells merged vertically report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Cells%20Merged%20Vertically%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Cells%20Merged%20Vertically%20Data.json)
from the example, and try to make a table with cells merged vertically online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Merge Table Cells Horizontally

{{% alert %}}

Although this guide shows working with a table with columns bound to a collection, you can apply a similar technique to tables
of any type including tables of static structure.

{{% /alert %}}

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-cells-merged-horizontally-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a
table](https://support.microsoft.com/en-us/office/insert-a-table-a138f745-73ef-4879-b99a-2f3d38be612a#platform=Windows)
with a necessary number of rows and [format its
elements](https://support.microsoft.com/en-us/office/format-a-table-e6e77bc6-1f4e-467e-b818-2e2acc488006)
to use it as a template.

3. Consider applying [automatical resizing to columns of
the table](https://support.microsoft.com/en-us/office/resize-a-table-row-or-column-9340d478-21be-4392-81cf-488f7bbd6715#__toc293661261).

4. Add static content like headers to the table, if needed.

5. Bind the table to a data collection by adding an opening `foreach` tag with a `horz` switch to the beginning of a column
to be repeated for every item of the collection as per the example:
{{< highlight "c#" >}}
<<foreach [in items] -horz>>
{{< /highlight >}}

6. Add a closing `foreach` tag to the end of a column to be repeated for every item of the collection like so:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

{{% alert %}}

With a `horz` switch applied, opening and closing `foreach` tags can be located in a single column or different columns of
a single table to capture one or more columns for repeating.

{{% /alert %}}

7. Within the range between the opening and closing `foreach` tags, bind cells of the table to values calculated upon an item
of the collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[category]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[project]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[revenue]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[expenses]>>
{{< /highlight >}}

8. For cells to be merged horizontally in a result table, append `cellMerge` tags with `horz` switches this way:
{{< highlight "c#" >}}
<<cellMerge -horz>>
{{< /highlight >}}

{{% alert %}}

In order to horizontally merge two or more neighbor cells, all the cells should contain a `cellMerge` tag with a `horz` switch,
have equal textual contents in a result table (ignoring surrounding whitespaces), and be not already merged vertically.

{{% /alert %}}

9. Review your table template before saving, it should look like this:\
\
<img src="table-with-cells-merged-horizontally-template.png"
  alt="Table with cells merged horizontally template for LINQ Reporting Engine in C#."
  style="width:625px"/>

10. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "be43c7e51ac9138792a43c08d599e154" "merging-table-cells-horizontally.cs" >}}

## Table with Cells Merged Horizontally Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-cells-merged-horizontally-report.png"
  alt="Table with cells merged horizontally report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Cells%20Merged%20Horizontally%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Cells%20Merged%20Horizontally%20Data.json)
from the example, and try to make a table with cells merged horizontally online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Merge Table Cells Vertically and Horizontally

{{% alert %}}

This guide uses a table with rows bound to a collection as an example, but you can apply the same approach to tables of any type
including static-structure ones.

{{% /alert %}}

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-cells-merged-vertically-and-horizontally-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a
table](https://support.microsoft.com/en-us/office/insert-a-table-a138f745-73ef-4879-b99a-2f3d38be612a#platform=Windows)
with a necessary number of columns and [format its
elements](https://support.microsoft.com/en-us/office/format-a-table-e6e77bc6-1f4e-467e-b818-2e2acc488006)
to use it as a template.

3. Add static content like headers to the table, if needed.

4. Bind the table to a data collection by adding an opening `foreach` tag to the beginning of a row to be repeated for every
item of the collection as per the example:
{{< highlight "c#" >}}
<<foreach [in items]>>
{{< /highlight >}}

5. Add a closing `foreach` tag to the end of a row to be repeated for every item of the collection like so:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

{{% alert %}}

Opening and closing `foreach` tags can be located in a single row or different rows of a single table to capture one or more
rows for repeating.

{{% /alert %}}

6. Within the range between the opening and closing `foreach` tags, bind cells of the table to values calculated upon an item
of the collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[category]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[subcategory]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[project]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[potentialValue]>>
{{< /highlight >}}

7. For cells to be merged vertically and horizontally in a result table, append `cellMerge` tags with `both` switches this way:
{{< highlight "c#" >}}
<<cellMerge -both>>
{{< /highlight >}}

{{% alert %}}

In order to merge two or more neighbor cells both vertically and horizontally, all the cells should contain a `cellMerge` tag
with a `both` switch and have equal textual contents in a result table (ignoring surrounding whitespaces).

{{% /alert %}}

8. Review your table template before saving, it should look like this:\
\
<img src="table-with-cells-merged-vertically-and-horizontally-template.png"
  alt="Table with cells merged vertically and horizontally template for LINQ Reporting Engine in C#."
  style="width:625px"/>

9. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "fd21a16d172df2129f52303978551c5c" "merging-table-cells-vertically-and-horizontally.cs" >}}

## Table with Cells Merged Vertically and Horizontally Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-cells-merged-vertically-and-horizontally-report.png"
  alt="Table with cells merged vertically and horizontally report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Cells%20Merged%20Vertically%20and%20Horizontally%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Cells%20Merged%20Vertically%20and%20Horizontally%20Data.json)
from the example, and try to make a table with cells merged vertically and horizontally online for free by using one of
the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Restrict Table Cell Merging

{{% alert %}}

Although this guide focuses on vertical cell merging for a table with rows bound to master-detail data, you can apply a similar
method to any direction of cell merging, tables of any type (including those with static structure), and data structured any
other way.

{{% /alert %}}

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-cell-merging-restriction-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a
table](https://support.microsoft.com/en-us/office/insert-a-table-a138f745-73ef-4879-b99a-2f3d38be612a#platform=Windows)
with a necessary number of columns and [format its
elements](https://support.microsoft.com/en-us/office/format-a-table-e6e77bc6-1f4e-467e-b818-2e2acc488006)
to use it as a template.

3. Add static content like headers to the table, if needed.

4. Bind the table to a master data collection by adding an opening `foreach` tag to the beginning of a row to be repeated for
every item of the collection as per the example:
{{< highlight "c#" >}}
<<foreach [i in items]>>
{{< /highlight >}}

5. Add a closing `foreach` tag to the end of a row to be repeated for every item of the collection like so:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

{{% alert %}}

Opening and closing `foreach` tags can be located in a single row or different rows of a single table to capture one or more
rows for repeating.

{{% /alert %}}

6. Bind the table row containing the opening `foreach` tag to a detail data collection calculated upon an item of the master
data collection to repeat the row for every item of the detail collection by adding an inner opening `foreach` tag to
the beginning of the row after the outer opening `foreach` tag, for instance, as follows:
{{< highlight "c#" >}}
<<foreach [in details]>>
{{< /highlight >}}

7. Add an inner closing `foreach` tag to the end of the row containing the outer closing `foreach` tag before the tag this way:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

{{% alert %}}

In this example, outer and inner `foreach` tags capture the same row for repeating.

{{% /alert %}}

8. Within the range between the inner opening and closing `foreach` tags, bind cells of the row to values calculated upon
an item of the detail collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[i.number]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[product]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[pack]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[price]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[count]>>
{{< /highlight >}}

{{% alert %}}

Since between the inner opening and closing `foreach` tags, expression values are calculated upon an item of the detail
collection, an explicit reference to an item of the master collection - such as `i` - is required when accessing master data.

{{% /alert %}}

9. For cells to be merged vertically in a result table, append `cellMerge` tags like so:
{{< highlight "c#" >}}
<<cellMerge>>
{{< /highlight >}}

{{% alert %}}

In order to vertically merge two or more neighbor cells, all the cells should contain a `cellMerge` tag without any switches,
have equal textual contents in a result table (ignoring surrounding whitespaces), and be not already merged horizontally.

{{% /alert %}}

10. To additionally restrict merging of cells to those for which a particular expression evaluates to the same value, append
the expression to corresponding `cellMerge` tags, for instance, as per the snippet:
{{< highlight "c#" >}}
<<cellMerge [i.number]>>
{{< /highlight >}}

{{% alert %}}

When an expression defined at a `cellMerge` tag evalutes to the same value for neighbor cells, the cells are merged if all
other conditions for merging - such as equal cell textual contents - are met.

{{% /alert %}}

11. Review your table template before saving, it should look like this:\
\
<img src="table-with-cell-merging-restriction-template.png"
  alt="Table with a cell merging restriction template for LINQ Reporting Engine in C#."
  style="width:625px"/>

12. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "ddf6b9088880b166c2619841b41bbc76" "restricting-table-cell-merging.cs" >}}

## Table with a Cell Merging Restriction Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-cell-merging-restriction-report.png"
  alt="Table with a cell merging restriction report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Cell%20Merging%20Restriction%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Cell%20Merging%20Restriction%20Data.json)
from the example, and try to make a table with a cell merging restriction online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## See Also

- [Building Tables]({{< ref "../../building-tables/" >}})
- [Binding Collections]({{< ref "../../binding-data/binding-collections/" >}})
- [Formatting Data]({{< ref "../../formatting-data/" >}})
- [LINQ Reporting Engine]({{< ref "../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../common/footer.md" %}}