---
title: Inserting Bookmark in C#
second_title: Aspose.Words for .NET
articleTitle: Inserting Bookmark
linktitle: Inserting Bookmark
description: "How to insert a bookmark using LINQ Reporting Engine in C#."
type: docs
weight: 10
url: /net/inserting-bookmark/
---

Inserting a bookmark is useful for creating an internal navigation system, which functions like a custom, interactive table of
contents or index. This allows readers to efficiently jump directly to specific sections, charts, or data points without
manually scrolling through many pages. You can insert a bookmark using LINQ Reporting Engine in C#.

## How to Insert a Bookmark

1. Prepare data for your bookmark in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include bookmark-inserting-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, create a template document, go to a position within its text at which to start a bookmark, and bind
the name of the bookmark to a value by adding a `bookmark` tag, for instance, like so:
{{< highlight "c#" >}}
<<bookmark [bookmarkName]>>
{{< /highlight >}}

3. Add a closing `bookmark` tag at a position within the template's text where to end the bookmark this way:
{{< highlight "c#" >}}
<</bookmark>>
{{< /highlight >}}

{{% alert %}}

Opening and closing `bookmark` tags cannot be located within a chart.

{{% /alert %}}

4. Review your bookmark template before saving, it should look like this:\
\
<img src="bookmark-inserting-template.png"
  alt="Bookmark inserting template for LINQ Reporting Engine in C#."
  style="width:590px"/>

5. Build your bookmark using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "c661a51da3e161fff0bbc1b38214a779" "inserting-bookmark.cs" >}}

## Bookmark Inserting Report Example

After taking all the steps, LINQ Reporting Engine creates a bookmark report as follows:\
\
<img src="bookmark-inserting-report.png"
  alt="Bookmark inserting report created by LINQ Reporting Engine in C#."
  style="width:672px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Bookmark%20Inserting%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Bookmark%20Inserting%20Data.json)
from the example, and try to insert a bookmark online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## See Also

- [Working with Links]({{< ref "../../working-with-links/" >}})
- [LINQ Reporting Engine]({{< ref "../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../common/footer.md" %}}