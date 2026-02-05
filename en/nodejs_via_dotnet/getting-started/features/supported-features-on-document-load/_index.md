---
title: Supported Features on Document Load
second_title: Aspose.Words for Node.js via .NET
articleTitle: Supported Features on Document Load
linktitle: Supported Features on Document Load
description: "Load your document in any supported format using Node.js. Import and convert a document of any size."
type: docs
weight: 20
ai_search_scope: words_nodejs
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nodejs-net/supported-features-on-document-load/
aliases:
  - /nodejs/document-loading-overview/
  - /nodejs/supported-features-on-document-load/
timestamp: 2025-04-18-14-23-37
---

Aspose.Words strives to support all features for all supported formats. Almost all features of Microsoft Word documents are supported and are faithfully preserved during conversion. Using Aspose.Words you can load and convert a document of any size and can easily handle the conversion of a document consisting of thousands of pages within seconds. The only limitation is the amount of available working memory on the machine.

{{% alert color="primary" %}}

For more information and a description of the features available for the different formats, see the [Supported Features on Document Load](/words/net/supported-features-on-document-load/) section in the Aspose.Words for .NET documentation.

{{% /alert %}}

------ 

## FAQ

1. **Q:** Which file formats can be loaded with Aspose.Words for Node.js?  
   **A:** Aspose.Words can load all Microsoft Word formats (DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF) as well as OpenDocument (ODT, OTT), HTML, MHTML, EPUB, and plain text. The full list is available in the “Supported Features on Document Load” section of the .NET documentation.

2. **Q:** Are there any features that are not preserved when a document is loaded?  
   **A:** Almost every Word feature is preserved, but a few advanced items such as certain custom XML parts, macros, and some legacy WordArt may be lost or converted to a static representation. The documentation lists the exact limitations per format.

3. **Q:** What limits the size of a document that can be loaded?  
   **A:** The only practical limitation is the amount of RAM available on the host machine. Aspose.Words processes documents in memory, so very large files require sufficient memory; otherwise an `OutOfMemoryException` may be thrown.

4. **Q:** How do I apply a license when using Aspose.Words for Node.js?  
   **A:** Load the license file on the .NET side before creating any `Document` objects:  

   ```csharp
   Aspose.Words.License license = new Aspose.Words.License();
   license.SetLicense("Aspose.Words.lic");
   ```  

   The licensed .NET assembly is then used by the Node.js wrapper, and all features become fully enabled.

5. **Q:** Is Aspose.Words for Node.js compatible with .NET 8 and the latest Node.js versions?  
   **A:** Yes. The library follows the .NET Standard 2.0/2.1 specifications, making it compatible with .NET 8, .NET 6, and .NET Core. The Node.js wrapper works with current LTS releases of Node.js. Always use the latest NuGet package to benefit from the newest compatibility updates.