---
title: AI перевірка граматики
second_title: Aspose.Words для C++
articleTitle: Перевірка граматики
linktitle: Перевірка граматики
type: docs
weight: 40
description: "Перевірте граматику документа. Aspose.Words для C++ дозволяє користувачам перевіряти граматику та виявляти помилки в документах за допомогою моделей OpenAI, Google та Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /uk/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Перевірка граматики в документах важлива для забезпечення ясності, професіоналізму та точності. Грамотно складені документи залишають позитивне враження і дозволяють уникнути непорозумінь. Перевірка граматики допомагає швидко виявляти та виправляти помилки, заощаджуючи час та покращуючи якість.

Aspose.Words дозволяє користувачам перевіряти граматику та виявляти помилки в документах, використовуючи сімейства моделей OpenAI, Google та Claude, перелічені у списку [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). Використовуйте метод [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), доступний у просторі імен [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** аналізує текст у документі та виявляє граматичні проблеми.

Наступний приклад коду показує, як використовувати модель GPT-4o mini в Aspose.Words для перевірки граматики:

{{< highlight cpp >}}
void AiGrammar()
{
    auto doc = MakeObject<Document>(MyDir + u"Big document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto grammarOptions = MakeObject<CheckGrammarOptions>();
    grammarOptions->set_ImproveStylistics(true);

    auto proofedDoc = model->CheckGrammar(doc, grammarOptions);
    proofedDoc->Save(ArtifactsDir + u"AI.AiGrammar.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Перевірка граматики за допомогою Aspose.Words покращує якість вашої роботи та полегшує впровадження коректури у ваші проекти. Для отримання додаткової інформації перегляньте документацію [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}