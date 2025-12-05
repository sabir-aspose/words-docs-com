---
title: AI Grammatika-Kontrole
second_title: Aspose.Words vir Java
articleTitle: Grammatika-Kontrole
linktitle: Grammatika-Kontrole
type: docs
weight: 40
description: "Gaan'n dokumentgrammatika na. Aspose.Words vir Java laat gebruikers toe om grammatika te kontroleer en foute in dokumente op te spoor met behulp van OpenAI, Google en Claude modelle."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /af/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Dit is belangrik om grammatika in dokumente te kontroleer om duidelikheid, professionaliteit en akkuraatheid te verseker. Goedgeskrewe dokumente laat'n positiewe indruk en vermy misverstande. Grammatika-kontroles help om foute vinnig te identifiseer en reg te stel, wat tyd bespaar en kwaliteit verbeter.

Aspose.Words laat gebruikers toe om grammatika te kontroleer en foute in dokumente op te spoor deur die OpenAI, Google en Claude modelle se families te gebruik wat in die [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/) opsomming gelys word. Gebruik die [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) - metode om die teks in'n dokument te ontleed en grammatikale probleme uit te lig.

Die volgende kode voorbeeld toon hoe om die GPT-4o mini model in Aspose.Words te gebruik om grammatika te kontroleer:

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

Die nagaan van grammatika met Aspose.Words verbeter die kwaliteit van u werk en maak dit maklik om proeflees in u projekte te integreer. Vir meer inligting, kyk na die [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}