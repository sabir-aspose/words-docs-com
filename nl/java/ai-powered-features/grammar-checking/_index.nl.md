---
title: AI Grammaticacontrole
second_title: Aspose.Words voor Java
articleTitle: Grammaticacontrole
linktitle: Grammaticacontrole
type: docs
weight: 40
description: "Controleer de grammatica van een document. Aspose.Words voor Java hiermee kunnen gebruikers grammatica controleren en fouten in documenten detecteren met behulp van OpenAI, Google en Claude modellen."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nl/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Het controleren van grammatica in documenten is belangrijk om duidelijkheid, professionaliteit en nauwkeurigheid te garanderen. Goed geschreven documenten laten een positieve indruk achter en voorkomen misverstanden. Grammaticacontroles helpen fouten snel te identificeren en te corrigeren, waardoor tijd wordt bespaard en de kwaliteit wordt verbeterd.

Aspose.Words stelt gebruikers in staat om grammatica te controleren en fouten in documenten te detecteren met behulp van de families van de OpenAI, Google en Claude modellen die in de [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/) - opsomming worden vermeld. Gebruik de methode [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) om de tekst in een document te analyseren en grammaticale problemen te markeren.

Het volgende codevoorbeeld laat zien hoe u het GPT-4o mini model in Aspose.Words gebruikt om grammatica te controleren:

{{< highlight java >}}
 Document doc = new Document("Big document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI generative language models.
 IAiModelText model = (OpenAiModel)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
 grammarOptions.setImproveStylistics(true);

 Document proofedDoc = model.checkGrammar(doc, grammarOptions);
 proofedDoc.save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Het controleren van grammatica met Aspose.Words verbetert de kwaliteit van uw werk en maakt het gemakkelijk om proeflezen in uw projecten te integreren. Kijk voor meer informatie op [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}