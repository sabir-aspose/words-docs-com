---
title: Formatting Numbers in C#
second_title: Aspose.Words for .NET
articleTitle: Formatting Numbers
linktitle: Formatting Numbers
description: "How to format numbers using LINQ Reporting Engine in C#."
type: docs
weight: 10
url: /net/formatting-numbers/
---

Formatting numbers ensures that all numeric data appear consistently, with appropriate decimal places, thousand separators, and
currency symbols, which enhances readability and professional appearance of the report. The feature can be applied to any
numeric expression, allowing the author to present calculations, totals, and key performance indicators in a way that aligns
with the intended audience’s expectations. You can format numbers using LINQ Reporting Engine in C#.

## How to Format Numbers

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include numbers-formatting-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a template document to numeric values and apply number formatting as per your requirements by adding
expression tags to the template such as the following ones:

    * To format a number using a standard .NET format, use [a standard numeric format
string](https://learn.microsoft.com/en-us/dotnet/standard/base-types/standard-numeric-format-strings) like so:
{{< highlight "c#" >}}
<<[productUnitCost]:"F">>
{{< /highlight >}}

    * To format a number using a custom .NET format, use [a custom numeric format
string](https://learn.microsoft.com/en-us/dotnet/standard/base-types/custom-numeric-format-strings) like this:
{{< highlight "c#" >}}
<<[quarterlyGdpGrowthRate]:"0.##">>
{{< /highlight >}}

    * To represent an integer as an upper-case letter (A, B, C, …) apply the `alphabetic` format specifier, for example:
{{< highlight "c#" >}}
<<[appendixIdentifier]:alphabetic>>
{{< /highlight >}}

    * To represent an integer as an upper-case Roman numeral (I, II, III, …) apply the `roman` format specifier, like that:
{{< highlight "c#" >}}
<<[corporateTierLevel]:roman>>
{{< /highlight >}}

    * To represent an integer with an ordinal suffix (1st, 2nd, 3rd, …) use the `ordinal` format specifier, for instance:
{{< highlight "c#" >}}
<<[quarterlyPerformanceRank]:ordinal>>
{{< /highlight >}}

    * To represent an integer as ordinal text (First, Second, Third, …) use the `ordinalText` format specifier, as shown:
{{< highlight "c#" >}}
<<[annualPriorityStage]:ordinalText>>
{{< /highlight >}}

    * To represent an integer as cardinal text (One, Two, Three, …) use the `cardinal` format specifier, like so:
{{< highlight "c#" >}}
<<[totalBoardMembersPresent]:cardinal>>
{{< /highlight >}}

    * To represent an integer as hexadecimal (8, 9, A, B, C, D, E, F, 10, …) use the `hex` format specifier, for example:
{{< highlight "c#" >}}
<<[systemErrorCode]:hex>>
{{< /highlight >}}

    * To enclose an integer with dashes (- 1 -, - 2 -, - 3 -, …) use the `arabicDash` format specifier, like this:
{{< highlight "c#" >}}
<<[documentPageNumber]:arabicDash>>
{{< /highlight >}}

    * To express a number as text with the fraction shown as Arabic numerators over 100, use the `dollarText` format specifier,
for instance:
{{< highlight "c#" >}}
<<[checkPaymentLegalAmount]:dollarText>>
{{< /highlight >}}

{{% alert %}}
For the standard and custom .NET format strings, enclose the format pattern in double quotes (`"…"`) after the colon. The custom
format identifiers (`alphabetic`, `roman`, `ordinal`, `ordinalText`, `cardinal`, `hex`, `arabicDash`, `dollarText`) are specific
to LINQ Reporting Engine and do not require quotes.
{{% /alert %}}

3. Review your numbers formatting template before saving, it should look like this:\
\
<img src="numbers-formatting-template.png"
  alt="Numbers formatting template for LINQ Reporting Engine in C#."
  style="width:387px"/>

4. Build your report formatting numbers using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "92769e3332e3f110bd2cc6e0d379b5c3" "formatting-numbers.cs" >}}

## Numbers Formatting Report Example

After taking all the steps, LINQ Reporting Engine creates a numbers formatting report as follows:\
\
<img src="numbers-formatting-report.png"
  alt="Numbers formatting report created by LINQ Reporting Engine in C#."
  style="width:387px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Numbers%20Formatting%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Numbers%20Formatting%20Data.json)
from the example, and try to format numbers online for free by using one of
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