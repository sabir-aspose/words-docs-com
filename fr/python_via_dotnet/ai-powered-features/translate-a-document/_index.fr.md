---
title: Traduire un Document
second_title: Aspose.Words pour Python via .NET
articleTitle: Traduire un Document
linktitle: Traduire un Document
type: docs
weight: 30
description: "Traduire un document. Aspose.Words pour Python simplifie la traduction de documents à l'aide des modèles Google AI, vous permettant de spécifier la langue cible."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

La traduction de documents est une option fréquemment nécessaire à l'ère de la numérisation élevée. Aspose.Words prend en charge la traduction de documents à l'aide de *Google* modèles de langage génératifs, ce qui permet aux développeurs de traduire le contenu des textes dans plus de 300 langues.

Utilisez la méthode [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) pour traduire vos documents dans n'importe quelle langue représentée dans l'énumération [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). Notez que si le document source contient plusieurs langues, le modèle basé sur Google AI pourra traduire toutes les langues prises en charge. Si le modèle ne peut pas reconnaître la langue dans certains fragments de texte, alors vous recevrez un document avec ces fragments non traduits et avec le reste du texte traduit.

L'exemple de code suivant montre comment utiliser le modèle *Gemini 1.5 Flash* dans Aspose.Words pour traduire un document en arabe:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Traduire des documents avec Aspose.Words vous fait gagner du temps et facilite l'intégration des fonctionnalités de traduction dans vos projets. Pour plus d'informations, consultez la documentation [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}