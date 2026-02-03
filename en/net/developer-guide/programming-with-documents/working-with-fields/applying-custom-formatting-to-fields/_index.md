---
title: Apply Custom Formatting to Fields in C#
second_title: Aspose.Words for .NET
articleTitle: Apply Custom Formatting to Fields
linktitle: Apply Custom Formatting to Fields
description: "Format and evaluate fields result using C#."
type: docs
weight: 40
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/applying-custom-formatting-to-fields/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page outlines how to apply custom formatting to fields (like merge fields or document variables) in Aspose.Words.

{{% /alert %}}

Sometimes users need to apply custom formatting to fields. In this article, we will look at a couple of examples of how this can be done.

To learn more options, see the full list of properties for each field type in the corresponding class in the [Fields namespace](https://reference.aspose.com/words/net/aspose.words.fields/).

## How to Apply Custom Formatting to Field Result

Aspose.Words provides API for custom formatting of field's result. You can implement [IFieldResultFormatter](https://reference.aspose.com/words/net/aspose.words.fields/ifieldresultformatter/) interface to control how the field result is formatted. You can apply numeric format switch, i.e. \# "#.##", date/time format switch, i.e. \@ "dd.MM.yyyy", and number format switch, i.e. \* Ordinal.

The following code example shows how to apply custom formatting for the field result:

{{< gist "aspose-words-gists" "79b46682fbfd7f02f64783b163ed95fc" "field-result-formatting.cs" >}}

{{< gist "aspose-words-gists" "79b46682fbfd7f02f64783b163ed95fc" "field-result-formatter.cs" >}}

## How to evaluate `IF` condition

If you want to evaluate `IF` condition after mail merge, you can use the [EvaluateCondition](https://reference.aspose.com/words/net/aspose.words.fields/fieldif/evaluatecondition/) method that immediately returns the result of the expression evaluation.

The following code example shows how to use this method:

{{< gist "aspose-words-gists" "79b46682fbfd7f02f64783b163ed95fc" "evaluate-if-condition.cs" >}}

## How to Apply Custom Formatting to Time Field

By default Aspose.Words updates `TIME` field with current culture short time format. We figured out that there is a difference between Microsoft Word formatting and .NET/Windows formatting, and also between different .NET Framework versions. If you want to format the `TIME` field according to your requirement, you can achieve this by implementing [IFieldUpdateCultureProvider](https://reference.aspose.com/words/net/aspose.words.fields/ifieldupdatecultureprovider/) interface.

The following code examples shows how to apply custom formatting to the `TIME` field:

{{< gist "aspose-words-gists" "79b46682fbfd7f02f64783b163ed95fc" "field-update-culture.cs" >}}

{{< gist "aspose-words-gists" "79b46682fbfd7f02f64783b163ed95fc" "field-update-culture-provider.cs" >}}

------  

## FAQ
1. **Q:** How can I apply a numeric format (e.g., two decimal places) to a merge field result?  
   **A:** Implement the `IFieldResultFormatter` interface and, in the `FormatResult` method, apply a numeric format string such as `"#.00"` to the field value. Register the formatter with `Document.FieldOptions.ResultFormatter` before updating the fields.

2. **Q:** What is the easiest way to format a date field with a custom pattern like `dd.MM.yyyy`?  
   **A:** Use a field result formatter and apply the date format switch (`\@ "dd.MM.yyyy"`). Inside `FormatResult`, check if the field type is `FieldDate` and return `DateTime.Parse(value).ToString("dd.MM.yyyy")`.

3. **Q:** How do I evaluate an `IF` field condition programmatically after a mail‑merge operation?  
   **A:** Call `FieldIf.EvaluateCondition(string condition)` which returns a `bool` indicating the result. This method does not require the field to be inserted into the document; you can pass the condition string directly.

4. **Q:** The `TIME` field shows a different format than I expect on my server. How can I control its output?  
   **A:** Implement `IFieldUpdateCultureProvider` and return a `CultureInfo` that matches the desired time format. Assign your provider to `Document.FieldOptions.UpdateCultureProvider` before calling `Field.Update()`.

5. **Q:** Can I combine multiple format switches (numeric, ordinal, date) for a single field?  
   **A:** Yes. In your `IFieldResultFormatter` implementation you can inspect the field code for switches such as `\#`, `\@`, and `\*`. Apply each switch sequentially to the raw field value to produce the final formatted result.  