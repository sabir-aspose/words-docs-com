---
title: Changing Table Headers in C#
second_title: Aspose.Words for .NET
articleTitle: Changing Table Headers
linktitle: Changing Table Headers
description: "How to change table headers using LINQ Reporting Engine in C#."
type: docs
weight: 13
url: /net/changing-table-headers/
---

Changing table headers allows for the customization of column titles to better reflect the content and context of the data
presented. This flexibility enhances clarity and understanding for users, ensuring that they can quickly grasp the significance
of each column and the information it contains, leading to more effective data interpretation. You can build a table with
changing headers using LINQ Reporting Engine in C#.

## How to Change Table Headers

1. Prepare data for your table in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include table-with-changing-headers-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a
table](https://support.microsoft.com/en-us/office/insert-a-table-a138f745-73ef-4879-b99a-2f3d38be612a#platform=Windows)
with a necessary number of columns and [format its
elements](https://support.microsoft.com/en-us/office/format-a-table-e6e77bc6-1f4e-467e-b818-2e2acc488006)
to use it as a template.

3. Add static content like some of headers to the table, if needed.

4. Bind header cells of the table to values by adding expression tags to the cells, for instance, like these:
{{< highlight "c#" >}}
<<[header2]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[header3]>>
{{< /highlight >}}

5. Bind the table to a data collection by adding an opening `foreach` tag to the beginning of a row to be repeated for every
item of the collection as per the example:
{{< highlight "c#" >}}
<<foreach [in items]>>
{{< /highlight >}}

6. Add a closing `foreach` tag to the end of a row to be repeated for every item of the collection like so:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

{{% alert %}}

Opening and closing `foreach` tags can be located in a single row or different rows of a single table to capture one or more
rows for repeating.

{{% /alert %}}

7. Within the range between the opening and closing `foreach` tags, bind cells of the table to values calculated upon an item
of the collection by adding expression tags to the cells such as the following ones:
{{< highlight "c#" >}}
<<[region]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[revenue]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[expenses]>>
{{< /highlight >}}

8. Review your table template before saving, it should look like this:\
\
<img src="table-with-changing-headers-template.png"
  alt="Table with changing headers template for LINQ Reporting Engine in C#."
  style="width:625px"/>

9. Build your table using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "16ccc82dfb99f3489159a9462aa3daab" "changing-table-headers.cs" >}}

## Table with Changing Headers Report Example

After taking all the steps, LINQ Reporting Engine creates a table report as follows:\
\
<img src="table-with-changing-headers-report.png"
  alt="Table with changing headers report created by LINQ Reporting Engine in C#."
  style="width:625px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Changing%20Headers%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Table%20with%20Changing%20Headers%20Data.json)
from the example, and try to make a table with changing headers online for free by using one of the options:\
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