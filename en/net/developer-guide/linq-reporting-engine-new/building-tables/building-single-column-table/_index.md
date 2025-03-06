---
title: Building Single-Column Table in C#
second_title: Aspose.Words for .NET
articleTitle: Building Single-Column Table
linktitle: Building Single-Column Table
description: "How to make a single-column table using LINQ Reporting Engine in C#."
type: docs
weight: 80
url: /net/building-single-column-table/
---

A single-column table provides a straightforward way to present information that requires minimal comparison, such as lists of
items, names, or categories. This simplicity enhances readability and focus, allowing users to quickly scan through the content
without the distraction of multiple columns or complex layouts. You can make a single-column table using LINQ Reporting Engine
in C#.

## How to Build a Single-Column Table

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include single-column-table-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a
table](https://support.microsoft.com/en-us/office/insert-a-table-a138f745-73ef-4879-b99a-2f3d38be612a#platform=Windows)
with one column and [format
elements of the table](https://support.microsoft.com/en-us/office/format-a-table-e6e77bc6-1f4e-467e-b818-2e2acc488006)
to use it as a template.

3. Add static content like a column header to the table, if needed.

4. Bind the table to a data collection by adding an opening `foreach` tag to the beginning of a row to be repeated for every
item of the collection as per the example:
{{< highlight "c#" >}}
<<foreach [in items]>>
{{< /highlight >}}

5. Add a closing `foreach` tag with a `greedy` switch to the end of a row to be repeated for every item of the collection
like so:
{{< highlight "c#" >}}
<</foreach -greedy>>
{{< /highlight >}}

{{% alert %}}

Opening and closing `foreach` tags can be located in a single row or different rows of a single table to capture one or more
rows for repeating.

{{% /alert %}}

6. Within the range between the opening and closing `foreach` tags, bind cells of the table (it can be just a single cell) to
values calculated upon an item of the collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[rating]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[customerName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[feedbackDate]:"dd\/MM\/yyyy">>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[comments]>>
{{< /highlight >}}

7. Review your table template before saving, it should look like this:\
\
<img src="single-column-table-template.png"
  alt="Single-column table template for LINQ Reporting Engine in C#."
  style="width:625px"/>

8. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "da447f6a823cc5e5c0599122edba80cc" "building-single-column-table.cs" >}}

## Single-Column Table Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="single-column-table-report.png"
  alt="Single-column table report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Single-Column%20Table%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Single-Column%20Table%20Data.json)
from the example, and try to make a single-column table online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Show a Single-Column Table Row Based on a Condition

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include single-column-table-with-row-shown-based-on-condition-data-1.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a
table](https://support.microsoft.com/en-us/office/insert-a-table-a138f745-73ef-4879-b99a-2f3d38be612a#platform=Windows)
with a maximum necessary number of rows and one column, and [format
elements of the table](https://support.microsoft.com/en-us/office/format-a-table-e6e77bc6-1f4e-467e-b818-2e2acc488006)
to use it as a template.

3. Add static content like a column header to the table, if needed.

4. Bind cells of the table to values by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[productName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[category]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[price]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[stockQuantity]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[supplierName]>>
{{< /highlight >}}

5. Bind visibility of a row of the table to be shown based on a condition to a Boolean value by adding an opening `if` tag to
the beginning of the row as per the example:
{{< highlight "c#" >}}
<<if [showQuantity]>>
{{< /highlight >}}

6. Add a closing `if` tag with a `greedy` switch to the end of a row of the table to be shown based on a condition like so:
{{< highlight "c#" >}}
<</if -greedy>>
{{< /highlight >}}

{{% alert %}}

Opening and closing `if` tags can be located in a single row or different rows of a single table to capture one or more rows
for showing based on the same condition.

{{% /alert %}}

7. Review your table template before saving, it should look like this:\
\
<img src="single-column-table-with-row-shown-based-on-condition-template.png"
  alt="Single-column table with a row shown based on a condition template for LINQ Reporting Engine in C#."
  style="width:625px"/>

8. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "b841d4c42cfcad6ede6feaaf84f485ad" "showing-single-column-table-row-based-on-condition.cs" >}}

## Single-Column Table with a Row Shown Based on a Condition Report Example

After taking all the steps, LINQ Reporting Engine creates a table report with all the rows shown as follows:\
\
<img src="single-column-table-with-row-shown-based-on-condition-report-1.png"
  alt="Single-column table with a row shown based on a condition report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

Now, let us consider the alternative case where data for the table implies exclusion of one of the rows, for example, like so:
{{< highlight json >}}
{{< include single-column-table-with-row-shown-based-on-condition-data-2.json >}}
{{< /highlight >}}

After running the same code with the JSON file being used instead, LINQ Reporting Engine generates a table report with
one of the rows excluded like this:\
\
<img src="single-column-table-with-row-shown-based-on-condition-report-2.png"
  alt="Single-column table with a row shown based on a condition report generated by LINQ Reporting Engine in C#."
  style="width:625px"/>

Thus, you can control which single-column table rows to show or hide based on conditions.

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Single-Column%20Table%20with%20Row%20Shown%20Based%20on%20Condition%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Single-Column%20Table%20with%20Row%20Shown%20Based%20on%20Condition%20Data%201.json)
from the example, and try to make a single-column table with a row shown based on a condition online for free by using one of
the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Bind Single-Column Table Rows to a Collection Based on a Condition

{{% alert %}}

This guide focuses on usage of `if` tags nested to `foreach` tags within single-column tables. However, binding of
single-column table rows to a collection based on a condition can also be done using `foreach` tags with [filtering of
the collection]({{< ref "../../binding-data/binding-collections/filtering-collection/" >}}) applied.

{{% /alert %}}

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include single-column-table-with-rows-bound-to-collection-based-on-condition-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a
table](https://support.microsoft.com/en-us/office/insert-a-table-a138f745-73ef-4879-b99a-2f3d38be612a#platform=Windows)
with one column and [format
elements of the table](https://support.microsoft.com/en-us/office/format-a-table-e6e77bc6-1f4e-467e-b818-2e2acc488006)
to use it as a template.

3. Add static content like a column header to the table, if needed.

4. Bind the table to a data collection by adding an opening `foreach` tag to the beginning of a row to be repeated for every
item of the collection as per the example:
{{< highlight "c#" >}}
<<foreach [in items]>>
{{< /highlight >}}

5. Add a closing `foreach` tag with a `greedy` switch to the end of a row to be repeated for every item of the collection
like so:
{{< highlight "c#" >}}
<</foreach -greedy>>
{{< /highlight >}}

{{% alert %}}

Opening and closing `foreach` tags can be located in a single row or different rows of a single table to capture one or more
rows for repeating.

{{% /alert %}}

6. Bind visibility of a row of the table to be shown based on a condition to a Boolean value calculated upon an item of
the collection by adding an opening `if` tag to the beginning of the row after the opening `foreach` tag, for instance,
like this:
{{< highlight "c#" >}}
<<if [potentialValue >= 50000]>>
{{< /highlight >}}

7. Add a closing `if` tag with a `greedy` switch to the end of a row of the table to be shown based on a condition before
the closing `foreach` tag as follows:
{{< highlight "c#" >}}
<</if -greedy>>
{{< /highlight >}}

{{% alert %}}

Opening and closing `if` tags can be located in a single row or different rows of a single table to capture one or more rows
for showing based on the same condition.

{{% /alert %}}

8. Within the range between the opening and closing `if` tags, bind cells of the table (it can be just a single cell) to values
calculated upon an item of the data collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[leadName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[contactPerson]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[status]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[potentialValue]>>
{{< /highlight >}}

9. Review your table template before saving, it should look like this:\
\
<img src="single-column-table-with-rows-bound-to-collection-based-on-condition-template.png"
  alt="Single-column table with rows bound to a collection based on a condition template for LINQ Reporting Engine in C#."
  style="width:625px"/>

10. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "091dc5121b1d33ca66031aa3c04b72f9" "binding-single-column-table-rows-to-collection-based-on-condition.cs" >}}

## Single-Column Table with Rows Bound to a Collection Based on a Condition Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="single-column-table-with-rows-bound-to-collection-based-on-condition-report.png"
  alt="Single-column table with rows bound to a collection based on a condition report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Single-Column%20Table%20with%20Rows%20Bound%20to%20Collection%20Based%20on%20Condition%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Single-Column%20Table%20with%20Rows%20Bound%20to%20Collection%20Based%20on%20Condition%20Data.json)
from the example, and try to make a single-column table with rows bound to a collection based on a condition online for free
by using one of the options:\
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