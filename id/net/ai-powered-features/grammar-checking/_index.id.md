---
title: AI Pemeriksaan Tata Bahasa
second_title: Aspose.Words untuk .NET
articleTitle: Pemeriksaan Tata Bahasa
linktitle: Pemeriksaan Tata Bahasa
type: docs
weight: 40
description: "Periksa tata bahasa dokumen. Aspose.Words untuk .NET memungkinkan pengguna memeriksa tata bahasa dan mendeteksi kesalahan dalam dokumen menggunakan model OpenAI."
url: /id/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Memeriksa tata bahasa dalam dokumen penting untuk memastikan kejelasan, profesionalisme, dan akurasi. Dokumen yang ditulis dengan baik meninggalkan kesan positif dan menghindari kesalahpahaman. Pemeriksaan tata bahasa membantu mengidentifikasi dan memperbaiki kesalahan dengan cepat, menghemat waktu, dan meningkatkan kualitas.

Aspose.Words memungkinkan pengguna untuk memeriksa tata bahasa dan mendeteksi kesalahan dalam dokumen menggunakan model generatif **OpenAI**. Gunakan metode [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), yang tersedia di namespace [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/). **CheckGrammar** menganalisis teks dalam dokumen dan menyoroti masalah tata bahasa.

Contoh kode berikut menunjukkan cara menggunakan model GPT-4o mini dalam Aspose.Words untuk memeriksa tata bahasa:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Big document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use OpenAI generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gpt4OMini).WithApiKey(apiKey);

CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
grammarOptions.ImproveStylistics = true;

Document proofedDoc = model.CheckGrammar(doc, grammarOptions);
proofedDoc.Save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Memeriksa tata bahasa dengan Aspose.Words meningkatkan kualitas pekerjaan Anda dan memudahkan untuk mengintegrasikan proofreading ke dalam proyek Anda. Untuk informasi selengkapnya, lihat dokumentasi [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}