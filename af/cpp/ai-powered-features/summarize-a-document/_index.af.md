---
title: Som'n Dokument op
second_title: Aspose.Words vir C++
articleTitle: Som'n Dokument op
linktitle: Som'n Dokument op
type: docs
weight: 20
description: "Som'n dokument op. Aspose.Words vir C++ vereenvoudig dokumentopsomming met behulp van OpenAI en Google AI modelle deur jou toe te laat om die opsommingslengte te spesifiseer."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /af/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Die opsomming van dokumente is'n waardevolle hulpmiddel vir inhoudhersiening, vinnige insigte of die voorbereiding van opsommings. Aspose.Words ondersteun dokumentopsomming met behulp van AI-aangedrewe modelle, wat dit makliker maak om lang teks te verwerk. Hierdie funksie, beskikbaar in die [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) naamruimte, integreer gevorderde generatiewe taalmodelle van *OpenAI* en *Google*, sowel as *Claude's* antropiese generatiewe taalmodelle. Die lys van ondersteun modelle is beskikbaar in die [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/) opsomming.

U kan verskeie opsies spesifiseer vir die opsomming van dokumentinhoud. Gebruik die [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) metode om'n opsomming van jou dokument te genereer. Jy kan ook opsommingslengte stel deur die [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/) eienskap te gebruik.

Met Aspose.Words is die implementering van dokumentopsomming eenvoudig. Die volgende kode voorbeeld toon hoe om'n dokument te som met behulp van GPT-4o model:

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

Die opsomming van dokumente met Aspose.Words bespaar tyd en help u om op noodsaaklike inligting te fokus. Vir meer inligting, kyk na die [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API dokumentasie.

{{% /alert %}}
