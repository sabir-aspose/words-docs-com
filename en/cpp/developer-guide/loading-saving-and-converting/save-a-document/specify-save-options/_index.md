---
title: Specify Save Options in C++
second_title: Aspose.Words for C++
articleTitle: Specify Save Options
linktitle: Specify Save Options
description: "More accurately control the save process."
type: docs
weight: 10
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cpp/specify-save-options/
timestamp: 2024-01-27-14-07-04
---

When saving a document, you can set some advanced properties. Aspose.Words provides you with the [SaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/) class, which allows more precise control of the save process. There are overloads of the **Save** method that accept a **SaveOptions** object – it should be an object of a class derived from the **SaveOptions** class. Each save format has a corresponding class that holds save options for this save format, for example, there is [PdfSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/) for saving to PDF format, [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions) for saving to Markdown format, or [ImageSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/imagesaveoptions/) for saving to an image. This article provides examples of working with some options classes derived from **SaveOptions**.

The following code example shows how to set the save options before saving the document into HTML:

{{< gist "aspose-words-gists" "d55d8631947d283b1f0da99afa06c492" 
"cpp-Loading-and-Saving-SpecifySaveOption-SpecifySaveOption.cpp" >}}

{{% alert color="primary" %}}

You can download the template file of this example from [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-C/tree/master/Examples).

{{% /alert %}}

The article describes a few properties you can control when saving a document.

## Encrypt a Document With a Password

Use the **Password** property to get or set a password for an encrypted document. Use the **Password** property of the corresponding class to work with the selected document format.

For example, when saving a document to DOC or DOT format, use the [Password](https://reference.aspose.com/words/cpp/aspose.words.saving/docsaveoptions/get_password/) property of the [DocSaveOptions](https://reference.aspose.com/words/cpp/class/aspose.words.saving.doc_save_options) class.

The following code example shows how to set a password to encrypt a document using the RC4 encryption method:

{{< gist "aspose-words-gists" "d55d8631947d283b1f0da99afa06c492" 
"cpp-Loading-and-Saving-WorkingWithDoc-EncryptDocumentWithPassword.cpp" >}}

When saving a document to ODT format, use the [Password](https://reference.aspose.com/words/cpp/aspose.words.saving/odtsaveoptions/get_password/) property of the [OdtSaveOptions](https://reference.aspose.com/words/cpp/class/aspose.words.saving.odt_save_options) class.

The following code example shows how to load and save OpenDocument encrypted with a password:

{{< gist "aspose-words-gists" "d55d8631947d283b1f0da99afa06c492" 
"cpp-Loading-and-Saving-Load_Options-LoadAndSaveEncryptedODT.cpp" >}}

Not all formats support encryption and the use of **Password** property.

## Show Document Saving Progress Notifications

Aspose.Words provides the ability to use the [ProgressCallback](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/get_progresscallback/) property to get notifications about the progress of document saving.

It is now available when saving to DOCX, FlatOpc, DOCM, DOTM, DOTX, HTML, MHTML, EPUB, XamlFlow, XamlFlowPack, or TXT formats.

## Update the Document Creation Time

Aspose.Words provides an ability to use the [CreatedTime](https://reference.aspose.com/words/cpp/aspose.words.properties/builtindocumentproperties/get_createdtime/) property to get or set the document creation date in UTC. You can also update this value before saving using the [UpdateCreatedTimeProperty](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/get_updatecreatedtimeproperty/) option.

The following code example shows how to update the document creation time:

{{< gist "aspose-words-gists" "d55d8631947d283b1f0da99afa06c492" 
"cpp-Rendering-Printing-WorkingWithPdfSaveOptions-UpdateIfLastPrinted.cpp" >}}

## Update Last Saved Property

Aspose.Words provides an ability to use the [UpdateLastSavedTimeProperty](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/set_updatelastsavedtimeproperty/) property to gets or sets a value determining whether the [LastSavedTime](https://reference.aspose.com/words/cpp/aspose.words.properties/builtindocumentproperties/get_lastsavedtime/) property is updated before saving.

The following code example shows how to set this property and save the document:

{{< gist "aspose-words-gists" "d55d8631947d283b1f0da99afa06c492" 
"cpp-Loading-and-Saving-WorkingWithOoxml-UpdateLastSavedTimeProperty.cpp" >}}

## Save Black and White Image with One Bit Per Pixel Format

To control image saving options, the **ImageSaveOptions** class is used. For example, you can use the [PixelFormat](https://reference.aspose.com/words/cpp/aspose.words.saving/imagesaveoptions/set_pixelformat/) property to set the pixel format for the generated images. Please note that the pixel format of the output image may differ from the set value because of the work of GDI+.

The following code example shows how to save a black and white image with one bit per pixel format:

{{< gist "aspose-words-gists" "d55d8631947d283b1f0da99afa06c492" "cpp-Rendering-Printing-ImageColorFilters-SaveImageToOnebitPerPixel.cpp" >}}

------  

## FAQ

1. **Q:** How can I set a password when saving a document to PDF in C++?  
   **A:** Use the `PdfSaveOptions` class and assign the desired password to its `Password` property. Then pass the `PdfSaveOptions` instance to `Document::Save`. Example:  

   ```cpp
   Aspose::Words::Saving::PdfSaveOptions saveOptions;
   saveOptions.set_Password(u"Secret123");
   doc->Save(u"Encrypted.pdf", saveOptions);
   ```

2. **Q:** Which property lets me receive progress notifications while a document is being saved?  
   **A:** Assign an implementation of `IProgressCallback` to the `ProgressCallback` property of the appropriate `SaveOptions` class (e.g., `DocxSaveOptions`). The callback’s `Notify` method will be called periodically with the percentage completed.

3. **Q:** How do I update the document’s creation time before saving?  
   **A:** Set the `CreatedTime` property of the document’s built‑in properties, then enable `UpdateCreatedTimeProperty` on the `SaveOptions` you use.  

   ```cpp
   doc->get_BuiltInDocumentProperties()->set_CreatedTime(Aspose::System::DateTime::Now);
   Aspose::Words::Saving::SaveOptions saveOptions;
   saveOptions.set_UpdateCreatedTimeProperty(true);
   doc->Save(u"output.docx", saveOptions);
   ```

4. **Q:** Can I force the last‑saved timestamp to be refreshed when saving?  
   **A:** Yes. Set `UpdateLastSavedTimeProperty` to `true` on the `SaveOptions` object you pass to `Document::Save`. This makes Aspose.Words write the current UTC time to the `LastSavedTime` property.

5. **Q:** How can I save an image generated from a document as a 1‑bit black‑and‑white PNG?  
   **A:** Use `ImageSaveOptions`, set its `PixelFormat` to `PixelFormat::Format1bppIndexed`, and then save the document page as an image.  

   ```cpp
   Aspose::Words::Saving::ImageSaveOptions imgOptions;
   imgOptions.set_PixelFormat(Aspose::Words::Saving::PixelFormat::Format1bppIndexed);
   doc->Save(u"page.png", imgOptions);
   ```