---
title: Overriding Text Color in C#
second_title: Aspose.Words for .NET
articleTitle: Overriding Text Color
linktitle: Overriding Text Color
description: "How to override text color using LINQ Reporting Engine in C#."
type: docs
weight: 20
url: /net/overriding-text-color/
---

Overriding text color provides precise visual control, allowing important data points to stand out against the default palette.
This capability enhances readability and directs the reader’s attention to critical information without altering the underlying
data. You can override text color using LINQ Reporting Engine in C#.

## How to Override Text Color

{{% alert %}}

This guide provides a shortcut method for applying only text colors to output text.

{{% /alert %}}

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include text-color-overriding-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a template document to data values that do not require text coloring by adding expression tags to
the template such as the following ones:
{{< highlight "c#" >}}
<<[projectId]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[projectName]>>
{{< /highlight >}}

3. Bind the text color of a text fragment to a [color value]({{< ref "#supported-color-values" >}}) by adding an opening
`textColor` tag to the beginning of the fragment like one of these:
{{< highlight "c#" >}}
<<textColor [projectHealth == "Healthy" ? "Green" : "Red"]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<textColor [budgetUtilization == "On Track" ? "Blue" : "Red"]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<textColor [completionPercentage > 50 ? "Green" : "Red"]>>
{{< /highlight >}}

{{% alert %}}

A color value can be directly stored in a data source, for example, as an object property.

{{% /alert %}}

4. Bind the text fragment to a data value by adding an expression tag to the fragment after the opening `textColor` tag, such
as:
{{< highlight "c#" >}}
<<[projectHealth]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[budgetUtilization]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[completionPercentage]>>
{{< /highlight >}}

5. Add a closing `textColor` tag at the end of the text fragment this way:
{{< highlight "c#" >}}
<</textColor>>
{{< /highlight >}}

{{% alert %}}

Such a text fragment may be multi-paragraph or even multi-section.

{{% /alert %}}

6. Review your text color overriding template before saving, it should look like this:\
\
<img src="text-color-overriding-template.png"
  alt="Text color overriding template for LINQ Reporting Engine in C#."
  style="width:455px"/>

7. Build your report overriding a text color using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "f8b950bfdf9a6341c86ddb5f8e8a7817" "overriding-text-color.cs" >}}

## Text Color Overriding Report Example

After taking all the steps, LINQ Reporting Engine creates a text color overriding report as follows:\
\
<img src="text-color-overriding-report.png"
  alt="Text color overriding report created by LINQ Reporting Engine in C#."
  style="width:172px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Text%20Color%20Overriding%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Text%20Color%20Overriding%20Data.json)
from the example, and try to override text color online for free by using one of
the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

{{% include "../../common/color-values.md" %}}

## See Also

- [Formatting Text]({{< ref "../../formatting-text/" >}})
- [LINQ Reporting Engine]({{< ref "../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../common/footer.md" %}}