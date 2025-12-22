---
title: Inserting Document in C#
second_title: Aspose.Words for .NET
articleTitle: Inserting Document
linktitle: Inserting Document
description: "How to insert a document using LINQ Reporting Engine in C#."
type: docs
weight: 10
url: /net/inserting-document/
---

Inserting a [document](https://en.wikipedia.org/wiki/Document) ensures consistent messaging across various sections of a report
or multiple reports while significantly reducing the time spent on manual recreation. This modular approach establishes a single
source of truth, allowing updates made in one document to automatically propagate everywhere it is inserted to maintain accuracy
and compliance. You can insert a document using LINQ Reporting Engine in C#.

## How to Insert a Document

1. Prepare data for your document in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include document-inserting-data.json >}}
{{< /highlight >}}

{{% alert %}}

In this example, the additional data source `dir` - the path to a directory of a document to be inserted - is used.

{{% /alert %}}

2. In Microsoft Word, create a template document and bind the source of a document to be inserted to a [value providing
the document's data]({{< ref "#supported-values-providing-document-data" >}}) by adding a `doc` tag at a position within
the template's text where to insert the document, for instance, like so:
{{< highlight "c#" >}}
<<doc [dir + fileName]>>
{{< /highlight >}}

{{% alert %}}

A `doc` tag cannot be used within textboxes and charts.

{{% /alert %}}

3. Review your importing template before saving, it should look like this:\
\
<img src="document-inserting-template.png"
  alt="Document inserting template for LINQ Reporting Engine in C#."
  style="width:230px"/>

4. Build your document using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "3c3524dec0a8f2e460922e519cc01a03" "inserting-document.cs" >}}

## Document Inserting Report Example

After taking all the steps, LINQ Reporting Engine creates an importing report as follows:\
\
<img src="document-inserting-report.png"
  alt="Document inserting report created by LINQ Reporting Engine in C#."
  style="width:598px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Document%20Inserting%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Document%20Inserting%20Data.json)
from the example, and try to insert a document online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Insert a Document Keeping Source Styles

{{% alert %}}

By default, content of a document being inserted inherits styles of a template document to make report content more consistent.
This guide shows how to preserve styles of a document being inserted when it is necessary.

{{% /alert %}}

1. Prepare data for your document in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include document-inserting-with-source-styles-keeping-data.json >}}
{{< /highlight >}}

{{% alert %}}

In this example, the additional data source `dir` - the path to a directory of a document to be inserted - is used.

{{% /alert %}}

2. In Microsoft Word, create a template document and bind the source of a document to be inserted to a [value providing
the document's data]({{< ref "#supported-values-providing-document-data" >}}) by adding a `doc` tag with a `sourceStyles`
switch at a position within the template's text where to insert the document, for instance, like so:
{{< highlight "c#" >}}
<<doc [dir + logoFile] -sourceStyles>>
{{< /highlight >}}

{{% alert %}}

A `doc` tag cannot be used within textboxes and charts.

{{% /alert %}}

3. Review your importing template before saving, it should look like this:\
\
<img src="document-inserting-with-source-styles-keeping-template.png"
  alt="Document inserting with source styles keeping template for LINQ Reporting Engine in C#."
  style="width:249px"/>

4. Build your document using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "a56501e020dfd2c3bf5f0c8a3ff41910" "inserting-document-keeping-source-styles.cs" >}}

## Document Inserting with Source Styles Keeping Report Example

After taking all the steps, LINQ Reporting Engine creates an importing report as follows:\
\
<img src="document-inserting-with-source-styles-keeping-report.png"
  alt="Document inserting with source styles keeping report created by LINQ Reporting Engine in C#."
  style="width:629px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Document%20Inserting%20with%20Source%20Styles%20Keeping%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Document%20Inserting%20with%20Source%20Styles%20Keeping%20Data.json)
from the example, and try to insert a document keeping source styles online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Insert a Document Keeping Source Numbering

{{% alert %}}

By default, when inserting a document, numbered lists with matching identifiers are continued in a report. This guide explains
how to keep numbering for content being inserted as is when needed.

{{% /alert %}}

1. Prepare data for your document in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include document-inserting-with-source-numbering-keeping-data.json >}}
{{< /highlight >}}

{{% alert %}}

In this example, the additional data source `dir` - the path to a directory of a document to be inserted - is used.

{{% /alert %}}

2. In Microsoft Word, create a template document and bind the source of every document to be inserted to a [value providing
the document's data]({{< ref "#supported-values-providing-document-data" >}}) by adding a `doc` tag with a `sourceNumbering`
switch at a position within the template's text where to insert the document, for instance, like so:
{{< highlight "c#" >}}
<<doc [dir + targetsFile] -sourceNumbering>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<doc [dir + metricsFile] -sourceNumbering>>
{{< /highlight >}}

{{% alert %}}

A `doc` tag cannot be used within textboxes and charts.

{{% /alert %}}

3. Review your importing template before saving, it should look like this:\
\
<img src="document-inserting-with-source-numbering-keeping-template.png"
  alt="Document inserting with source numbering keeping template for LINQ Reporting Engine in C#."
  style="width:353px"/>

4. Build your document using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "066173699fd000a7ce63bc6c34babc65" "inserting-document-keeping-source-numbering.cs" >}}

## Document Inserting with Source Numbering Keeping Report Example

After taking all the steps, LINQ Reporting Engine creates an importing report as follows:\
\
<img src="document-inserting-with-source-numbering-keeping-report.png"
  alt="Document inserting with source numbering keeping report created by LINQ Reporting Engine in C#."
  style="width:618px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Document%20Inserting%20with%20Source%20Numbering%20Keeping%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Document%20Inserting%20with%20Source%20Numbering%20Keeping%20Data.json)
from the example, and try to insert a document keeping source numbering online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Insert a Document Inlining Content

{{% alert %}}

This guide walks through trimming of the last paragraph break from a document being inserted, which is most useful when
the document is single-paragraph and it is required to put the document's content within a paragraph having special formatting
such as list numbering applied. Although the guide focuses on usage of `doc` tags with `inline` switches nested to `foreach`
tags, a similar technique can be used with no `foreach` tags involved.

{{% /alert %}}

1. Prepare data for your document in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include document-inserting-with-content-inlining-data.json >}}
{{< /highlight >}}

{{% alert %}}

In this example, the additional data source `dir` - the path to a directory of a document to be inserted - is used.

{{% /alert %}}

2. In Microsoft Word, create a template document and bind a fragment of its text to a data collection to repeat the fragment
for every item of the collection by adding an opening `foreach` tag to the beginning of the fragment, for instance, like so:
{{< highlight "c#" >}}
<<foreach [in items]>>
{{< /highlight >}}

3. Bind the fragment to values calculated upon an item of the data collection by adding expression tags after the opening
`foreach` tag such as the following one:
{{< highlight "c#" >}}
<<[milestone]>>
{{< /highlight >}}

4. Bind the source of a document to be inserted to a [value providing the document's
data]({{< ref "#supported-values-providing-document-data" >}}) calculated upon an item of the data collection by adding
a `doc` tag with an `inline` switch at a position within the fragment after the opening `foreach` tag where to insert
the document as per the example:
{{< highlight "c#" >}}
<<doc [dir + definitionFile] -inline>>
{{< /highlight >}}

{{% alert %}}

A `doc` tag cannot be used within textboxes and charts.

{{% /alert %}}

5. Add a closing `foreach` tag at the end of the fragment this way:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

6. Review your importing template before saving, it should look like this:\
\
<img src="document-inserting-with-content-inlining-template.png"
  alt="Document inserting with content inlining template for LINQ Reporting Engine in C#."
  style="width:372px"/>

7. Build your document using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "b4f7d42cdf0b5d6cddf159e7fbc1337f" "inserting-document-inlining-content.cs" >}}

## Document Inserting with Content Inlining Report Example

After taking all the steps, LINQ Reporting Engine creates an importing report as follows:\
\
<img src="document-inserting-with-content-inlining-report.png"
  alt="Document inserting with content inlining report created by LINQ Reporting Engine in C#."
  style="width:616px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Document%20Inserting%20with%20Content%20Inlining%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Document%20Inserting%20with%20Content%20Inlining%20Data.json)
from the example, and try to insert a document inlining content online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

{{% include "../../common/document-values.md" %}}

## See Also

- [Importing Content]({{< ref "../../importing-content/" >}})
- [Binding Collections]({{< ref "../../binding-data/binding-collections/" >}})
- [LINQ Reporting Engine]({{< ref "../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../common/footer.md" %}}