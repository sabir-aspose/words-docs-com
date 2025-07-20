---
title: Getting Unique Collection Items in C#
second_title: Aspose.Words for .NET
articleTitle: Getting Unique Collection Items
linktitle: Getting Unique Collection Items
description: "How to get unique collection items using LINQ Reporting Engine in C#."
type: docs
weight: 70
url: /net/getting-unique-collection-items/
---

Getting unique collection items during building a report eliminates duplicates, providing a clear and concise overview of
distinct data points. This process helps users focus on the variety of items or categories represented, enabling better
analysis of trends and patterns without redundancy. You can get unique collection items while making a report using LINQ
Reporting Engine in C#.

## How to Get Unique Collection Items

{{% alert %}}

Although this guide deals with text blocks, the same approach can be applied to any template blocks such as
[lists]({{< ref "../../../building-lists/" >}}), [table rows and columns]({{< ref "../../../building-tables/" >}}), 
[charts]({{< ref "../../../building-charts/" >}}), and others.

{{% /alert %}}

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include unique-collection-items-getting-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a text block to a data collection by adding an opening `foreach` tag to the beginning of the block
and excluding duplicate collection items using [the `Distinct` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.distinct?view=net-9.0#system-linq-enumerable-distinct-1(system-collections-generic-ienumerable((-0))))
as per the example:
{{< highlight "c#" >}}
<<foreach [method in items.Select(i => i.paymentMethod).Distinct().OrderBy(m => m)]>>
{{< /highlight >}}

{{% alert %}}

In this case, [a collection projection is applied using
`Select`]({{< ref "../applying-collection-projection/" >}}) to form a collection to exclude duplicate items from. Also, since
the projection does not imply any ordering, the result collection is further [sorted using
`OrderBy`]({{< ref "../sorting-collection/" >}}) to get consistent output as shown in the example. Depending on structure of
your data, these extra steps may be not needed.

{{% /alert %}}

3. Add a closing `foreach` tag to the end of the text block like that:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

4. Bind the text block to values calculated upon an item of the result collection by adding expression tags to the block
between the opening and closing `foreach` tags such as the following one:
{{< highlight "c#" >}}
<<[method]>>
{{< /highlight >}}

5. Review your unique collection items getting template before saving, it should look like this:\
\
<img src="unique-collection-items-getting-template.png"
  alt="Unique collection items getting template for LINQ Reporting Engine in C#."
  style="width:529px"/>

6. Build your report getting unique collection items using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "fed41697c49040e617f232ff128a2c21" "getting-unique-collection-items.cs" >}}

## Unique Collection Items Getting Report Example

After taking all the steps, LINQ Reporting Engine creates a unique collection items getting report as follows:\
\
<img src="unique-collection-items-getting-report.png"
  alt="Unique collection items getting report created by LINQ Reporting Engine in C#."
  style="width:156px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Unique%20Collection%20Items%20Getting%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Unique%20Collection%20Items%20Getting%20Data.json)
from the example, and try to make a report getting unique collection items online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## See Also

- [Binding Collections]({{< ref "../../binding-collections/" >}})
- [Binding Data]({{< ref "../../../binding-data/" >}})
- [LINQ Reporting Engine]({{< ref "../../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../../common/footer.md" %}}