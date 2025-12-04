---
title: Translate a Document
second_title: Aspose.Words for C++
articleTitle: Translate a Document
linktitle: Translate a Document
type: docs
weight: 30
description: "Translate a document. Aspose.Words for C++ simplifies document translation using Google AI models, allowing you to specify the target language."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Document translation is a frequently needed option in the age of high digitalization. Aspose.Words supports document translation using *Google* generative language models, which allows developers to translate texts content into more than 300 languages.

Use the [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) method to translate your documents into any language represented in the [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) enumeration. Note that if the source document contains several languages, the Google AI-based model will be able to translate all supported languages. If the model cannot recognize the language in some text fragments, then you will be returned a document with these untranslated fragments and with the rest of the text translated.

The following code example shows how to use the *Gemini 1.5 Flash* model in Aspose.Words to translate a document into Arabic:

{{< highlight cpp >}}
void AiTranslate()
{
    auto doc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<GoogleAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto translatedDoc = model->Translate(doc, Language::Arabic);
    translatedDoc->Save(ArtifactsDir + u"AI.AiTranslate.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Translating documents with Aspose.Words saves time and makes it easy to integrate translation functionality into your projects. For more information, check the [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API documentation.

{{% /alert %}}