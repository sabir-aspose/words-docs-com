---
title: Tradurre un documento
second_title: Aspose.Wordsper Java
articleTitle: Tradurre un documento
linktitle: Tradurre un documento
type: docs
weight: 30
description: "Tradurre un documento. Aspose.Wordsper Java semplifica la traduzione di documenti utilizzando i modelli Google AI, consentendo di specificare la lingua di destinazione."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /it/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

La traduzione di documenti è un'opzione spesso necessaria nell'era dell'alta digitalizzazione. Aspose.Words supporta la traduzione di documenti utilizzando modelli linguistici generativi *Google*, che consentono agli sviluppatori di tradurre il contenuto dei testi in più di 300 lingue.

Utilizzare il metodo [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) per tradurre i documenti in qualsiasi lingua rappresentata nell'enumerazione [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). Si noti che se il documento di origine contiene più lingue, il modello basato su Google AI sarà in grado di tradurre tutte le lingue supportate. Se il modello non è in grado di riconoscere la lingua in alcuni frammenti di testo, verrà restituito un documento con questi frammenti non tradotti e con il resto del testo tradotto.

Il seguente esempio di codice mostra come utilizzare il modello *Gemini 1.5 Flash* in Aspose.Words per tradurre un documento in arabo:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Tradurre documenti con Aspose.Words consente di risparmiare tempo e semplifica l'integrazione delle funzionalità di traduzione nei progetti. Per ulteriori informazioni, controllare [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}