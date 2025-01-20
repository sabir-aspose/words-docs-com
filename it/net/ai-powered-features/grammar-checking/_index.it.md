---
title: AI Controllo grammaticale
second_title: Aspose.Wordsper .NET
articleTitle: Controllo grammaticale
linktitle: Controllo grammaticale
type: docs
weight: 40
description: "Controllare la grammatica di un documento. Aspose.Wordsper .NET consente agli utenti di controllare la grammatica e rilevare errori nei documenti utilizzando i modelli OpenAI."
url: /it/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Controllare la grammatica nei documenti è importante per garantire chiarezza, professionalità e accuratezza. I documenti ben scritti lasciano un'impressione positiva ed evitano malintesi. I controlli grammaticali aiutano a identificare e correggere rapidamente gli errori, risparmiando tempo e migliorando la qualità.

Aspose.Words consente agli utenti di controllare la grammatica e rilevare errori nei documenti utilizzando modelli generativi **OpenAI**. Utilizzare il metodo [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), disponibile nello spazio dei nomi [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/). **CheckGrammar** analizza il testo di un documento ed evidenzia i problemi grammaticali.

Il seguente esempio di codice mostra come utilizzare il modello GPT-4o mini in Aspose.Words per controllare la grammatica:

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

Il controllo della grammatica con Aspose.Words migliora la qualità del tuo lavoro e semplifica l'integrazione della correzione di bozze nei tuoi progetti. Per ulteriori informazioni, controllare la documentazione [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}