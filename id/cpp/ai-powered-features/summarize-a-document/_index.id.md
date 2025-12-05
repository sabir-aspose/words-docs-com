---
title: Meringkas Dokumen
second_title: Aspose.Words untuk C++
articleTitle: Meringkas Dokumen
linktitle: Meringkas Dokumen
type: docs
weight: 20
description: "Meringkas dokumen. Aspose.Words untuk C++ menyederhanakan peringkasan dokumen menggunakan model OpenAI dan Google AI dengan memungkinkan Anda menentukan panjang ringkasan."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /id/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Meringkas dokumen adalah alat yang berharga untuk tinjauan konten, wawasan cepat, atau menyiapkan abstrak. Aspose.Words mendukung peringkasan dokumen menggunakan model bertenaga AI, sehingga memudahkan pemrosesan teks panjang. Fitur ini, tersedia dalam namespace [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), mengintegrasikan model bahasa generatif lanjutan dari *OpenAI* dan *Google*, serta model bahasa generatif antropik *Claude's*. Daftar model yang didukung tersedia dalam pencacahan [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

Anda dapat menentukan berbagai opsi untuk meringkas konten dokumen. Gunakan metode [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) untuk membuat ringkasan dokumen Anda. Anda juga dapat mengatur panjang ringkasan menggunakan properti [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

Dengan Aspose.Words, menerapkan peringkasan dokumen sangatlah mudah. Contoh kode berikut menunjukkan cara meringkas dokumen menggunakan model GPT-4o:

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

Meringkas dokumen dengan Aspose.Words menghemat waktu dan membantu Anda fokus pada informasi penting. Untuk informasi selengkapnya, lihat dokumentasi [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
