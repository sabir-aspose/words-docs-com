---
title: Tradurre un documento
second_title: Aspose.Wordsper .NET
articleTitle: Tradurre un documento
linktitle: Tradurre un documento
type: docs
weight: 30
description: "Tradurre un documento. Aspose.Wordsper .NET semplifica la traduzione di documenti utilizzando i modelli Google AI, consentendo di specificare la lingua di destinazione."
url: /it/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

La traduzione di documenti è un'opzione spesso necessaria nell'era dell'alta digitalizzazione. Aspose.Words supporta la traduzione di documenti utilizzando modelli linguistici generativi *Google*, che consentono agli sviluppatori di tradurre il contenuto dei testi in più di 300 lingue.

Utilizzare il metodo [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) per tradurre i documenti in qualsiasi lingua rappresentata nell'enumerazione [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Si noti che se il documento di origine contiene più lingue, il modello basato su Google AI sarà in grado di tradurre tutte le lingue supportate. Se il modello non è in grado di riconoscere la lingua in alcuni frammenti di testo, verrà restituito un documento con questi frammenti non tradotti e con il resto del testo tradotto.

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

Tradurre documenti con Aspose.Words consente di risparmiare tempo e semplifica l'integrazione delle funzionalità di traduzione nei progetti. Per ulteriori informazioni, controllare la documentazione [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}