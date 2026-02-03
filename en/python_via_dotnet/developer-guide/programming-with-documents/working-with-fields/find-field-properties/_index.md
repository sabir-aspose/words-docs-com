---
title: Find Field Properties in Python
second_title: Aspose.Words for Python via .NET
articleTitle: Find Field Properties
linktitle: Find Field Properties
description: "How to find some field properties like field code and field result in Python."
type: docs
weight: 25
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/find-field-properties/
timestamp: 2026-02-03-11-08-55
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page demonstrates how to retrieve a field’s code, result, and merge‑field names using Aspose.Words for Python via .NET.

{{% /alert %}}

A field that is inserted using [DocumentBuilder](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/).[insert_field](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_field/) returns a [Field](https://reference.aspose.com/words/python-net/aspose.words.fields/field/) object. This is a faсade class that provides useful methods to quickly find some properties of a field.

The following code example shows how to find the field code and field result:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-working_with_fields-GetFieldCode.py" >}}

Note if you are only looking for the names of merge fields in a document, then you can instead use the built-in [get_field_names](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names/) method.

The following code example shows how to get names of all merge fields in a document:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-working_with_fields-GetFieldNames.py" >}}

------ 

## FAQ

1. **Q:** How can I obtain the field code of a field inserted with `DocumentBuilder`?  
   **A:** After inserting the field, the `InsertField` method returns a `Field` object. Call `field.get_field_code()` to retrieve the full field code string, which includes the field name and its switches.

2. **Q:** How do I read the result (displayed text) of a field?  
   **A:** Use the `field.result` property. It returns the evaluated result of the field as a string. For example, `field_result = field.result`.

3. **Q:** What is the easiest way to list all merge field names in a document?  
   **A:** Use the static method `MailMerge.get_field_names(document)`. It returns a list of strings containing the names of every merge field found in the supplied `Document` object.

4. **Q:** Can I differentiate between different field types (e.g., MERGEFIELD, REF, PAGE) programmatically?  
   **A:** Yes. The `field.type` property returns a `FieldType` enumeration value. Compare it with members such as `aw.fields.FieldType.FIELD_MERGE_FIELD`, `aw.fields.FieldType.FIELD_REF`, etc., to identify the field type.

5. **Q:** How can I modify a field’s code after it has been created?  
   **A:** Retrieve the field code with `field.get_field_code()`, edit the string as needed, and then assign the modified code back using `field.set_field_code(modified_code)`. After updating, call `field.update()` to re‑evaluate the field.