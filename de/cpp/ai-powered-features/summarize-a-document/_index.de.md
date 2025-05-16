---
title: Ein Dokument zusammenfassen
second_title: Aspose.Words für C++
articleTitle: Ein Dokument zusammenfassen
linktitle: Ein Dokument zusammenfassen
type: docs
weight: 20
description: "Fassen Sie ein Dokument zusammen. Aspose.Words für C++ vereinfacht die Dokumentzusammenfassung mit OpenAI- und Google AI -Modellen, indem Sie die Länge der Zusammenfassung angeben können."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /de/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Das Zusammenfassen von Dokumenten ist ein wertvolles Werkzeug für die Inhaltsprüfung, schnelle Einblicke oder das Erstellen von Abstracts. Aspose.Words unterstützt die Dokumentzusammenfassung mit AI-basierten Modellen, wodurch die Verarbeitung von Langtext erleichtert wird. Diese Funktion, die im [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)-Namespace verfügbar ist, integriert erweiterte generative Sprachmodelle aus *OpenAI* und *Google* sowie *Claude's* anthropische generative Sprachmodelle. Die Liste der unterstützten Modelle ist in der [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/)-Aufzählung verfügbar.

Sie können verschiedene Optionen für die Zusammenfassung von Dokumentinhalten angeben. Verwenden Sie die Methode [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/), um eine Zusammenfassung Ihres Dokuments zu generieren. Sie können die Zusammenfassungslänge auch mit der Eigenschaft [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/) festlegen.

Mit Aspose.Words ist die Implementierung der Dokumentzusammenfassung unkompliziert. Das folgende Codebeispiel zeigt, wie Sie ein Dokument mit dem Modell GPT-4o zusammenfassen:

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

Das Zusammenfassen von Dokumenten mit Aspose.Words spart Zeit und hilft Ihnen, sich auf wesentliche Informationen zu konzentrieren. Weitere Informationen finden Sie in der Dokumentation zu [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
