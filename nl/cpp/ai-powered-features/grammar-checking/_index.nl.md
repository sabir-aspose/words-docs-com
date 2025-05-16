---
title: AI Grammaticacontrole
second_title: Aspose.Words voor C++
articleTitle: Grammaticacontrole
linktitle: Grammaticacontrole
type: docs
weight: 40
description: "Controleer de grammatica van een document. Aspose.Words voor C++ hiermee kunnen gebruikers grammatica controleren en fouten in documenten detecteren met behulp van OpenAI, Google en Claude modellen."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nl/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Het controleren van grammatica in documenten is belangrijk om duidelijkheid, professionaliteit en nauwkeurigheid te garanderen. Goed geschreven documenten laten een positieve indruk achter en voorkomen misverstanden. Grammaticacontroles helpen fouten snel te identificeren en te corrigeren, waardoor tijd wordt bespaard en de kwaliteit wordt verbeterd.

Aspose.Words stelt gebruikers in staat om grammatica te controleren en fouten in documenten te detecteren met behulp van de families van de OpenAI, Google en Claude modellen die in de [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/) - opsomming worden vermeld. Gebruik de methode [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), Beschikbaar in de [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) naamruimte. **CheckGrammar** analyseert de tekst in een document en wijst op grammaticale problemen.

Het volgende codevoorbeeld laat zien hoe u het GPT-4o mini model in Aspose.Words gebruikt om grammatica te controleren:

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

Het controleren van grammatica met Aspose.Words verbetert de kwaliteit van uw werk en maakt het gemakkelijk om proeflezen in uw projecten te integreren. Raadpleeg de [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API documentatie voor meer informatie.

{{% /alert %}}