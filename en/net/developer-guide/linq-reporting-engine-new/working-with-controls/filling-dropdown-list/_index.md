---
title: Filling Dropdown List in C#
second_title: Aspose.Words for .NET
articleTitle: Filling Dropdown List
linktitle: Filling Dropdown List
description: "How to fill a dropdown list using LINQ Reporting Engine in C#."
type: docs
weight: 20
url: /net/filling-dropdown-list/
---

Filling a [dropdown list](https://en.wikipedia.org/wiki/Drop-down_list) or [combobox](https://en.wikipedia.org/wiki/Combo_box)
is essential for data integrity and user efficiency. It restricts user input to pre-approved choices, which enforces data
standardization by ensuring users select only from a validated set of options, thereby preventing errors in input. You can fill
a dropdown list using LINQ Reporting Engine in C#.

## How to Fill a Dropdown List

{{% alert %}}

This guide highlights usage of `item` tags nested to `foreach` tags to fill a dropdown list upon a data collection. However,
a similar approach without `foreach` tags can be used for filling a dropdown list with a fixed number of items just by adding
as many `item` tags as needed.

{{% /alert %}}

1. Prepare data for your dropdown list in one of [formats supported by LINQ Reporting Engine]({{< ref "../../binding-data/" >}}),
for example, a JSON file as follows:
{{< highlight json >}}
{{< include dropdown-list-filling-data.json >}}
{{< /highlight >}}

2. In Microsoft Word, [create a dropdown list or combobox content
control](https://support.microsoft.com/en-us/office/create-a-form-in-word-that-users-can-complete-or-print-040c5cc1-e309-445b-94ac-542f732c8c8b)
and [set its
properties](https://support.microsoft.com/en-us/office/create-a-form-in-word-that-users-can-complete-or-print-040c5cc1-e309-445b-94ac-542f732c8c8b#__set_properties)
to use it as a template.

3. By editing the properties, remove the default dropdown list item, if not needed.

{{% alert %}}

You can modify the item instead or add more items to be present regardless of data used for filling the dropdown list.

{{% /alert %}}

4. Bind the dropdown list to a data collection by adding an opening `foreach` tag to the title of the dropdown list upon [editing
content control properties](https://support.microsoft.com/en-us/office/create-a-form-in-word-that-users-can-complete-or-print-040c5cc1-e309-445b-94ac-542f732c8c8b#__set_properties)
as per the example:
{{< highlight "c#" >}}
<<foreach [in items]>>
{{< /highlight >}}

5. Bind every dropdown list item to be added to an item of the data collection by adding an `item` tag after the opening
`foreach` tag and declaring values calculated upon the collection's item to define the value and display name of the dropdown
list item respectively, for instance, like so:
{{< highlight "c#" >}}
<<item [code] [region]>>
{{< /highlight >}}

{{% alert %}}

The value defining the display name can be omitted, then the dropdown list item's value is used as its display name as well.

{{% /alert %}}

6. Add a closing `foreach` tag after the `item` tag this way:
{{< highlight "c#" >}}
<</foreach>>
{{< /highlight >}}

7. Review your dropdown list template before saving, it should look like this:\
\
<img src="dropdown-list-filling-template.png"
  alt="Dropdown list filling template for LINQ Reporting Engine in C#."
  style="width:357px"/>

7. Build your dropdown list using LINQ Reporting Engine by running the following C# code:\
{{< gist "aspose-words-gists" "a66ce447ae59fc41f64f9e6b0d73e17f" "filling-dropdown-list.cs" >}}

## Dropdown List Filling Report Example

After taking all the steps, LINQ Reporting Engine creates a dropdown list report as follows:\
\
<img src="dropdown-list-filling-report.png"
  alt="Dropdown list filling report created by LINQ Reporting Engine in C#."
  style="width:164px"/>

{{% alert %}}

You can download the [template
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Dropdown%20List%20Filling%20Template.docx)
and [data
](https://github.com/aspose-words/Aspose.Words-for-.NET/raw/ivan.lyagin/UEX-331/Examples/Data/LINQ/Dropdown%20List%20Filling%20Data.json)
from the example, and try to fill a dropdown list online for free by using one of the options:\
<a class="product-item docs-btn" href="https://products.aspose.app/words/assembly" >APP </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/net/report/" >.NET API </a>
<a class="product-item docs-btn" href="https://products.aspose.com/words/python-net/report/" >
PYTHON via <em class="docs-vianet">net</em> API</a>
<br/>
<br/>

{{% /alert %}}

## See Also

- [Working with Controls]({{< ref "../../working-with-controls/" >}})
- [Binding Collections]({{< ref "../../binding-data/binding-collections/" >}})
- [LINQ Reporting Engine]({{< ref "../../../linq-reporting-engine-new/" >}})
- [ReportingEngine Class](https://reference.aspose.com/words/net/aspose.words.reporting/reportingengine/)

{{% include "../../common/footer.md" %}}