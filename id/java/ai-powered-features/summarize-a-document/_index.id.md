---
title: Meringkas Dokumen
second_title: Aspose.Words untuk Java
articleTitle: Meringkas Dokumen
linktitle: Meringkas Dokumen
type: docs
weight: 20
description: "Meringkas dokumen. Aspose.Words untuk Java menyederhanakan peringkasan dokumen menggunakan model OpenAI dan Google AI dengan memungkinkan Anda menentukan panjang ringkasan."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /id/java/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Meringkas dokumen adalah alat yang berharga untuk tinjauan konten, wawasan cepat, atau menyiapkan abstrak. Aspose.Words mendukung peringkasan dokumen menggunakan model bertenaga AI, sehingga memudahkan pemrosesan teks panjang. Fitur ini, tersedia dalam fungsionalitas AI berbasis Aspose.Words, mengintegrasikan model bahasa generatif lanjutan dari *OpenAI* dan *Google*, serta model bahasa generatif antropik *Claude's*. Daftar model yang didukung tersedia dalam pencacahan [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/).

Anda dapat menentukan berbagai opsi untuk meringkas konten dokumen. Gunakan metode [Summarize](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#summarize-com.aspose.words.Document-com.aspose.words.SummarizeOptions) untuk membuat ringkasan dokumen Anda. Anda juga dapat mengatur panjang ringkasan menggunakan properti [SummaryLength](https://reference.aspose.com/words/java/com.aspose.words/summarizeoptions/#getSummaryLength).

Dengan Aspose.Words, menerapkan peringkasan dokumen sangatlah mudah. Contoh kode berikut menunjukkan cara meringkas dokumen menggunakan model GPT-4o:

{{< highlight java >}}
Document firstDoc = new Document(getMyDir() + "Big document.docx");
 Document secondDoc = new Document(getMyDir() + "Document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI or Google generative language models.
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 Document oneDocumentSummary = model.summarize(firstDoc, new SummarizeOptions(); { oneDocumentSummary.setSummaryLength(SummaryLength.SHORT); });
 oneDocumentSummary.save(getArtifactsDir() + "AI.AiSummarize.One.docx");

 Document multiDocumentSummary = model.summarize(new Document[] { firstDoc, secondDoc }, new SummarizeOptions(); { multiDocumentSummary.setSummaryLength(SummaryLength.LONG); });
 multiDocumentSummary.save(getArtifactsDir() + "AI.AiSummarize.Multi.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Meringkas dokumen dengan Aspose.Words menghemat waktu dan membantu Anda fokus pada informasi penting. Untuk informasi lebih lanjut, periksa [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}