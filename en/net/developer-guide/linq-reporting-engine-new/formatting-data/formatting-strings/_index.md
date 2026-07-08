---
title: Formatting Strings in C#
second_title: Aspose.Words for .NET
articleTitle: Formatting Strings
linktitle: Formatting Strings
description: "How to format strings using LINQ Reporting Engine in C#."
type: docs
weight: 30
url: /net/formatting-strings/
---

Applying string formatting transforms raw textual data into a standardized structure by automatically modifying case styles.
This process establishes complete consistency across all final documents, ensuring that text-based expressions appear polished
and professional. You can format strings using LINQ Reporting Engine in C#.

## How to Format Strings

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include strings-formatting-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a template document to values and apply string formatting as per your requirements by adding
expression tags to the template such as the following ones:

    * To convert a string to lower case, apply the `lower` format specifier, for example:
{{< highlight "c#" >}}
<<[customerEmailAddress]:lower>>
{{< /highlight >}}

    * To convert a string to upper case, apply the `upper` format specifier, like that:
{{< highlight "c#" >}}
<<[internationalStandardBankingCode]:upper>>
{{< /highlight >}}

    * To capitalize the first letter of every word, apply the `caps` format specifier, as shown:
{{< highlight "c#" >}}
<<[employeeJobTitle]:caps>>
{{< /highlight >}}

    * To capitalize the first letter of the first word only, apply the `firstCap` format specifier, like so:
{{< highlight "c#" >}}
<<[projectStatusDescription]:firstCap>>
{{< /highlight >}}

    * To combine [numeric]({{< ref "../formatting-numbers/" >}}) and string formats, chain the format specifiers, for example:
{{< highlight "c#" >}}
<<[contractNoticePeriodMonths]:cardinal:lower>>
{{< /highlight >}}

    * To combine [date-time]({{< ref "../formatting-date-and-time/" >}}) and string formats, chain the format specifiers, for
instance:
{{< highlight "c#" >}}
<<[fiscalQuarterEndDateTime]:"MMMM d":upper>>
{{< /highlight >}}

{{% alert %}}
For standard and custom .NET format strings, enclose the format pattern in double quotes (`"…"`) after the colon. The custom
string format identifiers (`lower`, `upper`, `caps`, `firstCap`) as well as [numeric ones]({{< ref "../formatting-numbers/" >}})
are specific to LINQ Reporting Engine and do not require quotes.
{{% /alert %}}

3. Review your strings formatting template before saving, it should look like this:\
\
<img src="strings-formatting-template.png"
  alt="Strings formatting template for LINQ Reporting Engine in C#."
  style="width:312px"/>

4. Build your report formatting strings using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "26a14ab1f3e2d3ff91d9f1ce4397a2b0" "formatting-strings.cs" >}}

## Strings Formatting Report Example

After taking all the steps, LINQ Reporting Engine creates a strings formatting report as follows:\
\
<img src="strings-formatting-report.png"
  alt="Strings formatting report created by LINQ Reporting Engine in C#."
  style="width:239px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Strings%20Formatting%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Strings%20Formatting%20Data.json)
from the example, and try to format strings online for free by using one of
the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## See Also

- [Formatting Data]({{< ref "../../formatting-data/" >}})
- [LINQ Reporting Engine]({{< ref "../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../common/footer.md" %}}