---
title: AI Grammaticacontrole
second_title: Aspose.Words voor .NET
articleTitle: Grammaticacontrole
linktitle: Grammaticacontrole
type: docs
weight: 40
description: "Controleer de grammatica van een document. Aspose.Words voor .NET hiermee kunnen gebruikers grammatica controleren en fouten in documenten detecteren met behulp van OpenAI - modellen."
url: /nl/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Het controleren van grammatica in documenten is belangrijk om duidelijkheid, professionaliteit en nauwkeurigheid te garanderen. Goed geschreven documenten laten een positieve indruk achter en voorkomen misverstanden. Grammaticacontroles helpen fouten snel te identificeren en te corrigeren, waardoor tijd wordt bespaard en de kwaliteit wordt verbeterd.

Aspose.Words stelt gebruikers in staat om grammatica te controleren en fouten in documenten te detecteren met behulp van **OpenAI** generatieve modellen. Gebruik de methode [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), Beschikbaar in de [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) naamruimte. **CheckGrammar** analyseert de tekst in een document en wijst op grammaticale problemen.

Het volgende codevoorbeeld laat zien hoe u het GPT-4o mini model in Aspose.Words gebruikt om grammatica te controleren:

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

Het controleren van grammatica met Aspose.Words verbetert de kwaliteit van uw werk en maakt het gemakkelijk om proeflezen in uw projecten te integreren. Raadpleeg de [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API documentatie voor meer informatie.

{{% /alert %}}