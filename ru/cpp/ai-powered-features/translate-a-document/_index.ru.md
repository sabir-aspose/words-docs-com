---
title: Перевести документ
second_title: Aspose.Words для C++
articleTitle: Перевести документ
linktitle: Перевести документ
type: docs
weight: 30
description: "Переведите документ. Aspose.Words для C++ упрощает перевод документов с помощью моделей Google AI, позволяя указать язык перевода."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ru/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Перевод документов - это часто необходимая опция в эпоху высокой цифровизации. Aspose.Words поддерживает перевод документов с использованием *Google* моделей генерирующего языка, что позволяет разработчикам переводить текстовое содержимое более чем на 300 языков.

Используйте метод [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) для перевода ваших документов на любой язык, представленный в списке [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/). Обратите внимание, что если исходный документ содержит несколько языков, модель, основанная на Google AI, сможет переводить все поддерживаемые языки. Если модель не сможет распознать язык в некоторых фрагментах текста, вам будет возвращен документ с этими непереведенными фрагментами и переведенным остальным текстом.

В следующем примере кода показано, как использовать модель *Gemini 1.5 Flash* в Aspose.Words для перевода документа на арабский язык:

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

Перевод документов с помощью Aspose.Words экономит время и упрощает интеграцию функций перевода в ваши проекты. Для получения дополнительной информации ознакомьтесь с документацией [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}