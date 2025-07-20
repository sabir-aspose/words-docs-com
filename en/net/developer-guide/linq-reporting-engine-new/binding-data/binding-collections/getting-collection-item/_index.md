---
title: Getting Collection Item in C#
second_title: Aspose.Words for .NET
articleTitle: Getting Collection Item
linktitle: Getting Collection Item
description: "How to get a collection item using LINQ Reporting Engine in C#."
type: docs
weight: 80
url: /net/getting-collection-item/
---

Getting a collection item (for example, by its index) during building a report allows for precise access to specific data
points, enabling detailed examination of individual records within a larger dataset. This targeted retrieval can facilitate
deeper insights and direct comparisons, enhancing the overall quality and relevance of findings from the data. You can get
a collection item while making a report using LINQ Reporting Engine in C#.

## How to Get a Collection Item

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include collection-item-getting-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a template document to values calculated upon an item of a data collection by adding expression tags
to the template and obtaining the item in one of the following ways as per your requirements:

    * To reference the first collection item, apply [the `First` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.first?view=net-9.0#system-linq-enumerable-first-1(system-collections-generic-ienumerable((-0)))),
for instance, like so:
{{< highlight "c#" >}}
<<[items.First().division]>>
{{< /highlight >}}

    * To recieve the first collection item or a default value if the collection contains no items, use [the `FirstOrDefault`
LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.firstordefault?view=net-9.0#system-linq-enumerable-firstordefault-1(system-collections-generic-ienumerable((-0)))),
for example, as follows:
{{< highlight "c#" >}}
<<[items.First().subdivisions.FirstOrDefault()?.name]>>
{{< /highlight >}}

    * To find the first collection item that satisfies a specified condition, apply [the `First` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.first?view=net-9.0#system-linq-enumerable-first-1(system-collections-generic-ienumerable((-0))-system-func((-0-system-boolean)))),
for instance, as per the snippet:
{{< highlight "c#" >}}
<<[items.First(i => i.ordersCancelled > 120).division]>>
{{< /highlight >}}

    * To get the first collection item that satisfies a specified condition or a default value if there is no such item, use
[the `FirstOrDefault` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.firstordefault?view=net-9.0#system-linq-enumerable-firstordefault-1(system-collections-generic-ienumerable((-0))-system-func((-0-system-boolean)))),
for example, this way:
{{< highlight "c#" >}}
<<[items.FirstOrDefault(i => i.ordersCancelled < 100)?.division]>>
{{< /highlight >}}

    * To pick the last collection item, apply [the `Last` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.last?view=net-9.0#system-linq-enumerable-last-1(system-collections-generic-ienumerable((-0)))),
for instance, like that:
{{< highlight "c#" >}}
<<[items.Last().division]>>
{{< /highlight >}}

    * To retrieve the last collection item or a default value if the collection contains no items, use [the `LastOrDefault`
LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.lastordefault?view=net-9.0#system-linq-enumerable-lastordefault-1(system-collections-generic-ienumerable((-0)))),
for example, in this fashion:
{{< highlight "c#" >}}
<<[items.First().subdivisions.LastOrDefault()?.name]>>
{{< /highlight >}}

    * To obtain the last collection item that satisfies a specified condition, apply [the `Last` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.last?view=net-9.0#system-linq-enumerable-last-1(system-collections-generic-ienumerable((-0))-system-func((-0-system-boolean)))),
for instance, as follows:
{{< highlight "c#" >}}
<<[items.Last(i => i.ordersDelivered < 1500).division]>>
{{< /highlight >}}

    * To recieve the last collection item that satisfies a specified condition or a default value if there is no such item, use
[the `LastOrDefault` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.lastordefault?view=net-9.0#system-linq-enumerable-lastordefault-1(system-collections-generic-ienumerable((-0))-system-func((-0-system-boolean))))
as per the example:
{{< highlight "c#" >}}
<<[items.LastOrDefault(i => i.ordersCancelled > 200)?.division]>>
{{< /highlight >}}

    * To reference the single collection item, apply [the `Single` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.single?view=net-9.0#system-linq-enumerable-single-1(system-collections-generic-ienumerable((-0)))),
for instance, like this:
{{< highlight "c#" >}}
<<[items.Last().subdivisions.Single().name]>>
{{< /highlight >}}

    * To get the single collection item or a default value if the collection contains no items, use [the `SingleOrDefault`
LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.singleordefault?view=net-9.0#system-linq-enumerable-singleordefault-1(system-collections-generic-ienumerable((-0)))),
for example, this way:
{{< highlight "c#" >}}
<<[items.First().subdivisions.SingleOrDefault()?.name]>>
{{< /highlight >}}

    * To find the single collection item that satisfies a specified condition, apply [the `Single` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.single?view=net-9.0#system-linq-enumerable-single-1(system-collections-generic-ienumerable((-0))-system-func((-0-system-boolean)))),
for instance, like that:
{{< highlight "c#" >}}
<<[items.Single(i => i.division == "Division B").ordersDelivered]>>
{{< /highlight >}}

    * To retrieve the single collection item that satisfies a specified condition or a default value if there is no such item, use
[the `SingleOrDefault` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.singleordefault?view=net-9.0#system-linq-enumerable-singleordefault-1(system-collections-generic-ienumerable((-0))-system-func((-0-system-boolean))))
similarly to this:
{{< highlight "c#" >}}
<<[items.SingleOrDefault(i => i.division == "Division Z")?.ordersCancelled]>>
{{< /highlight >}}

    * To pick a collection item with a specified index, apply [the `ElementAt` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.elementat?view=net-9.0#system-linq-enumerable-elementat-1(system-collections-generic-ienumerable((-0))-system-int32)),
for example, as per the snippet:
{{< highlight "c#" >}}
<<[items.ElementAt(2).division]>>
{{< /highlight >}}

    * To recieve a collection item with a specified index or a default value if there is no such item, use
[the `ElementAtOrDefault` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.elementatordefault?view=net-9.0#system-linq-enumerable-elementatordefault-1(system-collections-generic-ienumerable((-0))-system-int32)),
for instance, in this fashion:
{{< highlight "c#" >}}
<<[items.ElementAtOrDefault(6)?.division]>>
{{< /highlight >}}

{{% alert %}}

Often, it is required to access multiple members of a collection item obtained in one of the abovementioned ways. In that case,
it becomes helpful to store the item into a [variable]({{< ref "../../working-with-variables/" >}}) and then use the variable
several times to access the members.

{{% /alert %}}

3. Review your collection item getting template before saving. Depending on your use cases, the template should contain
one or several blocks that look like these:\
\
<img src="collection-item-getting-template.png"
  alt="Collection item getting template for LINQ Reporting Engine in C#."
  style="width:453px"/>

4. Build your report getting a collection item using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "9bf7bf0f8aab16fec51e577ce64d8634" "getting-collection-item.cs" >}}

## Collection Item Getting Report Example

After taking all the steps, LINQ Reporting Engine creates a collection item getting report as follows:\
\
<img src="collection-item-getting-report.png"
  alt="Collection item getting report created by LINQ Reporting Engine in C#."
  style="width:394px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Collection%20Item%20Getting%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Collection%20Item%20Getting%20Data.json)
from the example, and try to make a report getting a collection item online for free by using one of the options:\
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