---
title: Working with Hyperlinks
second_title: Aspose.Words for Python via .NET
articleTitle: Add or Modify Hyperlinks
linktitle: Add or Modify Hyperlinks
description: "Add, replace, or modify a hyperlink in a document using Python."
type: docs
weight: 50
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/working-with-hyperlinks/
aliases:
- /python/working-with-hyperlinks-and-html/
- /python-net/working-with-hyperlinks-and-html/
timestamp: 2024-01-27-14-07-04
---

A hyperlink in Microsoft Word documents is the `HYPERLINK` field. In Aspose.Words, hyperlinks are implemented through the [FieldHyperlink](https://reference.aspose.com/words/python-net/aspose.words.fields/fieldhyperlink/) class.

## Inserting a Hyperlink

Use the [insert_hyperlink](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_hyperlink/) method to insert a hyperlink into the document. This method accepts three parameters:

1. Text of the link to be displayed in the document
2. Link destination (URL or a name of a bookmark inside the document)
3. Boolean parameter that should be true if the `URL` is a name of a bookmark inside a document

The **InsertHyperlink** method always adds apostrophes at the beginning and end of the URL.

{{% alert color="primary" %}}

Note that you need to specify font formatting for the hyperlink display text explicitly using the `Font` property.

{{% /alert %}}

The following code example shows how to insert a hyperlink into a document using [DocumentBuilder](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Document-add_content_using_document_builder-InsertHyperlink.py" >}}

## Replace or Modify Hyperlinks

Hyperlink in Microsoft Word documents is a field. A field in a Word document is a complex structure consisting of multiple nodes that include field start, field code, field separator, field result and field end. Fields can be nested, contain rich content and span multiple paragraphs or sections in a document. 

To replace or modify hyperlinks, it is need to find the hyperlinks in the document and replace either their text, URLs, or both.

The following code example shows how to find all hyperlinks in Word document and changes their `URL` and display name:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-working_with_fields-ReplaceHyperlinks.py" >}}

------  

## FAQ

1. **Q:** How can I insert a hyperlink that points to a bookmark inside the same document?  
   **A:** Pass the bookmark name as the second argument to `insert_hyperlink` and set the third argument (`is_bookmark`) to `True`. Example:  

   ```python
   builder.insert_hyperlink("Go to Intro", "IntroBookmark", True)
   ```

2. **Q:** How do I change the display text of an existing hyperlink without altering its URL?  
   **A:** Locate the `FieldHyperlink` node, modify its `Result` property (the displayed text), and then update the document.  

   ```python
   for field in doc.get_child_nodes(aspose.words.NodeType.FIELD_START, True):
       if isinstance(field, aspose.words.fields.FieldHyperlink):
           field.result = "New Display Text"
   ```

3. **Q:** Is it possible to remove a hyperlink while keeping the link text?  
   **A:** Yes. Replace the `FieldHyperlink` with a plain `Run` node that contains the same text. Remove the field start, separator, and end nodes, then insert a `Run` with the original result text.

4. **Q:** How can I apply custom font formatting (e.g., color, underline) to a hyperlink after insertion?  
   **A:** After calling `insert_hyperlink`, the builder’s `font` property refers to the hyperlink text. Set the desired properties before moving the cursor away.  

   ```python
   builder.insert_hyperlink("Aspose", "https://www.aspose.com", False)
   builder.font.color = aspose.words.Color.blue
   builder.font.underline = aspose.words.Underline.SINGLE
   ```

5. **Q:** Can I retrieve a list of all hyperlink URLs in a document?  
   **A:** Iterate through all `FieldHyperlink` nodes and read their `Hyperlink` property.  

   ```python
   urls = []
   for field in doc.get_child_nodes(aspose.words.NodeType.FIELD_START, True):
       if isinstance(field, aspose.words.fields.FieldHyperlink):
           urls.append(field.hyperlink)
   ```