---
title: AI Grammatika-Kontrole
second_title: Aspose.Words vir C++
articleTitle: Grammatika-Kontrole
linktitle: Grammatika-Kontrole
type: docs
weight: 40
description: "Gaan'n dokumentgrammatika na. Aspose.Words vir C++ laat gebruikers toe om grammatika te kontroleer en foute in dokumente op te spoor met behulp van OpenAI, Google en Claude modelle."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /af/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Dit is belangrik om grammatika in dokumente te kontroleer om duidelikheid, professionaliteit en akkuraatheid te verseker. Goedgeskrewe dokumente laat'n positiewe indruk en vermy misverstande. Grammatika-kontroles help om foute vinnig te identifiseer en reg te stel, wat tyd bespaar en kwaliteit verbeter.

Aspose.Words laat gebruikers toe om grammatika te kontroleer en foute in dokumente op te spoor deur die OpenAI, Google en Claude modelle se families te gebruik wat in die [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/) opsomming gelys word. Gebruik die [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/) metode, beskikbaar in die [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) naamruimte. **CheckGrammar** ontleed die teks in'n dokument en beklemtoon grammatikale probleme.

Die volgende kode voorbeeld toon hoe om die GPT-4o mini model in Aspose.Words te gebruik om grammatika te kontroleer:

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

Die nagaan van grammatika met Aspose.Words verbeter die kwaliteit van u werk en maak dit maklik om proeflees in u projekte te integreer. Vir meer inligting, kyk na die [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API dokumentasie.

{{% /alert %}}