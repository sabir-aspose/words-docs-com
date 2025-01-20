---
title: AI Grammatika-Kontrole
second_title: Aspose.Words vir .NET
articleTitle: Grammatika-Kontrole
linktitle: Grammatika-Kontrole
type: docs
weight: 40
description: "Gaan'n dokumentgrammatika na. Aspose.Words vir .NET laat gebruikers toe om grammatika te kontroleer en foute in dokumente op te spoor met behulp van OpenAI modelle."
url: /af/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Dit is belangrik om grammatika in dokumente te kontroleer om duidelikheid, professionaliteit en akkuraatheid te verseker. Goedgeskrewe dokumente laat'n positiewe indruk en vermy misverstande. Grammatika-kontroles help om foute vinnig te identifiseer en reg te stel, wat tyd bespaar en kwaliteit verbeter.

Aspose.Words laat gebruikers toe om grammatika te kontroleer en foute in dokumente op te spoor met behulp van **OpenAI** generatiewe modelle. Gebruik die [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/) metode, beskikbaar in die [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) naamruimte. **CheckGrammar** ontleed die teks in'n dokument en beklemtoon grammatikale probleme.

Die volgende kode voorbeeld toon hoe om die GPT-4o mini model in Aspose.Words te gebruik om grammatika te kontroleer:

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

Die nagaan van grammatika met Aspose.Words verbeter die kwaliteit van u werk en maak dit maklik om proeflees in u projekte te integreer. Vir meer inligting, kyk na die [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API dokumentasie.

{{% /alert %}}