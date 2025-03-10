---
title: AI Pemeriksaan Tata Bahasa
second_title: Aspose.Words untuk Python via .NET
articleTitle: Pemeriksaan Tata Bahasa
linktitle: Pemeriksaan Tata Bahasa
type: docs
weight: 40
description: "Periksa tata bahasa dokumen. Aspose.Words untuk Python memungkinkan pengguna memeriksa tata bahasa dan mendeteksi kesalahan dalam dokumen menggunakan model OpenAI."
url: /id/python-net/grammar-checking/
timestamp: 2025-01-15-16-40-05
---

Memeriksa tata bahasa dalam dokumen penting untuk memastikan kejelasan, profesionalisme, dan akurasi. Dokumen yang ditulis dengan baik meninggalkan kesan positif dan menghindari kesalahpahaman. Pemeriksaan tata bahasa membantu mengidentifikasi dan memperbaiki kesalahan dengan cepat, menghemat waktu, dan meningkatkan kualitas.

Aspose.Words memungkinkan pengguna untuk memeriksa tata bahasa dan mendeteksi kesalahan dalam dokumen menggunakan model generatif **OpenAI**. Gunakan metode [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), yang tersedia di namespace [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** menganalisis teks dalam dokumen dan menyoroti masalah tata bahasa.

Contoh kode berikut menunjukkan cara menggunakan model GPT-4o mini dalam Aspose.Words untuk memeriksa tata bahasa:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + 'Big document.docx')

api_key = system_helper.environment.Environment.get_environment_variable('API_KEY')
# Use OpenAI generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GPT_4O_MINI).with_api_key(api_key).as_open_ai_model()

grammar_options = aw.ai.CheckGrammarOptions()
grammar_options.improve_stylistics = True

proofed_doc = model.check_grammar(doc, grammar_options)
proofed_doc.save(file_name='AI.AiGrammar.docx')
{{< /highlight >}}

{{% alert color="primary" %}}

Memeriksa tata bahasa dengan Aspose.Words meningkatkan kualitas pekerjaan Anda dan memudahkan untuk mengintegrasikan proofreading ke dalam proyek Anda. Untuk informasi selengkapnya, lihat dokumentasi [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}