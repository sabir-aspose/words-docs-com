---
title: Inserting Sub-template in C#
second_title: Aspose.Words for .NET
articleTitle: Inserting Sub-template
linktitle: Inserting Sub-template
description: "How to insert a sub-template using LINQ Reporting Engine in C#."
type: docs
weight: 20
url: /net/inserting-sub-template/
---

Inserting [sub-templates](https://en.wiktionary.org/wiki/subtemplate) allows users to reuse standardized blocks and layouts,
such as consistent headers, footers, or complex calculations, across multiple reports without manual recreation. This modular
approach ensures report-wide consistency and enables global updates by modifying a single source file rather than editing every
individual layout. You can insert a sub-template using LINQ Reporting Engine in C#.

## How to Insert a Sub-template

{{% alert %}}

* Inserting a sub-template is a special case of [inserting a document]({{< ref "../inserting-document/" >}}), so all the options
available for document insertion can be applied to sub-template insertion as well.

* Although the guide focuses on usage of `doc` tags with `build` switches nested to `foreach` tags, a similar approach can be
used with no `foreach` tags involved.

{{% /alert %}}

1. Prepare data for your template and sub-template in one of [formats supported by LINQ Reporting
Engine]({{< ref "../../binding-data/" >}}), for example, a JSON file as follows:
{{< highlight json >}}
{{< include sub-template-inserting-data.json >}}
{{< /highlight >}}

{{% alert %}}

In this example, the additional data source `dir` - the path to a directory of a sub-template to be inserted - is used.

{{% /alert %}}

2. In Microsoft Word, create a template document and bind a fragment of its text to a data collection to repeat the fragment
for every item of the collection by adding an opening `foreach` tag to the beginning of the fragment, for instance, like so:
{{< highlight "c#" >}}
<<foreach [in items]>>
{{< /highlight >}}

3. In Microsoft Word, create one more standalone document to use it as a sub-template accessing an item of the data collection
by taking the following steps:

    * Define necessary calculations upon an item of the collection using [variables
]({{< ref "../../binding-data/working-with-variables/" >}}) for intermediate results by adding `var` tags to the sub-template
similar to these:
{{< highlight "c#" >}}
<<var [bonus = totalSales > 100000 ? (totalSales - 100000) * 0.15 + 7500 :
               totalSales > 50000 ? (totalSales - 50000) * 0.10 + 2500 :
               totalSales * 0.05]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<var [bonus = bonus + totalSales * (productCategory == "Technology" ? 0.02 : 0)]>>
{{< /highlight >}}

    * Bind the sub-template to values calculated upon an item of the collection and the variables by adding expression tags
after the `var` tags such as the following ones:
{{< highlight "c#" >}}
<<[salesPerson]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[bonus]>>
{{< /highlight >}}

    * Review your sub-template before saving, it should look like that:\
\
<img src="salesperson-bonuses-sub-template.png"
  alt="Sub-template for LINQ Reporting Engine in C#."
  style="width:501px"/>

{{% alert %}}

A sub-template can access the following data available at a position within a template where the sub-template is inserted:
* Data sources
* [Variables]({{< ref "../../binding-data/working-with-variables/" >}})
* [A contextual object]({{< ref "../../binding-data/shorthanding-object-member-references/" >}})
* [Known external types]({{< ref "../../binding-data/running-custom-code/" >}})

{{% /alert %}}

4. Getting back to editing the template, bind the source of a sub-template to be inserted to a [value providing the document's
data]({{< ref "#supported-values-providing-document-data" >}}) by adding a `doc` tag with a `build` switch at a position
within the template's fragment after the opening `foreach` tag where to insert the sub-template as per the example:
{{< highlight "c#" >}}
<<doc [dir + ds.subTemplateFile] -build>>
{{< /highlight >}}

{{% alert %}}

* Since between opening and closing `foreach` tags, expressions are evaluated upon an item of a corresponding data collection,
it is required to explicitly specify the name of a data source - such as `ds` - here, in order to reference the same
sub-template for all items of the collection.

* A `doc` tag cannot be used within textboxes and charts.

{{% /alert %}}

5. Add a closing `foreach` tag at the end of the fragment this way:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

6. Review your importing template before saving, it should look like this:\
\
<img src="sub-template-inserting-template.png"
  alt="Sub-template inserting template for LINQ Reporting Engine in C#."
  style="width:245px"/>

7. Build your document using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "163634c0cc5926a3a5fd4e9b74594641" "inserting-sub-template.cs" >}}

## Sub-template Inserting Report Example

After taking all the steps, LINQ Reporting Engine creates an importing report as follows:\
\
<img src="sub-template-inserting-report.png"
  alt="Sub-template inserting report created by LINQ Reporting Engine in C#."
  style="width:224px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Sub-template%20Inserting%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Sub-template%20Inserting%20Data.json)
from the example, and try to insert a sub-template online for free by using one of the options:\
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