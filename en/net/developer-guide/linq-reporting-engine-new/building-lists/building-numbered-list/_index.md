---
title: Building Numbered List in C#
second_title: Aspose.Words for .NET
articleTitle: Building Numbered List
linktitle: Building Numbered List
description: "How to make a numbered list using LINQ Reporting Engine in C#."
type: docs
weight: 20
url: /net/building-numbered-list/
---

[Numbered lists](https://en.wikipedia.org/wiki/Collation#Labeling_of_ordered_items) are useful for presenting sequential
information, such as step-by-step instructions, a timeline of events, or a hierarchy of points. They provide clear, logical
structure that helps the reader follow the precise order of information, ensuring processes are understood and executed
correctly. You can make a numbered list using LINQ Reporting Engine in C#.

## How to Build a Numbered List

1. Prepare data for your list in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include numbered-list-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a numbered
list](https://support.microsoft.com/en-us/office/create-a-numbered-or-numbered-list-9ff81241-58a8-4d88-8d8c-acab3006a23e)
with a single empty paragraph and [format the
list](https://support.microsoft.com/en-us/office/change-the-color-size-or-format-of-bullets-or-numbers-in-a-list-in-word-005b7248-75e4-465e-85cc-9f768af03836)
to use it as a template.

3. Bind the paragraph to a data collection to repeat the paragraph for every item of the collection by adding an opening
`foreach` tag to the beginning of the paragraph as per the example:
{{< highlight "c#" >}}
<<foreach [in items]>>
{{< /highlight >}}

4. Bind the paragraph to values calculated upon an item of the data collection by adding expression tags after the opening
`foreach` tag such as the following one:
{{< highlight "c#" >}}
<<[product]>>
{{< /highlight >}}

5. Right after the paragraph, add one more paragraph without a numbered list and put a closing `foreach` tag into the new
paragraph like so:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

6. Review your list template before saving, it should look like this:\
\
<img src="numbered-list-template.png"
  alt="Numbered list template for LINQ Reporting Engine in C#."
  style="width:284px"/>

7. Build your list using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "dba46de6f9697ecd608b15bc14a152a7" "building-numbered-list.cs" >}}

## Numbered List Report Example

After taking all the steps, LINQ Reporting Engine creates a list report as follows:\
\
<img src="numbered-list-report.png"
  alt="Numbered list report created by LINQ Reporting Engine in C#."
  style="width:284px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Numbered%20List%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Numbered%20List%20Data.json)
from the example, and try to make a numbered list online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## See Also

- [Building Lists]({{< ref "../../building-lists/" >}})
- [Binding Collections]({{< ref "../../binding-data/binding-collections/" >}})
- [LINQ Reporting Engine]({{< ref "../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../common/footer.md" %}}