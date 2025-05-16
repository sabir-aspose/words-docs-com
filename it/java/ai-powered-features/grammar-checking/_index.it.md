---
title: AI Controllo grammaticale
second_title: Aspose.Wordsper Java
articleTitle: Controllo grammaticale
linktitle: Controllo grammaticale
type: docs
weight: 40
description: "Controllare la grammatica di un documento. Aspose.Wordsper Java consente agli utenti di controllare la grammatica e rilevare errori nei documenti utilizzando i modelli OpenAI, Google e Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /it/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Controllare la grammatica nei documenti è importante per garantire chiarezza, professionalità e accuratezza. I documenti ben scritti lasciano un'impressione positiva ed evitano malintesi. I controlli grammaticali aiutano a identificare e correggere rapidamente gli errori, risparmiando tempo e migliorando la qualità.

Aspose.Words consente agli utenti di controllare la grammatica e rilevare errori nei documenti utilizzando le famiglie dei modelli OpenAI, Google e Claude elencate nell'enumerazione [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). Utilizzare il metodo [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) per analizzare il testo in un documento ed evidenziare i problemi grammaticali.

Il seguente esempio di codice mostra come utilizzare il modello GPT-4o mini in Aspose.Words per controllare la grammatica:

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

Il controllo della grammatica con Aspose.Words migliora la qualità del tuo lavoro e semplifica l'integrazione della correzione di bozze nei tuoi progetti. Per ulteriori informazioni, controllare [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}