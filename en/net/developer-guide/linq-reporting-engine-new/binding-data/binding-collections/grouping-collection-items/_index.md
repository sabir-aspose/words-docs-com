---
title: Grouping Collection Items in C#
second_title: Aspose.Words for .NET
articleTitle: Grouping Collection Items
linktitle: Grouping Collection Items
description: "How to group collection items using LINQ Reporting Engine in C#."
type: docs
weight: 30
url: /net/grouping-collection-items/
---

Grouping collection items during building a report consolidates related data into aggregated categories, facilitating
navigation and understanding of the information presented. This approach enhances data analysis by providing insights into
different segments of the data, making it easier for users to understand trends and make comparisons within the dataset.
You can group collection items while making a report using LINQ Reporting Engine in C#.

## How to Group Collection Items

{{% alert %}}

Although this guide deals with text blocks, the same approach can be applied to any template blocks such as
[lists]({{< ref "../../../building-lists/" >}}), [table rows and columns]({{< ref "../../../building-tables/" >}}), 
[charts]({{< ref "../../../building-charts/" >}}), and others.

{{% /alert %}}

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include collection-items-grouping-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a text block to a data collection by adding an opening `foreach` tag to the beginning of the block
and applying grouping of collection items in one of the following ways as per your requirements:

    * To group collection items according to a single key, use [the `GroupBy` LINQ extension
method](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.groupby?view=net-9.0#system-linq-enumerable-groupby-2(system-collections-generic-ienumerable((-0))-system-func((-0-1))))
with a selector function returning the key, for instance, like so:
{{< highlight "c#" >}}
<<foreach [group in items.GroupBy(i => i.division).OrderBy(g => g.Key)]>>
{{< /highlight >}}

    * To group collection items according to multiple keys, apply the `GroupBy` LINQ extension method with a selector function
returning an instance of [an anonymous type](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/types/anonymous-types)
with properties initialized upon the keys similarly to this:
{{< highlight "c#" >}}
<<foreach [group in items.GroupBy(i => new { i.division, i.quarter }).OrderBy(g => g.Key.division).ThenBy(g => g.Key.quarter)]>>
{{< /highlight >}}

{{% alert %}}

Since grouping itself does not imply ordering, it often makes sense to [sort groups of items]({{< ref "../sorting-collection/" >}})
using the `OrderBy`, `OrderByDescending`, `ThenBy`, and `ThenByDescending` LINQ extension methods in order to get consistent
output as shown in this guide.

{{% /alert %}}

3. Add a closing `foreach` tag to the end of the text block like that:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

4. Bind the text block to values calculated upon [the Key
property](https://learn.microsoft.com/en-us/dotnet/api/system.linq.igrouping-2.key?view=net-9.0#system-linq-igrouping-2-key)
of a group of collection items by adding expression tags to the block between the opening and closing `foreach` tags such as
the following ones depending on how the group's key was initialized:
{{< highlight "c#" >}}
<<[group.Key]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[group.Key.division]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[group.Key.quarter]>>
{{< /highlight >}}

5. Bind an inner text block to items of a group by adding an inner opening `foreach` tag before the outer closing `foreach` tag
and applying ordering to the items as per one of the examples according to your scenario:
{{< highlight "c#" >}}
<<foreach [in group.OrderBy(i => i.quarter).ThenBy(i => i.region)]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<foreach [in group.OrderBy(i => i.region)]>>
{{< /highlight >}}

{{% alert %}}

Ordering of collection items forming a group is used under the same reasoning as ordering of groups themselves and can be
omitted, if needed.

{{% /alert %}}

6. Add an inner closing `foreach` tag before the outer closing `foreach` tag this way:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

7. Bind the inner text block to values calculated upon an item of a group by adding expression tags to the block between
the inner opening and closing `foreach` tags like the following ones:
{{< highlight "c#" >}}
<<[quarter]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[region]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[sales]>>
{{< /highlight >}}

8. Review your collection items grouping template before saving. Depending on your use cases, the template should contain one or
several blocks that look like these:\
\
<img src="collection-items-grouping-template.png"
  alt="Collection items grouping template for LINQ Reporting Engine in C#."
  style="width:435px"/>

9. Build your report grouping collection items using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "33a1a11b80298cf4e826181f5c1fb430" "grouping-collection-items.cs" >}}

## Collection Items Grouping Report Example

After taking all the steps, LINQ Reporting Engine creates a collection items grouping report as follows:\
\
<img src="collection-items-grouping-report.png"
  alt="Collection items grouping report created by LINQ Reporting Engine in C#."
  style="width:249px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Collection%20Items%20Grouping%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Collection%20Items%20Grouping%20Data.json)
from the example, and try to make a report grouping collection items online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## See Also

- [Sorting Collection]({{< ref "../sorting-collection/" >}})
- [Binding Collections]({{< ref "../../binding-collections/" >}})
- [Binding Data]({{< ref "../../../binding-data/" >}})
- [LINQ Reporting Engine]({{< ref "../../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../../common/footer.md" %}}