---
title: Een Document samenvatten
second_title: Aspose.Words voor C++
articleTitle: Een Document samenvatten
linktitle: Een Document samenvatten
type: docs
weight: 20
description: "Een document samenvatten. Aspose.Words voor C++ vereenvoudigt het samenvatten van documenten met behulp van OpenAI - en Google AI - modellen door u in staat te stellen de lengte van de samenvatting op te geven."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nl/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Het samenvatten van documenten is een waardevol hulpmiddel voor het beoordelen van inhoud, Snelle inzichten of het opstellen van samenvattingen. Aspose.Words ondersteunt documentsamenvatting met behulp van AI-aangedreven modellen, waardoor het gemakkelijker wordt om lange tekst te verwerken. Deze functie, beschikbaar in de [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) naamruimte, integreert geavanceerde generatieve taalmodellen van *OpenAI* en *Google*, evenals *Claude's* antropische generatieve taalmodellen. De lijst met ondersteunde modellen is beschikbaar in de [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/) - opsomming.

U kunt verschillende opties opgeven voor het samenvatten van documentinhoud. Gebruik de methode [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) om een samenvatting van uw document te genereren. U kunt ook de lengte van de samenvatting instellen met de eigenschap [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

Met Aspose.Words is het implementeren van documentsamenvatting eenvoudig. Het volgende codevoorbeeld laat zien hoe u een document samenvat met behulp van GPT-4o model:

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

Het samenvatten van documenten met Aspose.Words bespaart tijd en helpt u zich te concentreren op essentiële informatie. Raadpleeg de [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API documentatie voor meer informatie.

{{% /alert %}}
