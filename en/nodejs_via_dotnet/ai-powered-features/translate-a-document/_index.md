---
title: Translate a Document
second_title: Aspose.Words for Node.js via .NET
articleTitle: Translate a Document
linktitle: Translate a Document
type: docs
weight: 30
description: "Translate a document. Aspose.Words for Node.js via .NET simplifies document translation using AI models, allowing you to specify the target language."
ai_search_scope: nodejs_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nodejs-net/translate-a-document/
timestamp: 2025-05-16-12-00-00
---

Document translation is a frequently needed option in the age of high digitalization. Aspose.Words supports document translation using *Google*, *OpenAI* and *Anthropic* generative language models, which allows developers to translate texts content into more than 300 languages.

Use the [translate](https://reference.aspose.com/words/nodejs-net/aspose.words.ai/iaimodeltext/translate/) method to translate your documents into any language represented in the [Language](https://reference.aspose.com/words/nodejs-net/aspose.words.ai/language/) enumeration. Note that if the source document contains several languages, the AI-based model will be able to translate all supported languages. If the model cannot recognize the language in some text fragments, then you will be returned a document with these untranslated fragments and with the rest of the text translated.

The following code example shows how to use the *Gemini 1.5 Flash* model in Aspose.Words to translate a document into Arabic:

{{< gist "aspose-words-gists" "757cf7d3534a39730cf3290d418681ab" "ai-translate.js" >}}

{{% alert color="primary" %}}

Translating documents with Aspose.Words saves time and makes it easy to integrate translation functionality into your projects. For more information, check the [Aspose.Words.AI](https://reference.aspose.com/words/nodejs-net/aspose.words.ai/) API documentation.

{{% /alert %}}