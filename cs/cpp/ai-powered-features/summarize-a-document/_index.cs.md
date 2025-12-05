---
title: Shrňte dokument
second_title: Aspose.Words pro C++
articleTitle: Shrňte dokument
linktitle: Shrňte dokument
type: docs
weight: 20
description: "Shrňte dokument. Aspose.Words pro C++ zjednodušuje sumarizaci dokumentů pomocí modelů OpenAI a Google AI tím, že umožňuje určit délku souhrnu."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cs/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Shrnutí dokumentů je cenným nástrojem pro kontrolu obsahu, rychlé postřehy nebo přípravu abstraktů. Aspose.Words podporuje sumarizaci dokumentů pomocí modelů poháněných AI, což usnadňuje zpracování dlouhého textu. Tato funkce, dostupná v oboru názvů [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), integruje pokročilé generativní jazykové modely z *OpenAI* a *Google* a také *Claude's* antropické generativní jazykové modely. Seznam podporovaných modelů je k dispozici ve výčtu [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

Můžete zadat různé možnosti pro shrnutí obsahu dokumentu. Pomocí metody [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) Vygenerujte souhrn dokumentu. Můžete také nastavit délku souhrnu pomocí vlastnosti [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

S Aspose.Words je shrnutí implementačního dokumentu jednoduché. Následující příklad kódu ukazuje, jak shrnout dokument pomocí modelu GPT-4o:

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

Shrnutí dokumentů pomocí Aspose.Words šetří čas a pomáhá vám soustředit se na základní informace. Další informace najdete v dokumentaci [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
