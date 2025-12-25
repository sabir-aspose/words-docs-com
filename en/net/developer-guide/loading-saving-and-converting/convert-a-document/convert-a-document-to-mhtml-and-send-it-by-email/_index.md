---
title: Convert File to MHTML and Send It by Email
second_title: Aspose.Words for .NET
articleTitle: Convert a Document to MHTML and Send It by Email
linktitle: Convert a Document to MHTML and Send It by Email
description: "Convert a document from almost any format to the MHTML format and send the result document by e-mail using C#."
type: docs
weight: 30
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/convert-a-document-to-mhtml-and-send-it-by-email/
timestamp: 2024-07-09-19-00-42
---

{{% alert color="grey" %}}

*What is this page about?*

This page describes how to convert a document to MHTML and send it via email, demonstrating both conversion settings and SMTP workflow integration.

{{% /alert %}}

Aspose.Words can convert any document to the MHTML (Web Archive) format. This makes it convenient to use Aspose.Words and `Aspose.Email` together. You can load a predefined document in any supported format, such as DOC, OOXML, or RTF, into Aspose.Words, fill it with data, save the resulting document as MHTML, and then send it by e‑mail using `Aspose.Email`.

The following code example shows how to convert any document to MHTML and send it by email:

{{< gist "aspose-words-gists" "537e7d4e2ddd23fa701dc4bf315064b9" "docx-to-mhtml.cs" >}}

------  

## FAQ

1. **Q:** Which document formats can be converted to MHTML with Aspose.Words?  
   **A:** Aspose.Words supports conversion from all formats it can load, including DOC, DOCX, RTF, HTML, ODT, and many others. Any of these can be saved directly as MHTML.

2. **Q:** Do I need a separate license for Aspose.Email when sending the MHTML file?  
   **A:** Yes. Aspose.Words handles the conversion, while Aspose.Email is a separate product used for SMTP operations. Both products require their own valid licenses.

3. **Q:** Can I customize the MIME type or encoding of the MHTML attachment?  
   **A:** After saving the document as MHTML (`document.Save("output.mht", SaveFormat.Mhtml)`), you can create an `Aspose.Email.MailMessage`, set the `ContentType` of the attachment, and specify the desired charset before sending.

4. **Q:** Is it possible to convert a document to MHTML without loading the entire file into memory?  
   **A:** Yes. You can open the source document from a stream (`Document doc = new Document(stream)`) and save it directly to a stream in MHTML format, which reduces memory usage for large files.

5. **Q:** How can I ensure the generated MHTML preserves the original document’s fonts and images?  
   **A:** Aspose.Words embeds referenced resources (fonts, images, CSS) into the MHTML file automatically. Ensure the source document has access to the required resources, or embed them manually using `Document.FontSettings` before saving.