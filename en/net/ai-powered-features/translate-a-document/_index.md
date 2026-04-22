---
title: Translate a Document
second_title: Aspose.Words for .NET
articleTitle: Translate a Document
linktitle: Translate a Document
type: docs
weight: 30
description: "Translate a document. Aspose.Words for .NET simplifies document translation using Google AI models, allowing you to specify the target language."
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

{{% alert color="grey" %}}

## Purpose Summary

This page explains how to translate a document using Aspose.Words and describes available translation workflows.

{{% /alert %}}

Document translation is a frequently needed option in the age of high digitalization. Aspose.Words supports document translation using *Google* generative language models, which allows developers to translate texts content into more than 300 languages.

Use the [Translate](https://reference.aspose.com/words/net/aspose.words.ai/aimodel/translate/) method to translate your documents into any language represented in the [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) enumeration. Note that if the source document contains several languages, the Google AI-based model will be able to translate all supported languages. If the model cannot recognize the language in some text fragments, then you will be returned a document with these untranslated fragments and with the rest of the text translated.

The following code example shows how to use the *Gemini 1.5 Flash* model in Aspose.Words to translate a document into Arabic:

{{< gist "aspose-words-gists" "ea14b3e44c0233eecd663f783a21c4f6" "ai-translate.cs" >}}

{{% alert color="primary" %}}

Translating documents with Aspose.Words saves time and makes it easy to integrate translation functionality into your projects. For more information, check the [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API documentation.

{{% /alert %}}

## Related APIs

------

## FAQ

1. **Q:** Which languages can be translated with Aspose.Words AI?  
   **A:** The translation feature uses Google generative language models, which support more than 300 languages. Any language listed in the `Language` enumeration can be specified as the target language.

2. **Q:** Do I need an internet connection to translate a document?  
   **A:** Yes. The translation request is sent to Google’s AI service, so a network connection is required for the `Translate` method to work.

3. **Q:** Can I translate only a part of a document, such as a single section or paragraph?  
   **A:** The `Translate` method works on the whole document. To translate only a portion, extract the desired nodes into a separate `Document` object, call `Translate`, and then replace the original nodes with the translated content.

4. **Q:** What happens if the source document contains multiple languages?  
   **A:** The AI model attempts to detect each language segment and translate it to the target language. Segments that cannot be recognized will remain untranslated, while the rest of the document will be translated.