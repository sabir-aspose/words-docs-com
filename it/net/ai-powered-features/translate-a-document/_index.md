---
title: Traduci un documento
second_title: Aspose.Words per .NET
articleTitle: Traduci un documento
linktitle: Traduci un documento
type: docs
weight: 30
description: "Traduci un documento. Aspose.Words per .NET semplifica la traduzione dei documenti utilizzando i modelli di intelligenza artificiale di Google, consentendoti di specificare la lingua di destinazione."
url: /it/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

La traduzione dei documenti è un'opzione spesso necessaria nell'era dell'elevata digitalizzazione. Aspose.Words supporta la traduzione dei documenti utilizzando modelli linguistici generativi di *Google*, che consentono agli sviluppatori di tradurre il contenuto dei testi in oltre 300 lingue.

Utilizza il metodo [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) per tradurre i tuoi documenti in qualsiasi lingua rappresentata nell'enumerazione [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Nota che se il documento di origine contiene diverse lingue, il modello basato su Google AI sarà in grado di tradurre tutte le lingue supportate. Se il modello non riesce a riconoscere la lingua in alcuni frammenti di testo, ti verrà restituito un documento con questi frammenti non tradotti e con il resto del testo tradotto.

Il seguente esempio di codice mostra come utilizzare il modello *Gemini 1.5 Flash* in Aspose.Words per tradurre un documento in arabo:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

La traduzione di documenti con Aspose.Words consente di risparmiare tempo e semplifica l'integrazione della funzionalità di traduzione nei progetti. Per ulteriori informazioni, consulta la documentazione API di [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

{{% /alert %}}