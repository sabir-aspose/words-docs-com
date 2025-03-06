---
title: Applying Conditional Formatting to Table Columns in C#
second_title: Aspose.Words for .NET
articleTitle: Applying Conditional Formatting to Table Columns
linktitle: Applying Conditional Formatting to Table Columns
description: "How to apply conditional formatting to table columns using LINQ Reporting Engine in C#."
type: docs
weight: 110
url: /net/applying-conditional-formatting-to-table-columns/
---

Applying conditional formatting to table columns enhances data visualization by allowing users to quickly identify patterns,
trends, or discrepancies based on specific criteria. By using visual cues such as color coding or highlighting, this technique
makes it easier for users to interpret large datasets and draw insights without having to manually sift through every entry.
You can build a table with conditional formatting applied to columns using LINQ Reporting Engine in C#.

## How to Apply Conditional Formatting to Table Columns

{{% alert %}}

This guide deals with a table with columns bound to a collection. However, you can apply a similar approach to tables of static
structure as well.

{{% /alert %}}

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-conditional-formatting-applied-to-columns-data.json >}}
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
a single table to capture one or more columns for repeating. For this example, the number of columns for capturing should be
twice larger than needed for a single item of the collection as explained further.

{{% /alert %}}

7. Imaginably, split the range of table columns between the opening and closing `foreach` tags into two equal parts.

8. Bind visibility of the first part of columns to a Boolean value calculated upon an item of the collection by adding an opening
`if` tag with a `horz` switch to the beginning of the first column of this part after the opening `foreach` tag, for instance,
like this:
{{< highlight "c#" >}}
<<if [participants >= 20] -horz>>
{{< /highlight >}}

9. Bind visibility of the second part of columns to the opposite value by adding an `else` tag to the beginning of the first column
of the second part this way:
{{< highlight "c#" >}}
<<else>>
{{< /highlight >}}

10. Add a closing `if` tag to the end of the last column of the second part of columns before the closing `foreach` tag as follows:
{{< highlight "c#" >}}
<</if>>
{{< /highlight >}}

{{% alert %}}

With a `horz` switch applied, opening `if` and `else` tags as well as `else` and closing `if` tags can be used to capture one
or more columns of a single table for showing in case when a particular condition is met or not met respectively.

{{% /alert %}}

11. Apply different formatting to every of the parts of columns depending on your needs.

12. Within the range between the opening `if` and `else` tags, bind cells of the table to values calculated upon an item of
the data collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[topic]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[date]:"dd\/MM\/yyyy">>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[durationHours]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[participants]>>
{{< /highlight >}}

13. Use the same expression tags to bind cells of the table within the range between the `else` and closing `if` tags to values
calculated upon an item of the collection.

14. Review your table template before saving, it should look like this:\
\
<img src="table-with-conditional-formatting-applied-to-columns-template.png"
  alt="Table with conditional formatting applied to columns template for LINQ Reporting Engine in C#."
  style="width:625px"/>

15. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "896a6e0853a7e706952eec3203954f4b" "applying-conditional-formatting-to-table-columns.cs" >}}

## Table with Conditional Formatting Applied to Columns Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-conditional-formatting-applied-to-columns-report.png"
  alt="Table with conditional formatting applied to columns report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Conditional%20Formatting%20Applied%20to%20Columns%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Conditional%20Formatting%20Applied%20to%20Columns%20Data.json)
from the example, and try to make a table with conditional formatting applied to columns online for free by using one of
the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Apply Background Colors to Table Columns

{{% alert %}}

This guide provides a shortcut method for applying only background colors to table columns.

{{% /alert %}}

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-background-colors-applied-to-columns-data.json >}}
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
of the data collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[projectName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[startDate]:"dd\/MM\/yyyy">>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[endDate]:"dd\/MM\/yyyy">>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[budget]>>
{{< /highlight >}}

8. For every cell of a column of the table to be repeated for every item of the collection, bind the cell's background color to
the same [color value]({{< ref "#supported-color-values" >}}) calculated upon an item of the collection by taking the following
steps:

    * Add an opening `backColor` tag to the beginning of the cell after the opening `foreach` tag, for instance, like this:
{{< highlight "c#" >}}
<<backColor [(budget >= 30000) ? "linen" : "white"]>>
{{< /highlight >}}
{{% alert %}}

A color value can be directly stored in a data source, for example, as a property of an item of a collection bound to the table.

{{% /alert %}}

    * Add a closing `backColor` tag to the end of the cell before the closing `foreach` tag as follows:
{{< highlight "c#" >}}
<</backColor>>
{{< /highlight >}}

9. Review your table template before saving, it should look like this:\
\
<img src="table-with-background-colors-applied-to-columns-template.png"
  alt="Table with background colors applied to columns template for LINQ Reporting Engine in C#."
  style="width:625px"/>

10. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "aae874038596ea2e96371bb37b30b692" "applying-background-colors-to-table-columns.cs" >}}

## Table with Background Colors Applied to Columns Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-background-colors-applied-to-columns-report.png"
  alt="Table with background colors applied to columns report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Background%20Colors%20Applied%20to%20Columns%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Background%20Colors%20Applied%20to%20Columns%20Data.json)
from the example, and try to make a table with background colors applied to columns online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Apply Text Colors to Table Columns

{{% alert %}}

This guide walks through a shortcut approach for applying only text colors to table columns.

{{% /alert %}}

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-text-colors-applied-to-columns-data.json >}}
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
of the data collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[platform]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[postDate]:"dd\/MM\/yyyy">>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[engagements]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[reach]>>
{{< /highlight >}}

8. For every cell of a column of the table to be repeated for every item of the collection, bind the cell's text color to
the same [color value]({{< ref "#supported-color-values" >}}) calculated upon an item of the collection by taking the following
steps:

    * Add an opening `textColor` tag to the beginning of the cell after the opening `foreach` tag, for instance, like this:
{{< highlight "c#" >}}
<<textColor [(reach >= 2000) ? "blue" : "black"]>>
{{< /highlight >}}
{{% alert %}}

A color value can be directly stored in a data source, for example, as a property of an item of a collection bound to the table.

{{% /alert %}}

    * Add a closing `textColor` tag to the end of the cell before the closing `foreach` tag as follows:
{{< highlight "c#" >}}
<</textColor>>
{{< /highlight >}}

9. Review your table template before saving, it should look like this:\
\
<img src="table-with-text-colors-applied-to-columns-template.png"
  alt="Table with text colors applied to columns template for LINQ Reporting Engine in C#."
  style="width:625px"/>

10. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "ad728469bf0d8b577d99b4d57004b59e" "applying-text-colors-to-table-columns.cs" >}}

## Table with Text Colors Applied to Columns Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-text-colors-applied-to-columns-report.png"
  alt="Table with text colors applied to columns report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Text%20Colors%20Applied%20to%20Columns%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Text%20Colors%20Applied%20to%20Columns%20Data.json)
from the example, and try to make a table with text colors applied to columns online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

{{% include "../../common/color-values.md" %}}

## See Also

- [Building Tables]({{< ref "../../building-tables/" >}})
- [Binding Collections]({{< ref "../../binding-data/binding-collections/" >}})
- [Formatting Data]({{< ref "../../formatting-data/" >}})
- [LINQ Reporting Engine]({{< ref "../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../common/footer.md" %}}