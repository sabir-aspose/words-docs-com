---
title: Applying Conditional Formatting to Table Rows in C#
second_title: Aspose.Words for .NET
articleTitle: Applying Conditional Formatting to Table Rows
linktitle: Applying Conditional Formatting to Table Rows
description: "How to apply conditional formatting to table rows using LINQ Reporting Engine in C#."
type: docs
weight: 40
url: /net/applying-conditional-formatting-to-table-rows/
---

Applying conditional formatting to table rows visually distinguishes data based on specific criteria, making it easier for
users to identify trends, outliers, or important patterns at a glance. This visual emphasis enhances data interpretation and
analysis, allowing users to quickly assess the significance of information without sifting through all the data manually.
You can build a table with conditional formatting applied to rows using LINQ Reporting Engine in C#.

## How to Apply Conditional Formatting to Table Rows

{{% alert %}}

This guide deals with a table with rows bound to a collection. However, you can apply a similar approach to tables of static
structure as well.

{{% /alert %}}

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-conditional-formatting-applied-to-rows-data.json >}}
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
rows for repeating. For this example, the number of rows for capturing should be twice larger than needed for a single item of
the collection as explained further.

{{% /alert %}}

6. Imaginably, split the range of table rows between the opening and closing `foreach` tags into two equal parts.

7. Bind visibility of the first part of rows to a Boolean value calculated upon an item of the collection by adding an opening
`if` tag to the beginning of the first row of this part after the opening `foreach` tag, for instance, like this:
{{< highlight "c#" >}}
<<if [visitors >= 2000]>>
{{< /highlight >}}

8. Bind visibility of the second part of rows to the opposite value by adding an `else` tag to the beginning of the first row
of the second part this way:
{{< highlight "c#" >}}
<<else>>
{{< /highlight >}}

9. Add a closing `if` tag to the end of the last row of the second part of rows before the closing `foreach` tag as follows:
{{< highlight "c#" >}}
<</if>>
{{< /highlight >}}

{{% alert %}}

Opening `if` and `else` tags as well as `else` and closing `if` tags can be used to capture one or more rows of a single table
for showing in case when a particular condition is met or not met respectively.

{{% /alert %}}

10. Apply different formatting to every of the parts of rows depending on your needs.

11. Within the range between the opening `if` and `else` tags, bind cells of the table to values calculated upon an item of
the data collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[date]:"dd\/MM\/yyyy">>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[visitors]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[pageViews]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[bounceRate]>>
{{< /highlight >}}

12. Use the same expression tags to bind cells of the table within the range between the `else` and closing `if` tags to values
calculated upon an item of the collection.

13. Review your table template before saving, it should look like this:\
\
<img src="table-with-conditional-formatting-applied-to-rows-template.png"
  alt="Table with conditional formatting applied to rows template for LINQ Reporting Engine in C#."
  style="width:625px"/>

14. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "749070be98dfa2c3159257b4f3ea3401" "applying-conditional-formatting-to-table-rows.cs" >}}

## Table with Conditional Formatting Applied to Rows Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-conditional-formatting-applied-to-rows-report.png"
  alt="Table with conditional formatting applied to rows report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Conditional%20Formatting%20Applied%20to%20Rows%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Conditional%20Formatting%20Applied%20to%20Rows%20Data.json)
from the example, and try to make a table with conditional formatting applied to rows online for free by using one of
the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Apply Background Colors to Table Rows

{{% alert %}}

This guide provides a shortcut method for applying only background colors to table rows.

{{% /alert %}}

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-background-colors-applied-to-rows-data.json >}}
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

6. Bind the background color of a row of the table to be repeated for every item of the collection to a [color value
]({{< ref "#supported-color-values" >}}) calculated upon an item of the collection by adding an opening `backColor` tag to
the beginning of the row after the opening `foreach` tag, for instance, like this:
{{< highlight "c#" >}}
<<backColor [(contractValue >= 100000) ? "beige" : "white"]>>
{{< /highlight >}}

{{% alert %}}

A color value can be directly stored in a data source, for example, as a property of an item of a collection bound to the table.

{{% /alert %}}

7. Add a closing `backColor` tag to the end of a row of the table to be repeated for every item of the collection before
the closing `foreach` tag as follows:
{{< highlight "c#" >}}
<</backColor>>
{{< /highlight >}}

{{% alert %}}

Opening and closing `backColor` tags can be located in a single row or different rows of a single table to capture one or more
rows for applying a background color.

{{% /alert %}}

8. Within the range between the opening and closing `backColor` tags, bind cells of the table to values calculated upon an item
of the data collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[clientName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[contractValue]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[startDate]:"dd\/MM\/yyyy">>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[endDate]:"dd\/MM\/yyyy">>
{{< /highlight >}}

9. Review your table template before saving, it should look like this:\
\
<img src="table-with-background-colors-applied-to-rows-template.png"
  alt="Table with background colors applied to rows template for LINQ Reporting Engine in C#."
  style="width:625px"/>

10. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "b1c9ffb0ed27ad32a33f4078b0b75231" "applying-background-colors-to-table-rows.cs" >}}

## Table with Background Colors Applied to Rows Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-background-colors-applied-to-rows-report.png"
  alt="Table with background colors applied to rows report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Background%20Colors%20Applied%20to%20Rows%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Background%20Colors%20Applied%20to%20Rows%20Data.json)
from the example, and try to make a table with background colors applied to rows online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Apply Text Colors to Table Rows

{{% alert %}}

This guide walks through a shortcut approach for applying only text colors to table rows.

{{% /alert %}}

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-text-colors-applied-to-rows-data.json >}}
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

6. Bind the text color of a row of the table to be repeated for every item of the collection to a [color value
]({{< ref "#supported-color-values" >}}) calculated upon an item of the collection by adding an opening `textColor` tag to
the beginning of the row after the opening `foreach` tag, for instance, like this:
{{< highlight "c#" >}}
<<textColor [adjustmentType == "Damage" ? "Red" : "Black"]>>
{{< /highlight >}}

{{% alert %}}

A color value can be directly stored in a data source, for example, as a property of an item of a collection bound to the table.

{{% /alert %}}

7. Add a closing `textColor` tag to the end of a row of the table to be repeated for every item of the collection before
the closing `foreach` tag as follows:
{{< highlight "c#" >}}
<</textColor>>
{{< /highlight >}}

{{% alert %}}

Opening and closing `textColor` tags can be located in a single row or different rows of a single table to capture one or more
rows for applying a text color.

{{% /alert %}}

8. Within the range between the opening and closing `textColor` tags, bind cells of the table to values calculated upon an item
of the data collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[productName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[adjustmentDate]:"dd\/MM\/yyyy">>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[adjustmentType]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[quantityAdjusted]>>
{{< /highlight >}}

9. Review your table template before saving, it should look like this:\
\
<img src="table-with-text-colors-applied-to-rows-template.png"
  alt="Table with text colors applied to rows template for LINQ Reporting Engine in C#."
  style="width:625px"/>

10. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "2b490da2afa4b725e1b0ceefaec92b32" "applying-text-colors-to-table-rows.cs" >}}

## Table with Text Colors Applied to Rows Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-text-colors-applied-to-rows-report.png"
  alt="Table with text colors applied to rows report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Text%20Colors%20Applied%20to%20Rows%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Text%20Colors%20Applied%20to%20Rows%20Data.json)
from the example, and try to make a table with text colors applied to rows online for free by using one of the options:\
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