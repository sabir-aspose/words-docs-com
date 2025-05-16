---
title: Узагальнення документа
second_title: Aspose.Words для C++
articleTitle: Узагальнення документа
linktitle: Узагальнення документа
type: docs
weight: 20
description: "Узагальніть документ. Aspose.Words для C++ спрощує Узагальнення документа за допомогою моделей OpenAI і Google AI, дозволяючи вказати довжину резюме."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /uk/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Узагальнення документів-це цінний інструмент для аналізу змісту, швидкого аналізу інформації або підготовки тез. Aspose.Words підтримує Узагальнення документів за допомогою моделей на основі AI, що полегшує обробку довгого тексту. Ця функція, доступна в просторі імен [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), поєднує розширені моделі генеративної мови з *OpenAI* та *Google*, а також антропні моделі генеративної мови *Claude's*. Список підтримуваних моделей доступний у списку [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

Ви можете вказати різні параметри для узагальнення вмісту документа. Використовуйте метод [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) для створення короткої інформації про ваш документ. Ви також можете задати довжину короткої інформації, використовуючи властивість [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

За допомогою Aspose.Words спрощується реалізація Узагальнення документа. Наступний приклад коду показує, як узагальнити документ за допомогою моделі GPT-4o.:

{{< highlight cpp >}}
void AiSummarize()
{
    auto firstDoc = MakeObject<Document>(MyDir + u"Big document.docx");
    auto secondDoc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"))->WithOrganization(u"Organization")->WithProject(u"Project");

    auto options = MakeObject<SummarizeOptions>();

    options->set_SummaryLength(SummaryLength::Short);
    auto firstDocumentSummary = model->Summarize(firstDoc, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.One.docx");

    System::ArrayPtr<System::SharedPtr<Document>> documents = System::MakeArray<System::SharedPtr<Document>>(2);
    documents[0] = firstDoc;
    documents[1] = secondDoc;

    options->set_SummaryLength(SummaryLength::Long);
    auto multiDocumentSummary = model->Summarize(documents, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.Multi.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Узагальнення документів за допомогою Aspose.Words економить час і допомагає зосередитися на важливій інформації. Для отримання додаткової інформації перегляньте документацію [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
