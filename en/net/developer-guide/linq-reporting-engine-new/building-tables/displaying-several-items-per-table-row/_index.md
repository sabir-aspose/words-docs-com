---
title: Displaying Several Items per Table Row in C#
second_title: Aspose.Words for .NET
articleTitle: Displaying Several Items per Table Row
linktitle: Displaying Several Items per Table Row
description: "How to display several items per table row using LINQ Reporting Engine in C#."
type: docs
weight: 60
url: /net/displaying-several-items-per-table-row/
---

Displaying several items per table row allows for a more compact and comprehensive view of related data, enabling users to
compare multiple attributes or categories at once. This format enhances clarity and efficiency by consolidating information,
making it easier for users to analyze relationships and draw insights without needing to navigate through multiple rows or
tables. You can build a table with several items displayed per row using LINQ Reporting Engine in C#.

## How to Display Several Items per Table Row

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-several-items-displayed-per-row-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a single-row
table](https://support.microsoft.com/en-us/office/insert-a-table-a138f745-73ef-4879-b99a-2f3d38be612a#platform=Windows)
with the number of columns equal to the number of items to display per row and [format
elements of the table](https://support.microsoft.com/en-us/office/format-a-table-e6e77bc6-1f4e-467e-b818-2e2acc488006)
to use it as a template.

3. Bind the table to a data collection by adding an opening `foreach` tag to the beginning of the table's single row (that is
to be repeated until all items of the collection are visited) as per the example:
{{< highlight "c#" >}}
<<foreach [in items]>>
{{< /highlight >}}

4. Add a closing `foreach` tag to the end of the row like so:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

5. Bind the first cell of the row to values calculated upon an item of the collection by adding expression tags to the cell
such as the following ones:
{{< highlight "c#" >}}
<<[productName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[supplierName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[price]>>
{{< /highlight >}}

6. Use literal-string expression tags to form static parts of the cell's content, for instance, this way:
{{< highlight "c#" >}}
<<["by "]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<["Price: "]>>
{{< /highlight >}}

7. Starting from the second cell, add a `next` tag to the beginning of every cell of the table's single row as follows:
{{< highlight "c#" >}}
<<next>>
{{< /highlight >}}

8. Copy content of the first cell of the row after the opening `foreach` tag to every of the rest of the row's cells after
a `next` tag and before the closing `foreach` tag, if any.

9. Review your table template before saving, it should look like this:\
\
<img src="table-with-several-items-displayed-per-row-template.png"
  alt="Table with several items displayed per row template for LINQ Reporting Engine in C#."
  style="width:625px"/>

10. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "6d983652a385c662c3a60602d4e54f16" "displaying-several-items-per-table-row.cs" >}}

## Table with Several Items Displayed per Row Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-several-items-displayed-per-row-report.png"
  alt="Table with several items displayed per row report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Several%20Items%20Displayed%20per%20Row%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Several%20Items%20Displayed%20per%20Row%20Data.json)
from the example, and try to make a table with several items displayed per row online for free by using one of the options:\
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