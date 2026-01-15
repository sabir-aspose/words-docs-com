---
title: Mail Merge Template in Python
second_title: Aspose.Words for Python via .NET
articleTitle: Mail Merge Template
linktitle: Mail Merge Template
type: docs
description: "Create a Mail Merge template to define fixed content in output documents, and then generate merge documents using the merge fields in Python."
keywords: "create Mail Merge template python"
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/mail-merge-template/
aliases: [/python/mail-merge-template/]
timestamp: 2024-01-31-14-23-37
---

It is common to use a merge template as the base document for a Mail Merge operation either if it is a simple Mail Merge or Mail Merge with regions. Mail merge with regions is more powerful and popular than the simple mail merge. Simple Mail Merge is considered as a particular case of Mail Merge with regions where the region is the entire document. All is explained in the next article “Types of Mail Merge Operation” in more detail.

The template ensures that the text in the output merged document is formatted correctly, and the Mail Merge operation guarantees that the text from the data source is correctly entered into the merge template.

Aspose.Words provides the ability to create a Mail Merge template to define fixed content and then generate merge documents using the merge fields. Thus, the merge template will have the necessary text, which is the same in all of the output documents, and the merge fields to fill in the changing content. As a result, information from the specified data source will be added to the merge template through these fields during the generation of the merged document.

## What is a Mail Merge Template

A Mail Merge template is a personalized document that contains the fixed data and the merged fields where you want the variable text to be. A merge template can be in any format that supports fields, for example, DOC, DOCX, DOT, DOTX, RTF. In addition, you can also use the mustache template that is explained in the article “Mustache Template Syntax” in more detail.

You can create a merge template to be a model for new documents, and it should include the main text that needs to be the same for each version of the merged document. Adding merge fields inside the template will represent the personalization data such as names or addresses that are fetched from a data source. A Mail Merge operation will automatically insert the personalization data from your data source to your merge template document.

In addition, you can add a Mail Merge region in your template by inserting two Mail Merge fields to mark the beginning and the end of the mail region. The next article “Types of Mail Merge Operation” explains that in more detail.

## Create a Mail Merge Template

You can create a template and add specific merge fields to it, that will be replaced by the values from the data source either manually, for example, using Microsoft Word, or programmatically using Aspose.Words. In this article, we will look at the programmatic way of creating a template.

Use the [DocumentBuilder](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/) class to create the required merge template using Aspose.Words. You can include a text, a merge field, and a line break in such a template using the [insert_text_input](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_text_input/), [inset_field](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_field/), and [insert_paragraph](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_paragraph/) methods.

The following code example shows how to create a Mail Merge template:

{{< highlight python >}}
@staticmethod
def create_mail_merge_template() :
    
    builder = aw.DocumentBuilder()
    
    # Insert a text input field the unique name of this field is "Hello", the other parameters define
    # what type of FormField it is, the format of the text, the field result and the maximum text length (0 = no limit)
    builder.insert_text_input("TextInput", aw.fields.TextFormFieldType.REGULAR, "", "Hello", 0)
    builder.insert_field("MERGEFIELD CustomerFirstName \\* MERGEFORMAT")
    
    builder.insert_text_input("TextInput1", aw.fields.TextFormFieldType.REGULAR, "", " ", 0)
    builder.insert_field("MERGEFIELD CustomerLastName \\* MERGEFORMAT")
    
    builder.insert_text_input("TextInput1", aw.fields.TextFormFieldType.REGULAR, "", " , ", 0)
    
    # Inserts a paragraph break into the document
    builder.insert_paragraph()
    
    # Insert mail body
    builder.insert_text_input("TextInput", aw.fields.TextFormFieldType.REGULAR, "", "Thanks for purchasing our ", 0)
    builder.insert_field("MERGEFIELD ProductName \\* MERGEFORMAT")
    
    builder.insert_text_input("TextInput", aw.fields.TextFormFieldType.REGULAR, "", ", please download your Invoice at ", 0)
    builder.insert_field("MERGEFIELD InvoiceURL \\* MERGEFORMAT")
    
    builder.insert_text_input("TextInput", aw.fields.TextFormFieldType.REGULAR, "", ". If you have any questions please call ", 0)
    builder.insert_field("MERGEFIELD Supportphone \\* MERGEFORMAT")
    
    builder.insert_text_input("TextInput", aw.fields.TextFormFieldType.REGULAR, "", ", or email us at ", 0)
    builder.insert_field("MERGEFIELD SupportEmail \\* MERGEFORMAT")
    
    builder.insert_text_input("TextInput", aw.fields.TextFormFieldType.REGULAR, "", ".", 0)
    
    builder.insert_paragraph()
    
    # Insert mail ending
    builder.insert_text_input("TextInput", aw.fields.TextFormFieldType.REGULAR, "", "Best regards,", 0)
    builder.insert_break(aw.BreakType.LINE_BREAK)
    builder.insert_field("MERGEFIELD EmployeeFullname \\* MERGEFORMAT")
    
    builder.insert_text_input("TextInput1", aw.fields.TextFormFieldType.REGULAR, "", " ", 0)
    builder.insert_field("MERGEFIELD EmployeeDepartment \\* MERGEFORMAT")
    
    return builder.document
{{< /highlight >}}

The picture below shows the created template:

<img src="mail-merge-template-1.png" alt="mail_merge_template" style="width:650px"/>

## Customize a Mail Merge Template Properties

Aspose.Words allows you to customize your template through many properties. Template customization will be described below through an example of customizing some properties of images and text.

## See Also

* For more details about how to create templates in Microsoft Word manually, please check the [Create a Template](https://support.microsoft.com/en-us/office/save-a-word-document-as-a-template-cb17846d-ecec-49d4-82ea-a6f5e3e8b9ae) article in the Microsoft Documentation



------ 

## FAQ

1. **Q:** How can I create a Mail Merge template programmatically in Python?  
   **A:** Use `DocumentBuilder` to build a new `Document`, insert text input fields and merge fields with `insert_text_input` and `insert_field`. After constructing the template, return `builder.document` and save it or use it directly for a mail merge operation.

2. **Q:** How do I define a Mail Merge region (start and end) in the template?  
   **A:** Insert two merge fields that mark the region boundaries, e.g., `builder.insert_field("MERGEFIELD TableStart \\* MERGEFORMAT")` at the beginning and `builder.insert_field("MERGEFIELD TableEnd \\* MERGEFORMAT")` at the end. The region will be processed by `MailMerge.ExecuteWithRegions` using the same field names.

3. **Q:** Can I use a Mustache template together with Aspose.Words Mail Merge?  
   **A:** Yes. Create the template as a Mustache file (e.g., `.mustache`), then load it with `aw.Document("template.mustache")`. After rendering the Mustache placeholders, perform the standard Mail Merge on the resulting document.

4. **Q:** How can I change the font size of text that is inserted via `insert_text_input`?  
   **A:** Set the font properties on the `DocumentBuilder` before inserting the field:  
   ```python
   builder.font.size = 12   # points
   builder.insert_text_input("TextInput", aw.fields.TextFormFieldType.REGULAR, "", "Sample", 0)
   ```

5. **Q:** How do I load an existing template and execute a Mail Merge in Python?  
   **A:** Load the template with `aw.Document("Template.docx")`, then call `document.mail_merge.execute(data_table)` or `execute_with_regions` for regions. The merge fields in the template will be replaced with data from the provided `DataTable` or list of dictionaries.