---
title: Traduire un Document
second_title: Aspose.Words pour Java
articleTitle: Traduire un Document
linktitle: Traduire un Document
type: docs
weight: 30
description: "Traduire un document. Aspose.Words pour Java simplifie la traduction de documents à l'aide des modèles Google AI, vous permettant de spécifier la langue cible."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

La traduction de documents est une option fréquemment nécessaire à l'ère de la numérisation élevée. Aspose.Words prend en charge la traduction de documents à l'aide de *Google* modèles de langage génératifs, ce qui permet aux développeurs de traduire le contenu des textes dans plus de 300 langues.

Utilisez la méthode [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) pour traduire vos documents dans n'importe quelle langue représentée dans l'énumération [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). Notez que si le document source contient plusieurs langues, le modèle basé sur Google AI pourra traduire toutes les langues prises en charge. Si le modèle ne peut pas reconnaître la langue dans certains fragments de texte, alors vous recevrez un document avec ces fragments non traduits et avec le reste du texte traduit.

L'exemple de code suivant montre comment utiliser le modèle *Gemini 1.5 Flash* dans Aspose.Words pour traduire un document en arabe:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Traduire des documents avec Aspose.Words vous fait gagner du temps et facilite l'intégration des fonctionnalités de traduction dans vos projets. Pour plus d'informations, vérifiez le [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}