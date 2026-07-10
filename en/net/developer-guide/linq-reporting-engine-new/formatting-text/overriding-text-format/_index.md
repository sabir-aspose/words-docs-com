---
title: Overriding Text Format in C#
second_title: Aspose.Words for .NET
articleTitle: Overriding Text Format
linktitle: Overriding Text Format
description: "How to override text format using LINQ Reporting Engine in C#."
type: docs
weight: 10
url: /net/overriding-text-format/
---

Overriding text format enables custom styling of any textual element, allowing the report to use specific fonts, sizes, colors,
or alignments that reflect the desired visual identity. This targeted formatting highlights key information and supports
conditional presentation based on data values. You can override text format using LINQ Reporting Engine in C#.

## How to Format Output Text

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include output-text-formatting-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a template document to data values by adding expression tags to the template such as the following
ones:
{{< highlight "c#" >}}
<<[kpiName]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[actualRevenue]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[targetRevenue]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[variancePct]>>
{{< /highlight >}}

3. Select text of an added expession tag and [apply text formatting to
it](https://support.microsoft.com/en-us/word/training/add-and-edit-text) depending on your requirements. The expression result
will derive this formatting in an output report.

4. Review your output text formatting template before saving, it should look like this:\
\
<img src="output-text-formatting-template.png"
  alt="Output text formatting template for LINQ Reporting Engine in C#."
  style="width:229px"/>

5. Build your report formatting output text using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "5040f3ac1771dc3d0ffc1251c6f6023d" "formatting-output-text.cs" >}}

## Output Text Formatting Report Example

After taking all the steps, LINQ Reporting Engine creates an output text formatting report as follows:\
\
<img src="output-text-formatting-report.png"
  alt="Output text formatting report created by LINQ Reporting Engine in C#."
  style="width:166px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Output%20Text%20Formatting%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Output%20Text%20Formatting%20Data.json)
from the example, and try to format output text online for free by using one of
the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Override Text Format

{{% alert %}}

This guide walks through overriding text format dynamically by basic usage of HTML. LINQ Reporting Engine also provides
[advanced options for HTML insertion]({{< ref "../../importing-content/inserting-html/" >}}).

{{% /alert %}}

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include text-format-overriding-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a template document to data values that do not require dynamic text format overriding by adding
expression tags to the template like this one:
{{< highlight "c#" >}}
<<[employeeName]>>
{{< /highlight >}}

3. Bind the template document to HTML-string values to override text format dynamically by adding expression tags with `html`
switches such as the following ones:
{{< highlight "c#" >}}
<<[quarterlyGoal] -html>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[achievedCount] -html>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[bonusEarned] -html>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[recognitionStatus] -html>>
{{< /highlight >}}

{{% alert %}}

* For this example, data values are preformatted with HTML tags. However, you can inject HTML tags directly into string
expressions instead, for instance, like so: `<<["<b>" + employeeName + "</b>"] -html>>`.

* An expression tag with an `html` switch cannot be used within charts.

{{% /alert %}}

4. Review your text format overriding template before saving, it should look like this:\
\
<img src="text-format-overriding-template.png"
  alt="Text format overriding template for LINQ Reporting Engine in C#."
  style="width:296px"/>

5. Build your report overriding a text format using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "ab271894904559b5c4dd351d662d04a1" "overriding-text-format.cs" >}}

## Text Format Overriding Report Example

After taking all the steps, LINQ Reporting Engine creates a text format overriding report as follows:\
\
<img src="text-format-overriding-report.png"
  alt="Text format overriding report created by LINQ Reporting Engine in C#."
  style="width:204px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Text%20Format%20Overriding%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Text%20Format%20Overriding%20Data.json)
from the example, and try to override text format online for free by using one of
the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## See Also

- [Formatting Text]({{< ref "../../formatting-text/" >}})
- [LINQ Reporting Engine]({{< ref "../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../common/footer.md" %}}