---
title: Riassumere un documento
second_title: Aspose.Wordsper C++
articleTitle: Riassumere un documento
linktitle: Riassumere un documento
type: docs
weight: 20
description: "Riassumere un documento. Aspose.Wordsper C++ semplifica il riepilogo dei documenti utilizzando i modelli OpenAI e Google AI, consentendo di specificare la lunghezza del riepilogo."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /it/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Il riepilogo dei documenti è uno strumento prezioso per la revisione dei contenuti, approfondimenti rapidi o la preparazione di abstract. Aspose.Words supporta il riepilogo dei documenti utilizzando modelli basati su AI, semplificando l'elaborazione di testo lungo. Questa funzione, disponibile nello spazio dei nomi [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), integra modelli di linguaggio generativo avanzati da *OpenAI* e *Google*, nonché modelli di linguaggio generativo antropico *Claude's*. L'elenco dei modelli supportati è disponibile nell'enumerazione [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

È possibile specificare varie opzioni per il riepilogo del contenuto del documento. Utilizzare il metodo [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) per generare un riepilogo del documento. È inoltre possibile impostare la lunghezza del riepilogo utilizzando la proprietà [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

Con Aspose.Words, l'implementazione del riepilogo dei documenti è semplice. L'esempio di codice seguente mostra come riassumere un documento utilizzando il modello GPT-4o:

{{< highlight cpp >}}
void AiSummarize()
{
    auto firstDoc = MakeObject<Document>(MyDir + u"Big document.docx");
    auto secondDoc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"))->WithOrganization(u"Organization")->WithProject(u"Project");

    auto options = MakeObject<SummarizeOptions>();

    options->set_SummaryLength(SummaryLength::Short);
    auto firstDocumentSummary = model->Summarize(firstDoc, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.One.docx");

    System::ArrayPtr<System::SharedPtr<Document>> documents = System::MakeArray<System::SharedPtr<Document>>(2);
    documents[0] = firstDoc;
    documents[1] = secondDoc;

    options->set_SummaryLength(SummaryLength::Long);
    auto multiDocumentSummary = model->Summarize(documents, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.Multi.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

La sintesi dei documenti con Aspose.Words consente di risparmiare tempo e consente di concentrarsi sulle informazioni essenziali. Per ulteriori informazioni, controllare la documentazione [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
