---
title: Podsumuj dokument
second_title: Aspose.Words dla C++
articleTitle: Podsumuj dokument
linktitle: Podsumuj dokument
type: docs
weight: 20
description: "Podsumuj dokument. Aspose.Words dla C++ upraszcza podsumowywanie dokumentów za pomocą modeli OpenAI i Google AI, umożliwiając określenie długości podsumowania."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pl/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Podsumowanie dokumentów jest cennym narzędziem do przeglądania treści, szybkiego wglądu lub przygotowywania streszczeń. Aspose.Words obsługuje podsumowanie dokumentów przy użyciu modeli opartych na AI, co ułatwia przetwarzanie długiego tekstu. Ta funkcja, dostępna w przestrzeni nazw [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), integruje zaawansowane generatywne modele językowe z *OpenAI* i *Google*, a także *Claude's* antropiczne generatywne modele językowe. Lista obsługiwanych modeli jest dostępna w wyliczeniu [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

Możesz określić różne opcje podsumowania zawartości dokumentu. Użyj metody [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/), aby wygenerować podsumowanie dokumentu. Możesz także ustawić długość podsumowania za pomocą właściwości [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

Dzięki Aspose.Words implementacja podsumowania dokumentu jest prosta. Poniższy przykład kodu pokazuje, jak podsumować dokument przy użyciu modelu GPT-4o:

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

Podsumowanie dokumentów za pomocą Aspose.Words oszczędza czas i pomaga skupić się na podstawowych informacjach. Aby uzyskać więcej informacji, sprawdź dokumentację [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
