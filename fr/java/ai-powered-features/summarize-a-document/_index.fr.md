---
title: Résumer un document
second_title: Aspose.Words pour Java
articleTitle: Résumer un document
linktitle: Résumer un document
type: docs
weight: 20
description: "Résumez un document. Aspose.Words pour Java simplifie la synthèse des documents à l'aide des modèles OpenAI et Google AI en vous permettant de spécifier la longueur du résumé."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/java/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

La synthèse des documents est un outil précieux pour l'examen du contenu, des informations rapides ou la préparation des résumés. Aspose.Words prend en charge la synthèse des documents à l'aide de modèles alimentés par AI, ce qui facilite le traitement du texte long. Cette fonctionnalité, disponible dans la fonctionnalité AI basée sur Aspose.Words, intègre des modèles de langage génératif avancés de *OpenAI* et *Google*, ainsi que des modèles de langage génératif anthropique *Claude's*. La liste des modèles pris en charge est disponible dans l'énumération [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/).

Vous pouvez spécifier diverses options pour résumer le contenu du document. Utilisez la méthode [Summarize](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#summarize-com.aspose.words.Document-com.aspose.words.SummarizeOptions) pour générer un résumé de votre document. Vous pouvez également définir la longueur du résumé à l'aide de la propriété [SummaryLength](https://reference.aspose.com/words/java/com.aspose.words/summarizeoptions/#getSummaryLength).

Avec Aspose.Words, la mise en œuvre de la synthèse des documents est simple. L'exemple de code suivant montre comment résumer un document à l'aide du modèle GPT-4o:

{{< highlight java >}}
Document firstDoc = new Document(getMyDir() + "Big document.docx");
 Document secondDoc = new Document(getMyDir() + "Document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI or Google generative language models.
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 Document oneDocumentSummary = model.summarize(firstDoc, new SummarizeOptions(); { oneDocumentSummary.setSummaryLength(SummaryLength.SHORT); });
 oneDocumentSummary.save(getArtifactsDir() + "AI.AiSummarize.One.docx");

 Document multiDocumentSummary = model.summarize(new Document[] { firstDoc, secondDoc }, new SummarizeOptions(); { multiDocumentSummary.setSummaryLength(SummaryLength.LONG); });
 multiDocumentSummary.save(getArtifactsDir() + "AI.AiSummarize.Multi.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Résumer des documents avec Aspose.Words vous fait gagner du temps et vous aide à vous concentrer sur les informations essentielles. Pour plus d'informations, vérifiez le [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}