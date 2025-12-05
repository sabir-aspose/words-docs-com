---
title: AI Pemeriksaan Tata Bahasa
second_title: Aspose.Words untuk C++
articleTitle: Pemeriksaan Tata Bahasa
linktitle: Pemeriksaan Tata Bahasa
type: docs
weight: 40
description: "Periksa tata bahasa dokumen. Aspose.Words untuk C++ memungkinkan pengguna memeriksa tata bahasa dan mendeteksi kesalahan dalam dokumen menggunakan model OpenAI, Google, dan Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /id/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Memeriksa tata bahasa dalam dokumen penting untuk memastikan kejelasan, profesionalisme, dan akurasi. Dokumen yang ditulis dengan baik meninggalkan kesan positif dan menghindari kesalahpahaman. Pemeriksaan tata bahasa membantu mengidentifikasi dan memperbaiki kesalahan dengan cepat, menghemat waktu, dan meningkatkan kualitas.

Aspose.Words memungkinkan pengguna untuk memeriksa tata bahasa dan mendeteksi kesalahan dalam dokumen menggunakan rangkaian model OpenAI, Google, dan Claude yang tercantum dalam pencacahan [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). Gunakan metode [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), yang tersedia di namespace [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** menganalisis teks dalam dokumen dan menyoroti masalah tata bahasa.

Contoh kode berikut menunjukkan cara menggunakan model GPT-4o mini dalam Aspose.Words untuk memeriksa tata bahasa:

{{< highlight cpp >}}
void AiGrammar()
{
    auto doc = MakeObject<Document>(MyDir + u"Big document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto grammarOptions = MakeObject<CheckGrammarOptions>();
    grammarOptions->set_ImproveStylistics(true);

    auto proofedDoc = model->CheckGrammar(doc, grammarOptions);
    proofedDoc->Save(ArtifactsDir + u"AI.AiGrammar.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Memeriksa tata bahasa dengan Aspose.Words meningkatkan kualitas pekerjaan Anda dan memudahkan untuk mengintegrasikan proofreading ke dalam proyek Anda. Untuk informasi selengkapnya, lihat dokumentasi [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}