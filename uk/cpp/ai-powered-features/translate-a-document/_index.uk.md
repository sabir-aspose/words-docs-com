---
title: Перекласти документ
second_title: Aspose.Words для C++
articleTitle: Перекласти документ
linktitle: Перекласти документ
type: docs
weight: 30
description: "Перекладіть документ. Aspose.Words для C++ спрощує Переклад документів за допомогою моделей Google AI, дозволяючи вказати мову перекладу."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Переклад документів-це часто необхідна опція в епоху високої цифровізації. Aspose.Words підтримує Переклад документів за допомогою *Google* моделей генеруючої мови, що дозволяє розробникам перекладати текстовий вміст більш ніж на 300 мов.

Використовуйте метод [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) для перекладу документів будь-якою мовою, представленою у списку [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/). Зверніть увагу, що якщо оригінальний документ містить кілька мов, модель, заснована на Google AI, зможе перекласти всі підтримувані мови. Якщо модель не зможе розпізнати мову в деяких фрагментах тексту, Вам буде повернуто документ із цими неперекладеними фрагментами та перекладеним рештою тексту.

Наступний приклад коду показує, як використовувати модель *Gemini 1.5 Flash* в Aspose.Words для перекладу документа на арабську мову:

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

Переклад документів за допомогою Aspose.Words економить час та полегшує інтеграцію функцій перекладу у ваші проекти. Для отримання додаткової інформації перегляньте документацію [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}