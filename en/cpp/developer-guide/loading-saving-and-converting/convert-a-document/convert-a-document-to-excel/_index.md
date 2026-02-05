---
title: Convert Word to Excel in C++
second_title: Aspose.Words for C++
articleTitle: Convert a Document to Excel
linktitle: Convert a Document to Excel
description: "Convert PDF to Excel, XML to Excel, DOCX to Excel C++. Save a document in various formats to XLSX using C++."
type: docs
weight: 15
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cpp/convert-a-document-to-excel/
timestamp: 2024-01-31-14-23-37
---

Converting documents from one format to another is the flagship feature of Aspose.Words. You can convert documents in any available [load format](https://reference.aspose.com/words/cpp/aspose.words/loadformat/) also to XLSX format.

## Convert a Document to XLSX

Converting a document to XLSX is a rather complicated process. To save your document to XLSX format using Aspose.Words, use the **XlsxSaveOptions** class and the new `Xlsx` element in the [SaveFormat](https://reference.aspose.com/words/cpp/aspose.words/saveformat/) enumeration. As mentioned above, you can save the document in any load format supported by Aspose.Words to XLSX.

The following code example shows how to save PDF to XLSX:

{{< highlight cpp >}}
auto doc = MakeObject<Document>(MyDir + u"Pdf Document.pdf");
doc->Save(ArtifactsDir + u"BaseConversions.PdfToXlsx.xlsx");
{{< /highlight >}}

## Find and Replace When Saving to XLSX

Also using Aspose.Words, you can find a specific string or regular expression in your document and replace it with the matching one you need. Then you can also save the result to XLSX format.

The following code example shows how to perform find and replace operation and save result to XLSX:

{{< highlight cpp >}}
auto doc = MakeObject<Document>();
auto builder = MakeObject<DocumentBuilder>(doc);

builder->Writeln(u"Ruby bought a ruby necklace.");

// We can use a "FindReplaceOptions" object to modify the find-and-replace process.
auto options = MakeObject<FindReplaceOptions>();
// Set the "MatchCase" flag to "true" to apply case sensitivity while finding strings to replace.
// Set the "MatchCase" flag to "false" to ignore character case while searching for text to replace.
options->set_MatchCase(true);

doc->get_Range()->Replace(u"Ruby", u"Jade", options);
doc->Save(ArtifactsDir + u"BaseConversions.FindReplaceXlsx.xlsx");
{{< /highlight >}}

## Specify Compression Level When Saving to XLSX

You can also specify the compression level when saving using the **CompressionLevel** property.

The following code example shows how to specify the compression level when saving to XLSX format:

{{< highlight cpp >}}
auto doc = MakeObject<Document>(MyDir + u"Document.docx");
auto saveOptions = MakeObject<XlsxSaveOptions>();
saveOptions->set_CompressionLevel(CompressionLevel::Maximum);

doc->Save(ArtifactsDir + u"BaseConversions.CompressXlsx.xlsx", saveOptions);
{{< /highlight >}}

## See Also

- Documentation section [Protect or Encrypt a Document](/words/cpp/protect-or-encrypt-a-document/) for more information about protecting and encrypting a document
- The article [Find and Replace](/words/cpp/find-and-replace/) for more more information about finding and replacing the content you want

------ 

## FAQ

1. **Q:** How can I convert a PDF document to Excel (XLSX) using Aspose.Words for C++?  
   **A:** Load the PDF with the `Document` class and call `Save` specifying an XLSX file name. Aspose.Words automatically detects the source format and writes the spreadsheet. Example:  
   ```cpp
   auto doc = MakeObject<Document>(MyDir + u"Pdf Document.pdf");
   doc->Save(ArtifactsDir + u"Result.xlsx");
   ```

2. **Q:** Can I perform find‑and‑replace on a document before saving it as Excel?  
   **A:** Yes. Use `FindReplaceOptions` together with `Range::Replace` to modify the document content, then save the updated document to XLSX. The same code shown in the “Find and Replace When Saving to XLSX” section applies.

3. **Q:** How do I control the compression level of the generated XLSX file?  
   **A:** Create an `XlsxSaveOptions` instance, set its `CompressionLevel` property (e.g., `CompressionLevel::Maximum`), and pass the options to `Document::Save`. This reduces file size at the cost of longer save time.

4. **Q:** Do I need a license to convert documents to Excel, and how do I apply it in C++?  
   **A:** A license is required for production use to remove evaluation watermarks and enable full functionality. Load the license file with the `License` class before any document operations:  
   ```cpp
   auto license = MakeObject<License>();
   license->SetLicense(u"Path/To/Aspose.Words.CPP.lic");
   ```
   After setting the license, all conversion features work without restrictions.