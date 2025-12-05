---
title: AI Проверка На Граматиката
second_title: Aspose.Words за C++
articleTitle: Проверка На Граматиката
linktitle: Проверка На Граматиката
type: docs
weight: 40
description: "Проверете граматиката на документа. Aspose.Words за C++ позволява на потребителите да проверяват граматиката и да откриват грешки в документи, използвайки модели OpenAI, Гугъл и Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Проверката на граматиката в документите е важна, за да се гарантира яснота, професионализъм и точност. Добре написаните документи оставят положително впечатление и избягват недоразумения. Проверките на граматиката помагат бързо да се идентифицират и коригират грешките, спестявайки време и подобрявайки качеството.

Aspose.Words позволява на потребителите да проверяват граматиката и да откриват грешки в документите, като използват семействата на моделите OpenAI, Гугъл и Claude, изброени в [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). Използвайте метода [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), Наличен в пространство от имена [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** анализира текста в документ и подчертава граматическите проблеми.

Следващият пример за код показва как да използвате модела GPT-4o mini в Aspose.Words, за да проверите граматиката:

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

Проверката на граматиката с Aspose.Words подобрява качеството на работата ви и улеснява интегрирането на корекцията във вашите проекти. За повече информация вижте документацията [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}