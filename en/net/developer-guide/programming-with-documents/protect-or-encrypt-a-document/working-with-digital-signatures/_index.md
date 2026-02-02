---
title: Work with Digital Signatures in C#
second_title: Aspose.Words for .NET
articleTitle: Work with Digital Signatures
linktitle: Work with Digital Signatures
description: "Digitally sign documents and detect, count, verify, and remove existing digital signatures using C#."
type: docs
weight: 40
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/working-with-digital-signatures/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page explains how to work with digital signatures, including signing and verification.

{{% /alert %}}

A digital signature is a technological implementation of electronic signatures to sign documents and authenticate the signer to guarantee that a document has not been modified since it was signed. Each digital signature is unique for each signer because of following the PKI protocol to generate both public and private keys. Signing a document digitally means creating a signature using the signer's private key where a mathematical algorithm is used to encrypt the generated hash.

Aspose.Words allows you to detect, count, or verify existing digital signatures, and also add a new signature to your document to find out any tampering in it. You can also remove all digital signatures from a document. Use the [DigitalSignatureUtil](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignatureutil/) class to work with digital signatures.

This article explains how to do all of the above to validate the authenticity and integrity of a digital document.

{{% alert color="primary" %}}

Note that you can access digital signatures of your document only when running the .NET Framework 2.0 version and above.

{{% /alert %}}

{{% alert color="primary" %}}

**Try online**

You can try this functionality with our [Free online signature](https://products.aspose.app/words/signature).

{{% /alert %}}

## Supported Formats

Aspose.Words allows you to work with digital signatures on DOC, OOXML, and ODT documents and to sign the generated document in PDF or XPS format.

## Limitations of Digital Signatures

The table below describes a few limitations that you may face while working with digital signatures through Aspose.Words, as well as some alternative options.

| Limitation | Alternative Option                                           |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Loss of digital signatures on a document after loading and saving it. Therefore, processing a document to a server may cause the loss of all digital signatures without a notice. | Check if a document has digital signatures and take the appropriate action if any are found. For example, send an alert to the clients informing them that the document they are uploading contains digital signatures that will be lost if it is processed. |
| Aspose.Words supports working with macros in a document. But Aspose.Words does not yet support digital signatures on macros. | Export the document back to any Word format, and use Microsoft Word to add a digital signature to macros. |

## Detect, Count, and Verify Digital Signatures

Aspose.Words allows you to detect digital signature in a document using the the [DetectFileFormat](https://reference.aspose.com/words/net/aspose.words/fileformatutil/detectfileformat/#detectfileformat/) method and the [HasDigitalSignature](https://reference.aspose.com/words/net/aspose.words/fileformatinfo/hasdigitalsignature/) property. It is worth noting that such a check will only detect the fact of the signature, but not its validity.

A document can be signed more than once, and this can be done by different users. To check the validity of digital signatures, you need to load them from the document using the [LoadSignatures](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignatureutil/loadsignatures/#loadsignatures/) method and use the [IsValid](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignaturecollection/isvalid/) property. Also Aspose.Words allows you to count a set of all digital signatures within a document using the [Count](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignaturecollection/count/) property.

All of this provides an efficient and safe way to check a document for signatures before processing it.

The following code example shows how to detect the presence of digital signatures and verify them:

{{< gist "aspose-words-gists" "bdc15a6de6b25d9d4e66f2ce918fc01b" "detect-document-signatures.cs" >}}

## Create a Digital Signature {#create-a-digital-signature}

To create a digital signature, you will require to load a signing certificate that confirms identity. When you send a digitally signed document, you also send your certificate and public key.

Aspose.Words allows you to create X.509 certificate, a digital certificate that uses the internationally accepted X.509 PKI standard to verify that a public key belongs to the signer included inside the certificate. To do this, use the [Create](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/certificateholder/create/) method within the [CertificateHolder](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/certificateholder/) class.

The next sections explain how to add a digital signature, signature line, and how to sign a generated PDF document.

### Sign a Document

Aspose.Words allows you to sign a DOC, DOCX, XPS, or ODT document digitally using the [Sign](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignatureutil/sign/#sign/) method and [SignOptions](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/signoptions/) properties.

The following code example shows how to sign documents using a certificate holder and sign options:

{{< gist "aspose-words-gists" "bdc15a6de6b25d9d4e66f2ce918fc01b" "sign-document.cs" >}}

### Add a Signature Line

A signature line is a visual representation of a digital signature in a document. Aspose.Words allows you to insert a signature line using the [DocumentBuilder.InsertSignatureLine](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertsignatureline/) method.  You can also set the parameters for this representation using the [SignatureLineOptions](https://reference.aspose.com/words/net/aspose.words/signaturelineoptions/) class.

For example, the picture below shows how valid and invalid signatures can be displayed.

<img src="valid.png" alt="drawing" style="width:300px"/>

<img src="invalid.png" alt="drawing" style="width:300px"/>

Also, if a document contains a signature line and no digital signature, there is a feature to ask the user to add a signature.

The following code example shows how to sign a document with a personal certificate and a specific signature line:

{{< gist "aspose-words-gists" "bdc15a6de6b25d9d4e66f2ce918fc01b" "create-new-signature-line-and-set-provider-id.cs" >}}

### Sign a Generated PDF Document {#sign-a-generated-pdf-document}

Aspose.Words allows you to sign and get all details of a PDF document using the [PdfDigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/pdfdigitalsignaturedetails/) properties.

The following code example shows how to sign a generated PDF:

{{< gist "aspose-words-gists" "bdc15a6de6b25d9d4e66f2ce918fc01b" "digitally-signed-pdf-using-certificate-holder.cs" >}}

## Retrieve the Digital Signature Value

Aspose.Words also provides the ability to retrieve the digital signature value from a digitally signed document as a byte array using the [SignatureValue](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignature/signaturevalue/) property.

The following code example shows how to obtain the digital signature value as a byte array from a document:

{{< gist "aspose-words-gists" "bdc15a6de6b25d9d4e66f2ce918fc01b" "signature-value.cs" >}}

## Remove Digital Signatures

Aspose.Words allows you to remove all digital signatures from a signed document using the [RemoveAllSignatures](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignatureutil/removeallsignatures/#removeallsignatures/) method.

The following code example shows how to load and remove digital signatures from a document:

{{< gist "aspose-words-gists" "bdc15a6de6b25d9d4e66f2ce918fc01b" "remove-signatures.cs" >}}

{{% alert color="primary" %}}

Note that you can not remove only one digital signature within your document.

{{% /alert %}}

------ 

## FAQ

1. **Q:** How can I check whether a document contains any digital signatures?  
   **A:** Use `FileFormatUtil.DetectFileFormat` to identify the file type and then read the `HasDigitalSignature` property from the `FileFormatInfo` object. This returns `true` if at least one digital signature is present.

2. **Q:** How do I verify the validity of the digital signatures in a document?  
   **A:** Load the signatures with `DigitalSignatureUtil.LoadSignatures`, then iterate through the returned `DigitalSignatureCollection` and examine each signature’s `IsValid` property. A value of `true` indicates a valid, untampered signature.

3. **Q:** How can I count the number of digital signatures in a document?  
   **A:** After loading the signatures using `DigitalSignatureUtil.LoadSignatures`, read the `Count` property of the resulting `DigitalSignatureCollection`. This gives the total number of signatures attached to the document.

4. **Q:** What is the recommended way to add a digital signature to a Word document?  
   **A:** Create a `CertificateHolder` with your X.509 certificate (`CertificateHolder.Create`), configure `SignOptions` as needed, and call `DigitalSignatureUtil.Sign` passing the document, the certificate holder, and the sign options.

5. **Q:** Can I remove a single digital signature from a document?  
   **A:** No. Aspose.Words currently supports only the removal of all signatures at once via `DigitalSignatureUtil.RemoveAllSignatures`. To remove a specific signature you would need to recreate the document without that signature using external tools.