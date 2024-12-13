---
title: Terjemahkan Dokumen
second_title: Aspose.Words untuk .NET
articleTitle: Terjemahkan Dokumen
linktitle: Terjemahkan Dokumen
type: docs
weight: 30
description: "Terjemahkan dokumen. Aspose.Words untuk .NET menyederhanakan penerjemahan dokumen menggunakan model AI Google, yang memungkinkan Anda menentukan bahasa target."
url: /id/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Penerjemahan dokumen merupakan opsi yang sering dibutuhkan di era digitalisasi tinggi. Aspose.Words mendukung penerjemahan dokumen menggunakan model bahasa generatif *Google*, yang memungkinkan pengembang menerjemahkan konten teks ke lebih dari 300 bahasa.

Gunakan metode [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) untuk menerjemahkan dokumen Anda ke dalam bahasa apa pun yang direpresentasikan dalam enumerasi [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Perhatikan bahwa jika dokumen sumber berisi beberapa bahasa, model berbasis Google AI akan dapat menerjemahkan semua bahasa yang didukung. Jika model tidak dapat mengenali bahasa dalam beberapa fragmen teks, maka Anda akan mendapatkan dokumen dengan fragmen yang tidak diterjemahkan ini dan dengan sisa teks yang diterjemahkan.

Contoh kode berikut menunjukkan cara menggunakan model *Gemini 1.5 Flash* di Aspose.Words untuk menerjemahkan dokumen ke dalam bahasa Arab:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Menerjemahkan dokumen dengan Aspose.Words menghemat waktu dan memudahkan integrasi fungsionalitas terjemahan ke dalam proyek Anda. Untuk informasi lebih lanjut, periksa dokumentasi API [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

{{% /alert %}}