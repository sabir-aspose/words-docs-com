---
title: Menerjemahkan Dokumen
second_title: Aspose.Words untuk C++
articleTitle: Menerjemahkan Dokumen
linktitle: Menerjemahkan Dokumen
type: docs
weight: 30
description: "Terjemahkan dokumen. Aspose.Words untuk C++ menyederhanakan terjemahan dokumen menggunakan model Google AI, memungkinkan Anda menentukan bahasa target."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /id/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Penerjemahan dokumen adalah pilihan yang sering dibutuhkan di era digitalisasi tinggi. Aspose.Words mendukung terjemahan dokumen menggunakan model bahasa generatif *Google*, yang memungkinkan pengembang menerjemahkan konten teks ke lebih dari 300 bahasa.

Gunakan metode [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) untuk menerjemahkan dokumen Anda ke dalam bahasa apa pun yang diwakili dalam enumerasi [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/). Perhatikan bahwa jika dokumen sumber berisi beberapa bahasa, model berbasis Google AI akan dapat menerjemahkan semua bahasa yang didukung. Jika model tidak dapat mengenali bahasa dalam beberapa fragmen teks, maka Anda akan dikembalikan dokumen dengan fragmen yang tidak diterjemahkan ini dan dengan teks lainnya diterjemahkan.

Contoh kode berikut menunjukkan cara menggunakan model *Gemini 1.5 Flash* dalam Aspose.Words untuk menerjemahkan dokumen ke dalam bahasa Arab:

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

Menerjemahkan dokumen dengan Aspose.Words menghemat waktu dan memudahkan integrasi fungsionalitas terjemahan ke dalam proyek Anda. Untuk informasi selengkapnya, lihat dokumentasi [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}