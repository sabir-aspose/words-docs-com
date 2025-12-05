---
title: Rezumați un Document
second_title: Aspose.Words pentru C++
articleTitle: Rezumați un Document
linktitle: Rezumați un Document
type: docs
weight: 20
description: "Rezumați un document. Aspose.Words pentru C++ simplifică rezumarea documentelor folosind modelele OpenAI și Google AI, permițându-vă să specificați lungimea rezumatului."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ro/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Rezumarea documentelor este un instrument valoros pentru revizuirea conținutului, informații rapide sau pregătirea rezumatelor. Aspose.Words acceptă rezumarea documentelor folosind modele alimentate cu AI, facilitând procesarea textului lung. Această caracteristică, disponibilă în spațiul de nume [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), integrează modele avansate de limbaj generativ din *OpenAI* și *Google*, precum și *Claude's* modele de limbaj generativ antropic. Lista modelelor acceptate este disponibilă în enumerarea [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

Puteți specifica diverse opțiuni pentru rezumarea conținutului documentului. Utilizați metoda [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) pentru a genera un rezumat al documentului. De asemenea, puteți seta lungimea rezumatului folosind proprietatea [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

Cu Aspose.Words, implementarea rezumării documentelor este simplă. Următorul exemplu de cod arată cum se rezumă un document folosind GPT-4o model:

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

Rezumarea documentelor cu Aspose.Words economisește timp și vă ajută să vă concentrați asupra informațiilor esențiale. Pentru mai multe informații, verificați documentația [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
