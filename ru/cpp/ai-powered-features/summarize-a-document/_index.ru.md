---
title: Обобщение документа
second_title: Aspose.Words для C++
articleTitle: Обобщение документа
linktitle: Обобщение документа
type: docs
weight: 20
description: "Обобщите документ. Aspose.Words для C++ упрощает обобщение документа с помощью моделей OpenAI и Google AI, позволяя указать длину резюме."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ru/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Обобщение документов - это ценный инструмент для анализа содержания, быстрого анализа информации или подготовки тезисов. Aspose.Words поддерживает обобщение документов с использованием моделей, основанных на AI, что упрощает обработку длинного текста. Эта функция, доступная в пространстве имен [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), объединяет расширенные модели порождающего языка из *OpenAI* и *Google*, а также антропные модели порождающего языка *Claude's*. Список поддерживаемых моделей доступен в списке [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

Вы можете указать различные параметры для обобщения содержимого документа. Используйте метод [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) для создания краткой информации о вашем документе. Вы также можете задать длину краткой информации, используя свойство [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

С помощью Aspose.Words упрощается реализация обобщения документа. В следующем примере кода показано, как обобщить документ, используя модель GPT-4o.:

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

Обобщение документов с помощью Aspose.Words экономит время и помогает сосредоточиться на важной информации. Для получения дополнительной информации ознакомьтесь с документацией [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
