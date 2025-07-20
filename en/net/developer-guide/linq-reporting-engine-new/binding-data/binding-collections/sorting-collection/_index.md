---
title: Sorting Collection in C#
second_title: Aspose.Words for .NET
articleTitle: Sorting Collection
linktitle: Sorting Collection
description: "How to sort a collection using LINQ Reporting Engine in C#."
type: docs
weight: 20
url: /net/sorting-collection/
---

[Sorting a collection](https://en.wikipedia.org/wiki/Sorting) during building a report organizes data in a meaningful order,
making it easier to identify patterns, trends, and outliers. This structured presentation enhances readability and allows users
to quickly analyze information, facilitating informed decision-making based on prioritized insights. You can sort a collection
while making a report using LINQ Reporting Engine in C#.

## How to Sort a Collection

{{% alert %}}

Although this guide deals with text blocks, the same approach can be applied to any template blocks such as
[lists]({{< ref "../../../building-lists/" >}}), [table rows and columns]({{< ref "../../../building-tables/" >}}), 
[charts]({{< ref "../../../building-charts/" >}}), and others.

{{% /alert %}}

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include collection-sorting-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a text block to a data collection by adding an opening `foreach` tag to the beginning of the block
and applying collection sorting in one of the following ways as per your requirements:

    * To sort collection items in ascending order according to a key, use [the `OrderBy` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.orderby?view=net-8.0#system-linq-enumerable-orderby-2(system-collections-generic-ienumerable((-0))-system-func((-0-1)))),
for instance, like so:
{{< highlight "c#" >}}
<<foreach [in items.OrderBy(i => i.price)]>>
{{< /highlight >}}

    * To sort collection items in descending order according to a key, apply [the `OrderByDescending` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.orderbydescending?view=net-8.0#system-linq-enumerable-orderbydescending-2(system-collections-generic-ienumerable((-0))-system-func((-0-1))))
as per the example:
{{< highlight "c#" >}}
<<foreach [in items.OrderByDescending(i => i.price)]>>
{{< /highlight >}}

    * To sort collection items in ascending order according to multiple keys, use the `OrderBy` and
[`ThenBy`](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.thenby?view=net-8.0#system-linq-enumerable-thenby-2(system-linq-iorderedenumerable((-0))-system-func((-0-1))))
LINQ extension methods (the latter can be applied several times), for instance, this way:
{{< highlight "c#" >}}
<<foreach [in items.OrderBy(i => i.price).ThenBy(i => i.stock)]>>
{{< /highlight >}}

    * To sort collection items in descending order according to multiple keys, use the `OrderByDescending` and
[`ThenByDescending`](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.thenbydescending?view=net-8.0#system-linq-enumerable-thenbydescending-2(system-linq-iorderedenumerable((-0))-system-func((-0-1))))
LINQ extension methods (the latter can be applied several times) similarly to this:
{{< highlight "c#" >}}
<<foreach [in items.OrderByDescending(i => i.price).ThenByDescending(i => i.stock)]>>
{{< /highlight >}}

{{% alert %}}

`OrderBy` and `OrderByDescending` as well as `ThenBy` and `ThenByDescending` can be used interchangeably. Thus, you can mix
ascending and descending ordering any way you need.

{{% /alert %}}

3. Add a closing `foreach` tag to the end of the text block like that:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

4. Bind the text block to values calculated upon an item of the collection by adding expression tags to the block between
the opening and closing `foreach` tags such as the following ones:
{{< highlight "c#" >}}
<<[name]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[price]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[stock]>>
{{< /highlight >}}

5. Review your collection sorting template before saving. Depending on your use cases, the template should contain one or
several blocks that look like these:\
\
<img src="collection-sorting-template.png"
  alt="Collection sorting template for LINQ Reporting Engine in C#."
  style="width:514px"/>

6. Build your report sorting a collection using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "a1447498e89384885b576b3d9ac6a54c" "sorting-collection.cs" >}}

## Collection Sorting Report Example

After taking all the steps, LINQ Reporting Engine creates a collection sorting report as follows:\
\
<img src="collection-sorting-report.png"
  alt="Collection sorting report created by LINQ Reporting Engine in C#."
  style="width:351px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Collection%20Sorting%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Collection%20Sorting%20Data.json)
from the example, and try to make a report sorting a collection online for free by using one of the options:\
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