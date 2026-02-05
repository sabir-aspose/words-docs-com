---
title: Asian Typography in Java
second_title: Aspose.Words for Java
articleTitle: Working with Asian Typography
linktitle: Working with Asian Typography
description: "Work with Asian typography using Java. Adjust Space between Asian and Latin text in Java."
type: docs
weight: 240
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /java/working-with-asian-typography/
timestamp: 2024-01-27-14-07-04
---

Asian Typography is a set of options for text paragraphs in documents written in Asian languages.

Aspose.Words supports Asian Typography using the [ParagraphFormat](https://reference.aspose.com/words/net/aspose.words/paragraphformat/) class and some of its properties.

## Automatically Adjust Space between Asian and Latin Text or Numbers

If you are designing a template with both East Asian and Latin text and  want to enhance the appearance of your form template by controlling the spaces between both types of text, you can configure your form template to automatically adjust the spaces between these two types of text. To achieve this, you can use [AddSpaceBetweenFarEastAndAlpha](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getAddSpaceBetweenFarEastAndAlpha) and [AddSpaceBetweenFarEastAndDigit](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getAddSpaceBetweenFarEastAndDigit) properties of the `ParagraphFormat` class.

The following code example shows how to use **AddSpaceBetweenFarEastAndAlpha** and **AddSpaceBetweenFarEastAndDigit** properties:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkingWithParagraphs-DocumentBuilderSetSpaceBetweenAsianAndLatinText.java" >}}

## Set Line Break Options

The Asian Typography tab of the paragraph properties dialog box in Microsoft Word has line break group. The options of this group can be set using the [FarEastLineBreakControl](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getFarEastLineBreakControl), [WordWrap](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getWordWrap), [HangingPunctuation](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getHangingPunctuation) properties of the **ParagraphFormat** class.

The following code example shows how to use these properties:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkingWithParagraphs-SetAsianTypographyLinebreakGroupProp.java" >}}

## Change Asian Paragraph Spacing and Indents

The following code example shows how to change Asian paragraph spacing and indents:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkingWithParagraphs-ChangeAsianParagraphSpacingandIndents.java" >}}

------ 

## FAQ

1. **Q:** How can I enable automatic spacing between Asian characters and Latin letters or numbers?  
   **A:** Set `ParagraphFormat.AddSpaceBetweenFarEastAndAlpha` to `true` for spacing with Latin letters and `ParagraphFormat.AddSpaceBetweenFarEastAndDigit` to `true` for spacing with digits. These properties can be applied to a `Paragraph` or globally via a `DocumentBuilder`.

2. **Q:** Which properties control line‑break behavior for Asian text?  
   **A:** Use `ParagraphFormat.FarEastLineBreakControl` to prevent line breaks within Asian words, `ParagraphFormat.WordWrap` to enable/disable wrapping, and `ParagraphFormat.HangingPunctuation` to control hanging punctuation for East Asian scripts.

3. **Q:** How do I adjust spacing and indents specifically for Asian paragraphs?  
   **A:** Modify `ParagraphFormat.FirstLineIndent`, `LeftIndent`, `RightIndent`, and `SpaceAfter`/`SpaceBefore` while the `ParagraphFormat` is set to an Asian language context. The examples in this article demonstrate these settings.

4. **Q:** Are there any font considerations when working with Asian typography?  
   **A:** Aspose.Words uses the fonts installed on the system. Ensure the required CJK fonts (e.g., SimSun, MS Mincho) are available, or use `FontSettings` to load custom fonts so that Asian characters render correctly.

5. **Q:** Can I disable Asian typography features for a document that contains only Latin text?  
   **A:** Yes. Set the three properties (`AddSpaceBetweenFarEastAndAlpha`, `AddSpaceBetweenFarEastAndDigit`, `FarEastLineBreakControl`) to `false` or leave them at their default values; Aspose.Words will then treat the text as regular Latin script.