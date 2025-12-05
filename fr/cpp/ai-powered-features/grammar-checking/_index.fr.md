---
title: AI Vérification grammaticale
second_title: Aspose.Words pour C++
articleTitle: Vérification Grammaticale
linktitle: Vérification Grammaticale
type: docs
weight: 40
description: "Vérifiez la grammaire d'un document. Aspose.Words pour C++ permet aux utilisateurs de vérifier la grammaire et de détecter les erreurs dans les documents à l'aide des modèles OpenAI, Google et Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

La vérification de la grammaire dans les documents est importante pour assurer la clarté, le professionnalisme et l'exactitude. Des documents bien écrits laissent une impression positive et évitent les malentendus. Les vérifications grammaticales aident à identifier et à corriger rapidement les erreurs, ce qui permet de gagner du temps et d'améliorer la qualité.

Aspose.Words permet aux utilisateurs de vérifier la grammaire et de détecter les erreurs dans les documents en utilisant les familles de modèles OpenAI, Google et Claude répertoriées dans l'énumération [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). Utilisez la méthode [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), disponible dans l'espace de noms [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** analyse le texte d'un document et met en évidence les problèmes grammaticaux.

L'exemple de code suivant montre comment utiliser le modèle GPT-4o mini dans Aspose.Words pour vérifier la grammaire:

{{< highlight cpp >}}
void AiGrammar()
{
    auto doc = MakeObject<Document>(MyDir + u"Big document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto grammarOptions = MakeObject<CheckGrammarOptions>();
    grammarOptions->set_ImproveStylistics(true);

    auto proofedDoc = model->CheckGrammar(doc, grammarOptions);
    proofedDoc->Save(ArtifactsDir + u"AI.AiGrammar.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Vérifier la grammaire avec Aspose.Words améliore la qualité de votre travail et facilite l'intégration de la relecture dans vos projets. Pour plus d'informations, consultez la documentation [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}