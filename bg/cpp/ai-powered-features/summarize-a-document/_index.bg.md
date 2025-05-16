---
title: Обобщаване на документ
second_title: Aspose.Words за C++
articleTitle: Обобщаване на документ
linktitle: Обобщаване на документ
type: docs
weight: 20
description: "Обобщете документ. Aspose.Words за C++ опростява обобщаването на документи, използвайки модели OpenAI и Гугъл AI, като ви позволява да зададете дължината на резюмето."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /bg/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Обобщаването на документи е ценен инструмент за преглед на съдържанието, бързи прозрения или изготвяне на резюмета. Aspose.Words поддържа обобщаване на документи, използвайки AI - захранвани модели, което улеснява обработката на дълъг текст. Тази функция, налична в [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) пространство от имена, интегрира съвременни генеративни езикови модели от *OpenAI* и *Google*, както и *Claude's* антропни генеративни езикови модели. Списъкът с поддържаните модели е достъпен в списъка [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

Можете да зададете различни опции за обобщаване на съдържанието на документа. Използвайте метода [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/), за да генерирате резюме на вашия документ. Можете също да зададете дължина на резюмето, като използвате свойството [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

При Aspose.Words обобщаването на документа е лесно. Следващият пример за код показва как да обобщите документ, като използвате модел GPT-4o:

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

Обобщаването на документи с Aspose.Words спестява време и Ви помага да се съсредоточите върху основната информация. За повече информация вижте документацията [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
