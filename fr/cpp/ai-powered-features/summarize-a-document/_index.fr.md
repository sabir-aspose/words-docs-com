---
title: Résumer un document
second_title: Aspose.Words pour C++
articleTitle: Résumer un document
linktitle: Résumer un document
type: docs
weight: 20
description: "Résumez un document. Aspose.Words pour C++ simplifie la synthèse des documents à l'aide des modèles OpenAI et Google AI en vous permettant de spécifier la longueur du résumé."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

La synthèse des documents est un outil précieux pour l'examen du contenu, des informations rapides ou la préparation des résumés. Aspose.Words prend en charge la synthèse des documents à l'aide de modèles alimentés par AI, ce qui facilite le traitement du texte long. Cette fonctionnalité, disponible dans l'espace de noms [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), intègre des modèles de langage génératif avancés de *OpenAI* et *Google*, ainsi que des modèles de langage génératif anthropique *Claude's*. La liste des modèles pris en charge est disponible dans l'énumération [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

Vous pouvez spécifier diverses options pour résumer le contenu du document. Utilisez la méthode [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) pour générer un résumé de votre document. Vous pouvez également définir la longueur du résumé à l'aide de la propriété [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

Avec Aspose.Words, la mise en œuvre de la synthèse des documents est simple. L'exemple de code suivant montre comment résumer un document à l'aide du modèle GPT-4o:

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

Résumer des documents avec Aspose.Words vous fait gagner du temps et vous aide à vous concentrer sur les informations essentielles. Pour plus d'informations, consultez la documentation [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
