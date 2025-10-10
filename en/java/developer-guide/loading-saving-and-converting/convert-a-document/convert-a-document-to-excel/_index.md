---
title: Convert Word to Excel in Java
second_title: Aspose.Words for Java
articleTitle: Convert a Document to Excel
linktitle: Convert a Document to Excel
description: "Convert XML to Excel, Word to Excel (including DOCX to Excel) in Java. Save a document in various formats to XLSX using Java."
type: docs
weight: 15
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /java/convert-a-document-to-excel/
timestamp: 2024-01-31-14-23-37
---

Converting documents from one format to another is the flagship feature of Aspose.Words. You can convert documents in any available [load format](https://reference.aspose.com/words/java/com.aspose.words/loadformat/) also to XLSX format.

## Convert a Document to XLSX

Converting a document to XLSX is a rather complicated process. To save your document to XLSX format using Aspose.Words, use the [XlsxSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/) class and the new `Xlsx` element in the [SaveFormat](https://reference.aspose.com/words/java/com.aspose.words/saveformat/) enumeration. As mentioned above, you can save the document in any load format supported by Aspose.Words to XLSX.

The following code example shows how to save DOCX to XLSX:

{{< gist "aspose-words-gists" "82fb3ee435d5abdc1472a58774ebe98c" "docx-to-xlsx.java" >}}

{{% alert color="primary" %}}

Sometimes it is necessary to specify additional options, which can affect the result of saving a document as a XLSX. These options can be specified using the [XlsxSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/) class, containing properties that determine how the XLSX output will be displayed.

{{% /alert %}}

## Find and Replace When Saving to XLSX

Also using Aspose.Words, you can find a specific string or regular expression in your document and replace it with the matching one you need. Then you can also save the result to XLSX format.

The following code example shows how to perform find and replace operation and save result to XLSX:

{{< gist "aspose-words-gists" "50971daf8f0c9ef4b0250c4a526b1652" "find-replace-xlsx.java" >}}

## Specify Compression Level When Saving to XLSX

You can also specify the compression level when saving using the [CompressionLevel](https://reference.aspose.com/words/java/com.aspose.words/compressionlevel/) property.

The following code example shows how to specify the compression level when saving to XLSX format:

{{< gist "aspose-words-gists" "50971daf8f0c9ef4b0250c4a526b1652" "compress-xlsx.java" >}}

## See Also

- Documentation section [Protect or Encrypt a Document](/words/java/protect-or-encrypt-a-document/) for more information about protecting and encrypting a document
- The article [Find and Replace](/words/java/find-and-replace/) for more more information about finding and replacing the content you want
