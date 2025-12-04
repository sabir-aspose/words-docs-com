---
title: AI Проверка грамматики
second_title: Aspose.Words для C++
articleTitle: Проверка грамматики
linktitle: Проверка грамматики
type: docs
weight: 40
description: "Проверьте грамматику документа. Aspose.Words для C++ позволяет пользователям проверять грамматику и обнаруживать ошибки в документах, используя модели OpenAI, Google и Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ru/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Проверка грамматики в документах важна для обеспечения ясности, профессионализма и точности. Грамотно составленные документы оставляют положительное впечатление и позволяют избежать недоразумений. Проверка грамматики помогает быстро выявлять и исправлять ошибки, экономя время и повышая качество.

Aspose.Words позволяет пользователям проверять грамматику и обнаруживать ошибки в документах, используя семейства моделей OpenAI, Google и Claude, перечисленные в списке [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). Используйте метод [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), доступный в пространстве имен [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** анализирует текст в документе и выявляет грамматические проблемы.

В следующем примере кода показано, как использовать модель GPT-4o mini в Aspose.Words для проверки грамматики:

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

Проверка грамматики с помощью Aspose.Words повышает качество вашей работы и упрощает внедрение корректуры в ваши проекты. Для получения дополнительной информации ознакомьтесь с документацией [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}