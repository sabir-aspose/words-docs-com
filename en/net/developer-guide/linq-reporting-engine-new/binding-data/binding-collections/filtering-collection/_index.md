---
title: Filtering Collection in C#
second_title: Aspose.Words for .NET
articleTitle: Filtering Collection
linktitle: Filtering Collection
description: "How to filter a collection using LINQ Reporting Engine in C#."
type: docs
weight: 10
url: /net/filtering-collection/
---

Filtering a collection during building a report enables the selection of specific data points that meet defined criteria,
ensuring that only relevant information is included. This targeted approach helps streamline the reporting process, allowing
users to focus on key insights and trends without being overwhelmed by extraneous data. You can filter a collection while
making a report using LINQ Reporting Engine in C#.

## How to Filter a Collection

{{% alert %}}

Although this guide deals with text blocks, the same approach can be applied to any template blocks such as
[lists]({{< ref "../../../building-lists/" >}}), [table rows and columns]({{< ref "../../../building-tables/" >}}), 
[charts]({{< ref "../../../building-charts/" >}}), and others.

{{% /alert %}}

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include collection-filtering-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a text block to a data collection by adding an opening `foreach` tag to the beginning of the block
and applying collection filtering in one of the following ways as per your requirements:

    * To filter all collection items based on a predicate, use [the `Where` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.where?view=net-8.0#system-linq-enumerable-where-1(system-collections-generic-ienumerable((-0))-system-func((-0-system-boolean)))),
for instance, like so:
{{< highlight "c#" >}}
<<foreach [in items.Where(i => i.industry == "Technology")]>>
{{< /highlight >}}

    * To keep collection items as long as a specified condition is true, apply [the `TakeWhile` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.takewhile?view=net-8.0#system-linq-enumerable-takewhile-1(system-collections-generic-ienumerable((-0))-system-func((-0-system-boolean))))
as per the example:
{{< highlight "c#" >}}
<<foreach [in items.TakeWhile(i => i.revenue > 5000000)]>>
{{< /highlight >}}

    * To bypass collection items as long as a specified condition is true and keep the remaining items, use [the `SkipWhile` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.skipwhile?view=net-8.0#system-linq-enumerable-skipwhile-1(system-collections-generic-ienumerable((-0))-system-func((-0-system-boolean)))),
for instance, this way:
{{< highlight "c#" >}}
<<foreach [in items.SkipWhile(i => i.revenue >= 5000000)]>>
{{< /highlight >}}

    * To keep a specified number of items from the start of the collection, apply [the `Take` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.take?view=net-8.0#system-linq-enumerable-take-1(system-collections-generic-ienumerable((-0))-system-int32))
similarly to this:
{{< highlight "c#" >}}
<<foreach [in items.Take(3)]>>
{{< /highlight >}}

    * To bypass a specified number of items from the start of the collection and keep the remaining items, use [the `Skip` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.skip?view=net-8.0), for instance, as per the snippet:
{{< highlight "c#" >}}
<<foreach [in items.Skip(5)]>>
{{< /highlight >}}

3. Add a closing `foreach` tag to the end of the text block like that:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

4. Bind the text block to a value calculated upon an item of the collection by adding an expression tag to the block between
the opening and closing `foreach` tags such as the following one:
{{< highlight "c#" >}}
<<[name]>>
{{< /highlight >}}

5. Review your collection filtering template before saving. Depending on your use cases, the template should contain one or
several blocks that look like these:\
\
<img src="collection-filtering-template.png"
  alt="Collection filtering template for LINQ Reporting Engine in C#."
  style="width:395px"/>

6. Build your report filtering a collection using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "2a372b3e0a32f6ecd34fccdfdc786d6f" "filtering-collection.cs" >}}

## Collection Filtering Report Example

After taking all the steps, LINQ Reporting Engine creates a collection filtering report as follows:\
\
<img src="collection-filtering-report.png"
  alt="Collection filtering report created by LINQ Reporting Engine in C#."
  style="width:396px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Collection%20Filtering%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Collection%20Filtering%20Data.json)
from the example, and try to make a report filtering a collection online for free by using one of the options:\
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