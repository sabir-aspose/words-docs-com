---
title: Using TrueType Fonts in C++
second_title: Aspose.Words for C++
articleTitle: Using TrueType Fonts
linktitle: Using TrueType Fonts
description: "Aspose.Words for C++ can find the right font or its suitable replacement for correct document rendering. This ensures that the difference between the displayed document and the original is minimal when there is not enough information about a font."
type: docs
weight: 20
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cpp/using-truetype-fonts/
timestamp: 2024-01-27-14-07-04
---

When working with documents, you often have to use different fonts, styles, and sizes. Documents can contain any number of fonts, which are not necessarily limited to the fonts that are installed in the operating system. The fonts can be completely different, such as fonts taken from other operating systems, purchased, or created by users themselves.

Sometimes, information about the fonts being used is embedded in the document, eliminating display problems during document transfer. In some other cases, only the font name is known, which does not guarantee that the document will look the same way on another computer. In this case, Aspose.Words can find the right font (or its suitable replacement, if the required font cannot be found) for correct rendering.

------ 

## FAQ

1. **Q:** How can I tell Aspose.Words for C++ where to look for TrueType fonts on a Linux machine?  
   **A:** Use the `FontSettings` class to add a folder that contains the required fonts. Create a `FontSettings` object, call `SetFontsFolder` with the path to the folder, and assign it to the `Document` via `SetFontSettings`. This makes the engine search the specified directory before falling back to system fonts.

2. **Q:** What should I do if a document references a font that is not installed on the target system?  
   **A:** Enable font substitution by configuring `FontSettings::set_SubstitutionSettings`. You can map the missing font name to an existing TrueType font using `SubstitutionSettings::get_TableSubstitution()->AddSubstitutes`. Aspose.Words will then render the document with the substitute font.

3. **Q:** Can I embed the original TrueType font into the output PDF or DOCX so that the document looks identical on any machine?  
   **A:** Yes. Set `FontSettings::set_EmbedTrueTypeFonts(true)` before saving. When the document is saved to PDF or DOCX, the engine will embed the used TrueType fonts, ensuring consistent rendering on machines that do not have those fonts installed.

4. **Q:** How do I load a font from a memory stream instead of a file path?  
   **A:** Create a `System::SharedPtr<Aspose::Words::FontSource>` from the byte array (e.g., `System::MakeObject<Aspose::Words::MemoryFontSource>(fontBytes)`) and add it to the `FontSettings::get_FontSources()` collection. This allows the engine to use fonts that are embedded in your application or downloaded at runtime.

```cpp
// Example: Set custom font folder and enable embedding
System::SharedPtr<Aspose::Words::FontSettings> fontSettings = System::MakeObject<Aspose::Words::FontSettings>();
fontSettings->SetFontsFolder(u"/usr/share/fonts/truetype", true);
fontSettings->set_EmbedTrueTypeFonts(true);

System::SharedPtr<Aspose::Words::Document> doc = System::MakeObject<Aspose::Words::Document>(u"input.docx");
doc->SetFontSettings(fontSettings);
doc->Save(u"output.pdf");
```