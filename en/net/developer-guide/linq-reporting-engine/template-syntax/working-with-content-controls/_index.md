---
title: Working with Content Controls in C#
second_title: Aspose.Words for .NET
articleTitle: Working with Content Controls
linktitle: Working with Content Controls
description: "Perform certain operations on content controls dynamically while building a report using C#."
type: docs
weight: 83
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/working-with-content-controls/
aliases: [/net/template-syntax/#working-with-content-controls]
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page explains how to work with content controls conceptually and programmatically.

{{% /alert %}}

LINQ Reporting Engine enables you to perform certain operations on content controls dynamically while building a report.

**Note** – To work with content controls in template documents using Microsoft Word®, you may need to [show the Developer tab on its ribbon](https://docs.microsoft.com/en-us/visualstudio/vsto/how-to-show-the-developer-tab-on-the-ribbon?view=vs-2022).

## Setting Checkbox Values Dynamically

You can set checkbox values to either checked or unchecked in your reports dynamically by taking the following steps:

1. Add a checkbox content control to your template at a place where you want it to appear in a result document.
1. By editing content control properties, add a `check` tag to the title of the checkbox content control using the following syntax.

{{< highlight csharp >}}
<<check [conditional_expression]>>
{{< /highlight >}}

Here, `conditional_expression` defines a condition upon which the value of the checkbox content control is to be set to checked (or unchecked, if the condition is not met). The conditional expression must return a `Boolean` value.

While building a report, a conditional expression declared within a `check` tag is evaluated and the value of its containing checkbox content control is set accordingly. The `check` tag itself is removed then.

## Adding Combobox and Dropdown List Items Dynamically

You can dynamically add items to comboboxes and dropdown lists defined in your template by taking the following steps:

1. Add a combobox or dropdown list content control to your template at a place where you want it to appear in a result document.
2. By editing content control properties, add an item tag to the title of this content control using the following syntax.

{{< highlight csharp >}}
<<item [value_expression] [display_name_expression]>>
{{< /highlight >}}

Here, `value_expression` defines a value of a combobox or dropdown list item to be added dynamically. This expression is mandatory and must return a non‑empty value.

In turn, `display_name_expression` defines a display name of the combobox or dropdown list item to be added. This expression is optional. If it is omitted, then during runtime, a value of `value_expression` is used as a display name as well.

**Note** – Values of both `value_expression` and `display_name_expression` can be of any types. During runtime, `Object.ToString()` is invoked to get textual representations of these expressions’ values.

While building a report, `value_expression` and `display_name_expression` are evaluated and a corresponding combobox or dropdown list item is added. A declaring item tag is removed then.

A single `item` tag causes addition of a single combobox or dropdown list item during runtime. You can add multiple combobox or dropdown list items using multiple `item` tags as shown in the following snippet.

{{< highlight csharp >}}
<<item ...>><<item ...>>
{{< /highlight >}}

Also, you can normally use `item` tags within data bands to add a combobox or dropdown list item per item of a data collection. For example, given that `clients` is a `DataTable` instance having a field named “Name”, you can use the following template to cover such a scenario.

{{< highlight csharp >}}
<<foreach [client in clients]>><<item [client.Name]>><</foreach>>
{{< /highlight >}}

An `item` tag can also be combined with an `if` tag to add a combobox or dropdown list item depending on a condition as shown in the following snippet.

{{< highlight csharp >}}
<<if ...>><<item ...>><</if>>
{{< /highlight >}}

Existing combobox and dropdown list items are not affected by `item` tags. Thus, you can combine both ways of adding combobox and dropdown list items using a template: static and dynamic.

**Note** – While inserting a combobox or dropdown list, Microsoft Word adds a default item that has to be removed manually, if the item is unwanted.

## Setting Content Control Titles Dynamically

You can normally use common expression tags in content control titles, thus forming their contents dynamically. For example, given that `s` is a string value, you can set a content control title from this value dynamically by putting the following expression tag into the title.

{{< highlight csharp >}}
<<[s]>>
{{< /highlight >}}

------ 

## FAQ

1. **Q:** How do I make a checkbox content control checked or unchecked based on data?  
   **A:** Add a `check` tag to the checkbox title using the syntax `<<check [conditional_expression]>>`. The expression must return a Boolean value; if true, the checkbox is checked, otherwise it remains unchecked. The `check` tag is removed automatically after evaluation.

2. **Q:** What is the correct way to add items to a combobox or dropdown list at runtime?  
   **A:** Use the `item` tag inside the content control title: `<<item [value_expression] [display_name_expression]>>`. The first argument supplies the item value (required), and the optional second argument supplies the display text. Multiple `item` tags can be placed sequentially or generated inside a `foreach` loop.

3. **Q:** Can I conditionally add a combobox item only when a certain condition is met?  
   **A:** Yes. Wrap the `item` tag inside an `if` tag, e.g., `<<if [condition]>> <<item [value]>> <</if>>`. The `item` will be added only if the condition evaluates to true.

4. **Q:** Why does a default item appear in a newly inserted dropdown list, and how can I remove it?  
   **A:** Microsoft Word automatically inserts a placeholder item when a dropdown list is created. This item is not removed by Aspose.Words, so you must delete it manually in the template or programmatically after the document is generated.

5. **Q:** How can I set the title of a content control dynamically using a variable?  
   **A:** Place an expression tag inside the title, such as `<<[myVariable]>>`. During report generation the variable’s `ToString()` value replaces the tag, producing a dynamic title. This works for any content control type.