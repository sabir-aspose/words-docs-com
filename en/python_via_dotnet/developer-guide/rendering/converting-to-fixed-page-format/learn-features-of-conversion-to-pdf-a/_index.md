---
title: Conversion to PDF/A and PDF/UA
second_title: Aspose.Words for Python via .NET
articleTitle: Learn Features of Conversion to PDF/A and PDF/UA
linktitle: Learn Features of Conversion to PDF/A and PDF/UA
description: "Convert to PDF/A-1, PDF/A-2, PDF/A-4 and PDF/UA using Python. Choose the best PDF standard to convert a document using Python via .NET."
type: docs
weight: 25
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/learn-features-of-conversion-to-pdf-a/
aliases: [/python/learn-features-of-conversion-to-pdf-a/]
timestamp: 2024-01-31-14-23-37
---

PDF is a fixed page format that is very popular among users and is widely supported by various applications, as a PDF document looks the same on any device. For this reason, converting to PDF is an important feature of Aspose.Words.

PDF is a complex format by itself, as it has a specific file structure, graphical model, font embedding, and some complex output functionality such as document structure tags, encryption, digital signatures, and editable forms. In addition, converting a document to PDF requires several calculation stages, which are complex and time‑consuming.

In this section, we will consider the main problems that may arise when working with documents in various PDF standards and describe options for solving them.

## Which PDF Standard Aspose.Words Supports

Aspose.Words now allows users to work with PDF/A-1, PDF/A-2 and PDF/A-4 formats, as well as PDF/UA-1:

- PDF/A-1 has serious limitations such as transparency and some compression options are prohibited
- PDF/A-2 eliminates some of the limitations of PDF/A-1, such as support of transparency and layer effects or embedding of OpenType fonts
- PDF/A-4 assumes revised conformance levels: regular PDF/A-4 conformance is equivalent to previous versions' level U conformance, and the level A conformance is removed
- PDF/UA-1 content should be tagged and standardized according to ISO 32000-1: 2008

PDF/A is an ISO‑standardized version of PDF intended for use in archiving and long‑term storage of electronic documents. At the same time, PDF/UA is another ISO standardized version of PDF designed to ensure accessibility for people with disabilities who use assistive technology. To specify the level of compliance with PDF standards, use the [PdfSaveOptions.compliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/compliance/) property. Due to storage conditions, PDF/A document must embed all fonts and disable encryption, while PDF/UA must only embed all fonts.

In this section, we will take a closer look at working with PDF/A or PDF/UA-1 documents.

## Relevant ISO for PDF Standards

To learn more about the different PDF standards, check the following ISOs:

- PDF 1.7 = ISO-32000-1: 2008
- PDF 2.0 = ISO-32000-2: 2020
- PDF/A-1 = ISO-19005-1: 2005
- PDF/A-2 = ISO-19005-2: 2011
- PDF/A-4 = ISO-19005-4: 2020
- PDF/UA-1 = ISO-14289: 2014

## See Also

* [How to edit document structure tags in Adobe Acrobat](https://helpx.adobe.com/acrobat/using/editing-document-structure-content-tags.html)
* [How to check or edit text language in Microsoft Word](https://support.microsoft.com/en-us/office/check-spelling-and-grammar-in-a-different-language-667ba67a-a202-42fd-8596-edc1fa320e00)
* [How to change text language in Adobe Acrobat](https://helpx.adobe.com/acrobat/using/editing-document-structure-content-tags.html#add_alternate_text_and_supplementary_information_to_tags)
* [How to add alternative text to a shape, picture, chart, SmartArt graphic, or other object in Microsoft Word](https://support.microsoft.com/en-us/office/add-alternative-text-to-a-shape-picture-chart-smartart-graphic-or-other-object-44989b2a-903c-4d9a-b742-6a75b451c669)
* [How to add alternate text and supplementary information to tags](https://helpx.adobe.com/acrobat/using/create-verify-pdf-accessibility.html) (or read the same information in the [Adobe Acrobat User Guide](https://helpx.adobe.com/acrobat/using/editing-document-structure-content-tags.html#add_alternate_text_and_supplementary_information_to_tags))
* [How to set up ActualText entry for text](https://helpx.adobe.com/acrobat/using/create-verify-pdf-accessibility.html), the “Add Actual Text for an Abbreviated Term, Formula, or Non‑Unicode Symbol” section
* [Unicode mapping for common Windows symbolic fonts](http://www.alanwood.net/demos/webdings.html)

------ 

## Troubleshoot

1. **Problem:** Conversion to PDF/A fails with an error about missing fonts.  
   **Solution:** Ensure the required fonts are installed on the machine running the conversion, or provide a custom font source by setting `options.custom_font_sources`. Also verify that `options.embed_full_fonts` is set to `True` so Aspose.Words embeds the fonts automatically.

2. **Problem:** The generated PDF/A file is rejected because it is encrypted.  
   **Solution:** Remove any encryption settings before saving. When using PDF/A compliance, do not set `options.encrypt` or any `PdfEncryptionOptions`. If encryption is required for a non‑PDF/A PDF, use a different compliance level.

3. **Problem:** Transparency in images causes the PDF/A‑1 conversion to produce a blank page.  
   **Solution:** Either change the compliance to PDF/A‑2 (`PdfCompliance.PdfA2b`) which permits transparency, or rasterize/flatten the transparent objects in the source document (e.g., convert them to PNG without alpha channel).

4. **Problem:** PDF/UA output is missing document structure tags, resulting in accessibility warnings.  
   **Solution:** Verify that the source Word document uses proper heading styles, alt text, and language attributes. Aspose.Words copies these tags only when they exist. If necessary, add them programmatically using `DocumentBuilder` before saving.

5. **Problem:** The conversion process is extremely slow for large documents.  
   **Solution:** Reduce the workload by disabling unnecessary features such as digital signatures (`options.digital_signature = None`) and by using `options.optimize_output = True`. Also ensure the machine has sufficient memory and that font caching is enabled.