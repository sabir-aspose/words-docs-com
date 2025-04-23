---
title: Translate a Document
second_title: Aspose.Words for Python via .NET
articleTitle: Translate a Document
linktitle: Translate a Document
type: docs
weight: 30
description: "Translate a document. Aspose.Words for Python simplifies document translation using Google AI models, allowing you to specify the target language."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Document translation is a frequently needed option in the age of high digitalization. Aspose.Words supports document translation using *Google* generative language models, which allows developers to translate texts content into more than 300 languages.

Use the [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) method to translate your documents into any language represented in the [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) enumeration. Note that if the source document contains several languages, the Google AI-based model will be able to translate all supported languages. If the model cannot recognize the language in some text fragments, then you will be returned a document with these untranslated fragments and with the rest of the text translated.

The following code example shows how to use the *Gemini 1.5 Flash* model in Aspose.Words to translate a document into Arabic:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Translating documents with Aspose.Words saves time and makes it easy to integrate translation functionality into your projects. For more information, check the [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API documentation.

{{% /alert %}}