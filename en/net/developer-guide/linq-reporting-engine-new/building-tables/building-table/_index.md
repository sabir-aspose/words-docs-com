---
title: Building Table in C#
second_title: Aspose.Words for .NET
articleTitle: Building Table
linktitle: Building Table
description: "How to make a table using LINQ Reporting Engine in C#."
type: docs
weight: 10
url: /net/building-table/
---

Utilizing [tables](https://en.wikipedia.org/wiki/Table_(information)) for data presentation enhances readability and
facilitates quick access to specific information, making it easier for audiences to interpret complex datasets. Their
systematic layout aids in the efficient communication of quantitative data, ensuring that key insights are readily accessible.
You can make a table using LINQ Reporting Engine in C#.

## How to Build a Table

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a
table](https://support.microsoft.com/en-us/office/insert-a-table-a138f745-73ef-4879-b99a-2f3d38be612a#platform=Windows)
of a necessary size and [format its
elements](https://support.microsoft.com/en-us/office/format-a-table-e6e77bc6-1f4e-467e-b818-2e2acc488006)
to use it as a template.

3. Add static content like headers to the table, if needed.

4. Bind cells of the table to values by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[customerName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[orderDate]:"dd\/MM\/yyyy">>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[totalAmount]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[status]>>
{{< /highlight >}}

5. Review your table template before saving, it should look like this:\
\
<img src="table-template.png"
  alt="Table template for LINQ Reporting Engine in C#."
  style="width:625px"/>

6. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "1db755b118593b067e1de46ad5fbe550" "building-table.cs" >}}

## Table Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-report.png"
  alt="Table report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20Data.json)
from the example, and try to make a table online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Bind Table Rows to a Collection

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-rows-bound-to-collection-data.json >}}
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
<<[productName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[supplierName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[price]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[stockQuantity]>>
{{< /highlight >}}

7. Review your table template before saving, it should look like this:\
\
<img src="table-with-rows-bound-to-collection-template.png"
  alt="Table with rows bound to a collection template for LINQ Reporting Engine in C#."
  style="width:625px"/>

8. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "046e728500b12abd8ed5c68274657d55" "binding-table-rows-to-collection.cs" >}}

## Table with Rows Bound to a Collection Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-rows-bound-to-collection-report.png"
  alt="Table with rows bound to a collection report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Rows%20Bound%20to%20Collection%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Rows%20Bound%20to%20Collection%20Data.json)
from the example, and try to make a table with rows bound to a collection online for free by using one of the options:\
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