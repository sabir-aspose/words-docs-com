---
title: Traduire un document
second_title: Aspose.Words pour .NET
articleTitle: Traduire un document
linktitle: Traduire un document
type: docs
weight: 30
description: "Traduire un document. Aspose.Words pour .NET simplifie la traduction de documents à l'aide de modèles d'IA de Google, vous permettant de spécifier la langue cible."
url: /fr/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

La traduction de documents est une option fréquemment nécessaire à l'ère de la numérisation élevée. Aspose.Words prend en charge la traduction de documents à l'aide de modèles de langage génératifs *Google*, qui permettent aux développeurs de traduire le contenu des textes dans plus de 300 langues.

Utilisez la méthode [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) pour traduire vos documents dans n'importe quelle langue représentée dans l'énumération [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Notez que si le document source contient plusieurs langues, le modèle basé sur l'IA de Google sera capable de traduire toutes les langues prises en charge. Si le modèle ne peut pas reconnaître la langue dans certains fragments de texte, vous recevrez un document contenant ces fragments non traduits et le reste du texte traduit.

L'exemple de code suivant montre comment utiliser le modèle *Gemini 1.5 Flash* dans Aspose.Words pour traduire un document en arabe :

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

La traduction de documents avec Aspose.Words permet de gagner du temps et d'intégrer facilement la fonctionnalité de traduction dans vos projets. Pour plus d'informations, consultez la documentation de l'API [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).
{{% /alert %}}