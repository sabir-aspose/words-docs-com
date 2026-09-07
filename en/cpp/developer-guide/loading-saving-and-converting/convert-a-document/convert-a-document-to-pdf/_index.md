---
title: Convert a Document to PDF in C++
second_title: Aspose.Words for C++
articleTitle: Convert a Document to PDF
linktitle: Convert a Document to PDF
description: "Convert a document to PDF using C++. Various input formats are supported, including Word, OpenOffice, Image and eBook formats."
type: docs
weight: 10
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cpp/convert-a-document-to-pdf/
timestamp: 2024-10-21-08-52-03
---

The ability to easily and reliably convert documents from one format to another is a key feature of Aspose.Words. One of the most popular formats for converting is PDF – a fixed‑layout format, which preserves the original appearance of a document during its rendering on various platforms. The “rendering” term is used in Aspose.Words to describe the process of converting a document into a file format that is paginated or has the concept of pages.

## Convert a Word Document to PDF {#convert-a-word-document-to-pdf}

Conversion from Word to PDF is a rather complex process that requires several stages of calculation. Aspose.Words layout engine mimics the way Microsoft Word's page layout engine works, making PDF output documents look as close as possible to what you can see in Microsoft Word.

With Aspose.Words you can programmatically convert a document from DOC or DOCX format to PDF without using Microsoft Office. This article explains how to perform this conversion.

{{% alert color="primary" %}}

Note that the number of pages in a document affects the conversion time.

{{% /alert %}}

### Converting DOCX or DOC to PDF {#converting-doc-or-docx-to-pdf}

Converting from the DOC or DOCX document format into the PDF format in Aspose.Words is very easy and can be accomplished with just two lines of code that:

1. Load your document into a[Document](https://reference.aspose.com/words/cpp/aspose.words/document/)object using one of its constructors by specifying the document name with its format extension.
2. Invoke one of the[Document.Save](https://reference.aspose.com/words/cpp/aspose.words/document/save/)methodson the**Document**object and specify the desired output format as PDF by entering afile name with the “.PDF” extension.

The following code example shows how to convert a document from DOCX into PDF using the `Save` method:

{{< gist "aspose-words-gists" "b9784b73e288805e08fba6e3fc5ae2af" "docx-to-pdf.h" >}}

You can download the template file of this example from[Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-C/tree/master/Examples).

{{% alert color="primary" %}}

Sometimes it is necessary to specify additional options, which can affect the result of saving a document as a PDF. These options can be specified using the[PdfSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/)class, containing properties that determine how the PDF output will be displayed.

Note that with the same technique, you can convert any flow‑layout format document to PDF format.

{{% /alert %}}

### Convert to Different PDF Standards {#converting-to-various-pdf-standards}

Aspose.Words provides the[PdfCompliance](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/get_compliance/) enumeration to support the conversion of DOC orDOCX into various PDF format standards (such as PDF 1.7, PDF 1.5, etc.).

The following code example demonstrates how to convert a document to PDF 1.7 using[PdfSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/)with compliance to PDF17:

{{< gist "aspose-words-gists" "b9784b73e288805e08fba6e3fc5ae2af" "conversion-to-pdf17.h" >}}

## Convert Images to PDF {#convert-an-image-to-pdf}

Converting to PDF is not restricted byMicrosoft Word document formats. Any format supported by Aspose.Words, including programmatically created, can also be converted to PDF. For example, we can convert single‑page images, such as JPEG, PNG, BMP, EMF, or WMF, as well as multi‑page images, such as TIFF and GIF, to PDF.

The following code example shows how to convert JPEG and TIFF images to PDF:

{{< gist "aspose-words-gists" "b9784b73e288805e08fba6e3fc5ae2af" "image-to-pdf.h" >}}

{{< gist "aspose-words-gists" "b9784b73e288805e08fba6e3fc5ae2af" "convert-image-to-pdf.h" >}}

To make this code work, you need to add references to Aspose.Words and `System.Drawing` to your project.

## See Also

- The article[Rendering](/words/cpp/rendering/)for more information on the fixed‑page and flow‑layout formats
- The article[Converting to Fixed‑page Format](/words/cpp/converting-to-fixed-page-format/#what-is-a-page-layout)for more information on the page layout
- The article[Specify Rendering Options When Converting to PDF](/words/cpp/specify-rendering-options-when-converting-to-pdf/)for more information on using the `PdfSaveOptions` class

------ 

## FAQ

1. **Q:** How do I convert a DOCX file to PDF using Aspose.Words for C++?  
   **A:** Load the DOCX into an `Aspose::Words::Document` object and call its `Save` method with a file name ending in “.pdf”. Example:  

   ```cpp
   Aspose::Words::Document doc(u"input.docx");
   doc.Save(u"output.pdf");
   ```

2. **Q:** How can I create a PDF that complies with a specific standard such as PDF/A‑1b or PDF/X‑4?  
   **A:** Use `Aspose::Words::Saving::PdfSaveOptions` and set its `Compliance` property to the desired `PdfCompliance` value, then pass the options to `Document::Save`. Example:  

   ```cpp
   Aspose::Words::Saving::PdfSaveOptions options;
   options.set_Compliance(Aspose::Words::Saving::PdfCompliance::PdfA1b);
   doc.Save(u"output_pdfa.pdf", options);
   ```

3. **Q:** How can I protect the generated PDF with a password?  
   **A:** Configure the `EncryptionDetails` of `PdfSaveOptions` with a user password (and optionally an owner password) and assign an encryption algorithm. Then save the document with those options. Example:  

   ```cpp
   Aspose::Words::Saving::PdfSaveOptions options;
   options.get_EncryptionDetails().set_UserPassword(u"myPassword");
   options.get_EncryptionDetails().set_EncryptionAlgorithm(Aspose::Words::Saving::PdfEncryptionAlgorithm::Aes256);
   doc.Save(u"protected.pdf", options);
   ```

4. **Q:** How can I control image quality or compression when converting images to PDF?  
   **A:** Set `ImageCompression` (e.g., `PdfImageCompression::Jpeg`) and `JpegQuality` (0‑100) on `PdfSaveOptions`. This reduces file size while preserving visual quality. Example:  

   ```cpp
   Aspose::Words::Saving::PdfSaveOptions options;
   options.set_ImageCompression(Aspose::Words::Saving::PdfImageCompression::Jpeg);
   options.set_JpegQuality(80);
   doc.Save(u"images.pdf", options);
   ```

5. **Q:** How do I combine several images (e.g., a multi‑page TIFF) into a single PDF document?  
   **A:** Load each image as a separate `Document` (or use `ImageLoadOptions` for multi‑page images) and append them to a master document using `Document::AppendDocument`. Finally, save the master document as PDF. Example:  

   ```cpp
   Aspose::Words::Document master(u"");
   Aspose::Words::Document imgDoc(u"page1.tiff");
   master.AppendDocument(imgDoc, Aspose::Words::ImportFormatMode::KeepSourceFormatting);
   // repeat for additional pages...
   master.Save(u"combined.pdf");
   ```