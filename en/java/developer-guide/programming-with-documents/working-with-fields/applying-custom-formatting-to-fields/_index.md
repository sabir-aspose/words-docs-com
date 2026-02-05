---
title: Apply Custom Formatting to Fields
second_title: Aspose.Words for Java
articleTitle: Apply Custom Formatting to Fields
linktitle: Apply Custom Formatting to Fields
description: "Format and evaluate fields result using Java."
type: docs
weight: 40
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /java/applying-custom-formatting-to-fields/
timestamp: 2024-01-27-14-07-04
---

Sometimes users need to apply custom formatting to fields. In this article, we will look at a couple of examples of how this can be done.

To learn more options, see the full list of properties for each field type in the corresponding class.

## How to Apply Custom Formatting to Field Result

Aspose.Words provides API for custom formatting of field's result. You can implement [IFieldResultFormatter](https://reference.aspose.com/words/java/com.aspose.words/ifieldresultformatter/) interface to control how the field result is formatted. You can apply numeric format switch, i.e. \# "#.##", date/time format switch, i.e. \@ "dd.MM.yyyy", and number format switch, i.e. \* Ordinal.

The following code example shows how to apply custom formatting for the field result.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-fields-FormatFieldResult-FormatFieldResult.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-fields-FieldResultFormatter-FieldResultFormatter.java" >}}

## How to evaluate `IF` condition

If you want to evaluate `IF` condition after mail merge, you can use the [EvaluateCondition](https://reference.aspose.com/words/java/com.aspose.words/fieldif/#evaluateCondition) method that immediately returns the result of the expression evaluation.

The following code example shows how to use this method:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-fields-EvaluateIFCondition-EvaluateIFCondition.java" >}}

## How to Apply Custom Formatting to Time Field

By default Aspose.Words updates `TIME` field with current culture short time format. If you want to format the `TIME` field according to your requirement, you can achieve this by implementing [IFieldUpdateCultureProvider](https://reference.aspose.com/words/java/com.aspose.words/ifieldupdatecultureprovider/) interface.

The following code examples shows how to apply custom formatting to the `TIME` field:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-fields-FieldUpdateCulture-FieldUpdateCulture.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-fields-FieldUpdateCultureProvider-FieldUpdateCultureProvider.java" >}}

------ 

## FAQ

1. **Q:** How can I format a date field with a custom pattern?  
   **A:** Implement `IFieldResultFormatter` and return the formatted string using `SimpleDateFormat`. In the `formatResult` method, detect the field type (e.g., `FieldDate`) and apply the desired pattern such as `"dd.MM.yyyy"`.

2. **Q:** What switch should I use to apply a numeric format to a field result?  
   **A:** Use the numeric format switch `\# "#.##"` (or any valid .NET/Java numeric format string) inside the field code. The custom formatter can also apply this switch programmatically.

3. **Q:** How do I evaluate an `IF` field after performing a mail merge?  
   **A:** Call `FieldIf.evaluateCondition()` on the `FieldIf` object. This method returns a boolean indicating the result of the expression without needing to update the whole document.

4. **Q:** How can I change the culture used by the `TIME` field?  
   **A:** Implement `IFieldUpdateCultureProvider` and return a `CultureInfo` that matches your required time format. Register the provider with `Document.updateFields()` or set it on the specific `FieldTime` instance.

5. **Q:** Is it possible to apply an ordinal number format (e.g., 1st, 2nd) to a field?  
   **A:** Yes. Use the number format switch `\* Ordinal` in the field code, or return the ordinal string from your `IFieldResultFormatter` implementation for the field’s result.