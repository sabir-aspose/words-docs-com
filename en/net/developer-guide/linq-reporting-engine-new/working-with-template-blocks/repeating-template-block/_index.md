---
title: Repeating Template Block in C#
second_title: Aspose.Words for .NET
articleTitle: Repeating Template Block
linktitle: Repeating Template Block
description: "How to repeat a template block using LINQ Reporting Engine in C#."
type: docs
weight: 10
url: /net/repeating-template-block/
---

Repeating a template block allows a defined section of a report to be reproduced automatically for each item of a data
collection, preserving layout and calculations uniformly. This capability eliminates the need to recreate the same design
repeatedly and ensures that any modification to the block is reflected instantly throughout the entire report. You can repeat a
template block using LINQ Reporting Engine in C#.

## How to Repeat a Template Block

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include template-block-repeating-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a template block to a data collection by adding an opening `foreach` tag to the beginning of the
block as per the example:  
{{< highlight "c#" >}}
<<foreach [in items]>>
{{< /highlight >}}

3. Add a closing `foreach` tag to the end of the template block like that:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

4. Bind the template block to values calculated upon an item of the data collection by adding expression tags to the block
between the opening and closing `foreach` tags such as the following ones:
{{< highlight "c#" >}}
<<[topic]>>
{{< /highlight >}}
{{< highlight "c#" >}}
<<[status]>>
{{< /highlight >}}

5. Review your template block repeating template before saving, it should look like this:\
\
<img src="template-block-repeating-template.png"
  alt="Template block repeating template for LINQ Reporting Engine in C#."
  style="width:212px"/>

6. Build your report repeating a template block using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "e70be26e4fe5bd75b41246169be155e1" "repeating-template-block.cs" >}}

## Template Block Repeating Report Example

After taking all the steps, LINQ Reporting Engine creates a template block repeating report as follows:\
\
<img src="template-block-repeating-report.png"
  alt="Template block repeating report created by LINQ Reporting Engine in C#."
  style="width:212px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Template%20Block%20Repeating%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Template%20Block%20Repeating%20Data.json)
from the example, and try to repeat a template block online for free by using one of
the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## How to Repeat Master-Detail Template Blocks

1. Prepare data for your report in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include master-detail-template-blocks-repeating-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, bind a master template block to a master data collection by adding an opening `foreach` tag to the
beginning of the block as per the example:
{{< highlight \"c#\" >}}
<<foreach [in items]>>
{{< /highlight >}}

3. Add a closing `foreach` tag to the end of the block like so:
{{< highlight \"c#\" >}}
<</foreach>>
{{< /highlight >}}

4. Bind the master block to values calculated upon an item of the master collection by adding expression tags between the
opening and closing `foreach` tags such as:
{{< highlight \"c#\" >}}
<<[department]>>
{{< /highlight >}}

5. Bind a detail template block to a detail data collection calculated upon an item of the master data collection by adding an
inner opening `foreach` tag to the beginning of the detail block between the outer opening and closing `foreach` tags as per the
example:
{{< highlight \"c#\" >}}
<<foreach [in milestones]>>
{{< /highlight >}}

6. Add an inner closing `foreach` tag to the end of the detail block between the outer opening and closing `foreach` tags like
that:
{{< highlight \"c#\" >}}
<</foreach>>
{{< /highlight >}}

7. Bind the detail block to values calculated upon an item of the detail collection by adding expression tags between the inner
opening and closing `foreach` tags such as:
{{< highlight \"c#\" >}}
<<[result]>>
{{< /highlight >}}

8. Review your master-detail template blocks repeating template before saving, it should look like this:\
\
<img src="master-detail-template-blocks-repeating-template.png"
  alt="Master-detail template blocks repeating template for LINQ Reporting Engine in C#."
  style="width:324px"/>

9. Build your report repeating master-detail template blocks using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "f39276b10a7343ba52a481410655ef91" "repeating-master-detail-template-blocks.cs" >}}

## Master-Detail Template Blocks Repeating Report Example

After taking all the steps, LINQ Reporting Engine creates a master-detail template blocks repeating report as follows:\
\
<img src="master-detail-template-blocks-repeating-report.png"
  alt="Master-detail template blocks repeating report created by LINQ Reporting Engine in C#."
  style="width:538px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Master-Detail%20Template%20Blocks%20Repeating%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Master-Detail%20Template%20Blocks%20Repeating%20Data.json)
from the example, and try to repeat master-detail template blocks online for free by using one of
the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## See Also

- [Working with Template Blocks]({{< ref "../../working-with-template-blocks/" >}})
- [Binding Collections]({{< ref "../../binding-data/binding-collections/" >}})
- [LINQ Reporting Engine]({{< ref "../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../common/footer.md" %}}