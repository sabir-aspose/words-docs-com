---
title: Traduire un Document
second_title: Aspose.Words pour C++
articleTitle: Traduire un Document
linktitle: Traduire un Document
type: docs
weight: 30
description: "Traduire un document. Aspose.Words pour C++ simplifie la traduction de documents à l'aide des modèles Google AI, vous permettant de spécifier la langue cible."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /fr/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

La traduction de documents est une option fréquemment nécessaire à l'ère de la numérisation élevée. Aspose.Words prend en charge la traduction de documents à l'aide de *Google* modèles de langage génératifs, ce qui permet aux développeurs de traduire le contenu des textes dans plus de 300 langues.

Utilisez la méthode [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) pour traduire vos documents dans n'importe quelle langue représentée dans l'énumération [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/). Notez que si le document source contient plusieurs langues, le modèle basé sur Google AI pourra traduire toutes les langues prises en charge. Si le modèle ne peut pas reconnaître la langue dans certains fragments de texte, alors vous recevrez un document avec ces fragments non traduits et avec le reste du texte traduit.

L'exemple de code suivant montre comment utiliser le modèle *Gemini 1.5 Flash* dans Aspose.Words pour traduire un document en arabe:

{{< highlight cpp >}}
void AiTranslate()
{
    auto doc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<GoogleAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto translatedDoc = model->Translate(doc, Language::Arabic);
    translatedDoc->Save(ArtifactsDir + u"AI.AiTranslate.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Traduire des documents avec Aspose.Words vous fait gagner du temps et facilite l'intégration des fonctionnalités de traduction dans vos projets. Pour plus d'informations, consultez la documentation [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}