---
title: Menerjemahkan Dokumen
second_title: Aspose.Words untuk Python via .NET
articleTitle: Menerjemahkan Dokumen
linktitle: Menerjemahkan Dokumen
type: docs
weight: 30
description: "Terjemahkan dokumen. Aspose.Words untuk Python menyederhanakan terjemahan dokumen menggunakan model Google AI, memungkinkan Anda menentukan bahasa target."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /id/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Penerjemahan dokumen adalah pilihan yang sering dibutuhkan di era digitalisasi tinggi. Aspose.Words mendukung terjemahan dokumen menggunakan model bahasa generatif *Google*, yang memungkinkan pengembang menerjemahkan konten teks ke lebih dari 300 bahasa.

Gunakan metode [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) untuk menerjemahkan dokumen Anda ke dalam bahasa apa pun yang diwakili dalam enumerasi [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). Perhatikan bahwa jika dokumen sumber berisi beberapa bahasa, model berbasis Google AI akan dapat menerjemahkan semua bahasa yang didukung. Jika model tidak dapat mengenali bahasa dalam beberapa fragmen teks, maka Anda akan dikembalikan dokumen dengan fragmen yang tidak diterjemahkan ini dan dengan teks lainnya diterjemahkan.

Contoh kode berikut menunjukkan cara menggunakan model *Gemini 1.5 Flash* dalam Aspose.Words untuk menerjemahkan dokumen ke dalam bahasa Arab:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Menerjemahkan dokumen dengan Aspose.Words menghemat waktu dan memudahkan integrasi fungsionalitas terjemahan ke dalam proyek Anda. Untuk informasi selengkapnya, lihat dokumentasi [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}