---
title: AI Vérification grammaticale
second_title: Aspose.Words pour Java
articleTitle: Vérification Grammaticale
linktitle: Vérification Grammaticale
type: docs
weight: 40
description: "Vérifiez la grammaire d'un document. Aspose.Words pour Java permet aux utilisateurs de vérifier la grammaire et de détecter les erreurs dans les documents à l'aide des modèles OpenAI, Google et Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

La vérification de la grammaire dans les documents est importante pour assurer la clarté, le professionnalisme et l'exactitude. Des documents bien écrits laissent une impression positive et évitent les malentendus. Les vérifications grammaticales aident à identifier et à corriger rapidement les erreurs, ce qui permet de gagner du temps et d'améliorer la qualité.

Aspose.Words permet aux utilisateurs de vérifier la grammaire et de détecter les erreurs dans les documents en utilisant les familles de modèles OpenAI, Google et Claude répertoriées dans l'énumération [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). Utilisez la méthode [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) pour analyser le texte d'un document et mettre en évidence les problèmes grammaticaux.

L'exemple de code suivant montre comment utiliser le modèle GPT-4o mini dans Aspose.Words pour vérifier la grammaire:

{{< highlight java >}}
 Document doc = new Document("Big document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI generative language models.
 IAiModelText model = (OpenAiModel)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
 grammarOptions.setImproveStylistics(true);

 Document proofedDoc = model.checkGrammar(doc, grammarOptions);
 proofedDoc.save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Vérifier la grammaire avec Aspose.Words améliore la qualité de votre travail et facilite l'intégration de la relecture dans vos projets. Pour plus d'informations, vérifiez le [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}