---
title: Font Manipulation and Performance Issues in C++
second_title: Aspose.Words for C++
articleTitle: Font Manipulation and Performance Issues
linktitle: Font Manipulation and Performance Issues
description: "Aspose.Words for C++ uses font full name, family name, version, style to find the required font data or a suitable replacement for the requested font. FontSettings allows you to speed up the loading of the documents."
type: docs
weight: 11
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cpp/font-manipulation-and-performance-issues/
timestamp: 2024-09-24-14-35-44
---

All available font manipulation mechanisms are contained in the [FontSettings](https://reference.aspose.com/words/cpp/class/aspose.words.fonts.font_settings) class. This class is responsible for fetching fonts within defined font sources as well as for the Font Substitution process, as described below.

## Parsing the Resolved Fonts

Fonts are parsed in several steps:

1. Obtaining info for font, resolving from all available fonts.  
2. Parsing the resolved fonts to get available glyphs and metrics (horizontal and vertical).  
3. Parsing the resolved fonts for embedding and subsetting.

When Aspose.Words encounters a font in the document for the first time, it attempts to obtain basic font information, such as the font full name, family name, version, style, from the font files located in each font source. After all the fonts are retrieved, Aspose.Words uses these details to find the required font data or a suitable replacement for the requested font.

## Performance Issue When Replacing Fonts

Since the procedure described above is time‑consuming, it may negatively affect application performance at its first launch. However, each instance of **FontSettings** has its own cache, which could reduce the processing time of subsequent documents. For example, you can share an instance of the **FontSettings** class between different documents, which allows you to speed up the loading of the documents. The following example demonstrates this:

{{< gist "aspose-words-gists" "d55d8631947d283b1f0da99afa06c492" "cpp-Rendering-Printing-WorkingWithFontSettings-FontSettingsWithLoadOptions.cpp" >}}

In the case when **FontSettings** is not defined explicitly, Aspose.Words uses the default **FontSettings** instance. This instance is also automatically shared among documents, and can be extracted as follows:

**C++**

{{< highlight cpp >}}
System::SharedPtr<FontSettings> fontSettings = System::MakeObject<FontSettings>()->get_DefaultInstance();
{{< /highlight >}}

## Using the Default FontSettings Instance

If you are sure that all processing documents require the same font settings, then it is recommended to set up and utilize the default **FontSettings** instance. Suppose that you need to use the same font sources for all your documents. In this case, you can just amend the default instance as follows:

{{< gist "aspose-words-gists" "d55d8631947d283b1f0da99afa06c492" "cpp-Rendering-Printing-WorkingWithFontSettings-FontSettingsFontSource.cpp" >}}

{{% alert color="primary" %}}
The custom **FontSettings** have higher priority than the default instance.
{{% /alert %}}

------  

## FAQ

1. **Q:** How can I share a single `FontSettings` instance across multiple documents to improve loading performance?  
   **A:** Create one `FontSettings` object, configure it (e.g., add font sources), and assign it to each `Document` via `Document::set_FontSettings`. Because the instance maintains its own cache, subsequent documents will reuse the already‑resolved fonts, reducing the time spent on font parsing.

2. **Q:** How do I access and modify the default `FontSettings` instance in C++?  
   **A:** The default instance can be obtained with `FontSettings::get_DefaultInstance()`. You can then call methods such as `AddFontSource` or `SetSubstitutionSettings` on the returned object, and all documents that rely on the default instance will automatically use the updated configuration.

3. **Q:** How can I add a custom folder as a font source for `FontSettings`?  
   **A:** Use `System::SharedPtr<FolderFontSource> folderSource = System::MakeObject<FolderFontSource>(u"/path/to/fonts", true);` and then add it to the settings with `fontSettings->AddFontSource(folderSource);`. Setting the second parameter to `true` enables recursive search of sub‑folders.

4. **Q:** Is there a way to clear the internal font cache if I change font sources at runtime?  
   **A:** Yes. Call `fontSettings->ClearCache();` after modifying the font sources. This forces Aspose.Words to re‑scan the sources the next time a document requests a font, ensuring the new fonts are taken into account.

5. **Q:** How does `FontSettings` affect font substitution, and can I control which fonts are used as substitutes?  
   **A:** `FontSettings` performs substitution based on the resolved font’s full name, family name, style, etc. You can customize substitution rules via `fontSettings->get_SubstitutionSettings()->AddSubstitutes(u"Arial", System::MakeArray<System::String>({ u"Helvetica", u"FreeSans" }));`. This tells Aspose.Words to prefer the listed fonts when the original font is unavailable.