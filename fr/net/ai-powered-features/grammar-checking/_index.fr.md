---
title: AI Vérification grammaticale
second_title: Aspose.Words pour .NET
articleTitle: Vérification Grammaticale
linktitle: Vérification Grammaticale
type: docs
weight: 40
description: "Vérifiez la grammaire d'un document. Aspose.Words pour .NET permet aux utilisateurs de vérifier la grammaire et de détecter les erreurs dans les documents à l'aide de OpenAI modèles."
url: /fr/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

La vérification de la grammaire dans les documents est importante pour assurer la clarté, le professionnalisme et l'exactitude. Des documents bien écrits laissent une impression positive et évitent les malentendus. Les vérifications grammaticales aident à identifier et à corriger rapidement les erreurs, ce qui permet de gagner du temps et d'améliorer la qualité.

Aspose.Words permet aux utilisateurs de vérifier la grammaire et de détecter les erreurs dans les documents à l'aide de **OpenAI** modèles génératifs. Utilisez la méthode [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), disponible dans l'espace de noms [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/). **CheckGrammar** analyse le texte d'un document et met en évidence les problèmes grammaticaux.

L'exemple de code suivant montre comment utiliser le modèle GPT-4o mini dans Aspose.Words pour vérifier la grammaire:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Big document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use OpenAI generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gpt4OMini).WithApiKey(apiKey);

CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
grammarOptions.ImproveStylistics = true;

Document proofedDoc = model.CheckGrammar(doc, grammarOptions);
proofedDoc.Save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Vérifier la grammaire avec Aspose.Words améliore la qualité de votre travail et facilite l'intégration de la relecture dans vos projets. Pour plus d'informations, consultez la documentation [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}