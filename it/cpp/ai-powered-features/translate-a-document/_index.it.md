---
title: Tradurre un documento
second_title: Aspose.Wordsper C++
articleTitle: Tradurre un documento
linktitle: Tradurre un documento
type: docs
weight: 30
description: "Tradurre un documento. Aspose.Wordsper C++ semplifica la traduzione di documenti utilizzando i modelli Google AI, consentendo di specificare la lingua di destinazione."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /it/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

La traduzione di documenti è un'opzione spesso necessaria nell'era dell'alta digitalizzazione. Aspose.Words supporta la traduzione di documenti utilizzando modelli linguistici generativi *Google*, che consentono agli sviluppatori di tradurre il contenuto dei testi in più di 300 lingue.

Utilizzare il metodo [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) per tradurre i documenti in qualsiasi lingua rappresentata nell'enumerazione [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/). Si noti che se il documento di origine contiene più lingue, il modello basato su Google AI sarà in grado di tradurre tutte le lingue supportate. Se il modello non è in grado di riconoscere la lingua in alcuni frammenti di testo, verrà restituito un documento con questi frammenti non tradotti e con il resto del testo tradotto.

Il seguente esempio di codice mostra come utilizzare il modello *Gemini 1.5 Flash* in Aspose.Words per tradurre un documento in arabo:

{{< highlight cpp >}}
void AiTranslate()
{
    auto doc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<GoogleAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto translatedDoc = model->Translate(doc, Language::Arabic);
    translatedDoc->Save(ArtifactsDir + u"AI.AiTranslate.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Tradurre documenti con Aspose.Words consente di risparmiare tempo e semplifica l'integrazione delle funzionalità di traduzione nei progetti. Per ulteriori informazioni, controllare la documentazione [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}