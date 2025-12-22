---
title: Inserting HTML in C#
second_title: Aspose.Words for .NET
articleTitle: Inserting HTML
linktitle: Inserting HTML
description: "How to insert HTML using LINQ Reporting Engine in C#."
type: docs
weight: 30
url: /net/inserting-html/
---

Inserting [HTML](https://en.wikipedia.org/wiki/HTML) empowers dynamic formatting by using tags to apply conditional styles -
such as highlighting specific data points or creating complex layouts - that transform static text into a visually engaging
and responsive experience. Also, this capability becomes a necessity when your source data already contains HTML strings.
You can insert HTML using LINQ Reporting Engine in C#.

## How to Insert HTML

1. Prepare data for your document in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include html-inserting-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, create a template document and bind the source of HTML to be inserted to an html-string value by adding
an `html` tag or an expression tag with an `html` switch at a position within the template's text where to insert HTML, for
instance, like so:
{{< highlight "c#" >}}
<<html [grossRevenue]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[netProfitMargin] -html>>
{{< /highlight >}}

{{% alert %}}

* An expression tag with an `html` switch and an `html` tag with no switches applied can be used interchangeably.

* An `html` tag or an expression tag with an `html` switch cannot be used within charts.

{{% /alert %}}

3. Review your importing template before saving, it should look like this:\
\
<img src="html-inserting-template.png"
  alt="HTML inserting template for LINQ Reporting Engine in C#."
  style="width:280px"/>

4. Build your HTML using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "3c23d9783e82ab2f06ceb01706f4594b" "inserting-html.cs" >}}

## HTML Inserting Report Example

After taking all the steps, LINQ Reporting Engine creates an importing report as follows:\
\
<img src="html-inserting-report.png"
  alt="HTML inserting report created by LINQ Reporting Engine in C#."
  style="width:237px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/HTML%20Inserting%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/HTML%20Inserting%20Data.json)
from the example, and try to insert HTML online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Insert HTML Keeping Source Styles

{{% alert %}}

By default, content of HTML being inserted inherits styles of a template document to make report content more consistent.
This guide shows how to preserve styles of HTML being inserted - to make it look like in a browser - when it is necessary.

{{% /alert %}}

1. Prepare data for your document in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include html-inserting-with-source-styles-keeping-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, create a template document and bind the source of HTML to be inserted to an html-string value by adding
an `html` tag with a `sourceStyles` switch at a position within the template's text where to insert HTML, for instance, like so:
{{< highlight "c#" >}}
<<html [statusHtml] -sourceStyles>>
{{< /highlight >}}

{{% alert %}}

An `html` tag cannot be used within charts.

{{% /alert %}}

3. Review your importing template before saving, it should look like this:\
\
<img src="html-inserting-with-source-styles-keeping-template.png"
  alt="HTML inserting with source styles keeping template for LINQ Reporting Engine in C#."
  style="width:256px"/>

4. Build your HTML using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "42a0b17f08762d99db5e5046fafd4955" "inserting-html-keeping-source-styles.cs" >}}

## HTML Inserting with Source Styles Keeping Report Example

After taking all the steps, LINQ Reporting Engine creates an importing report as follows:\
\
<img src="html-inserting-with-source-styles-keeping-report.png"
  alt="HTML inserting with source styles keeping report created by LINQ Reporting Engine in C#."
  style="width:257px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/HTML%20Inserting%20with%20Source%20Styles%20Keeping%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/HTML%20Inserting%20with%20Source%20Styles%20Keeping%20Data.json)
from the example, and try to insert HTML keeping source styles online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## See Also

- [Importing Content]({{< ref "../../importing-content/" >}})
- [LINQ Reporting Engine]({{< ref "../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../common/footer.md" %}}