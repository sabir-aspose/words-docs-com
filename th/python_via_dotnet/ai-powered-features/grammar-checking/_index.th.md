---
title: AIการตรวจสอบไวยากรณ์
second_title: Aspose.WordsสำหรับPython via .NET
articleTitle: การตรวจสอบไวยากรณ์
linktitle: การตรวจสอบไวยากรณ์
type: docs
weight: 40
description: "ตรวจสอบไวยากรณ์เอกสาร Aspose.WordsสำหรับPython อนุญาตให้ผู้ใช้สามารถตรวจสอบไวยากรณ์และตรวจจับข้อผิดพลาดในเอกสารโดยใช้รุ่นOpenAI."
url: /th/python-net/grammar-checking/
timestamp: 2025-01-15-16-40-05
---

การตรวจสอบไวยากรณ์ในเอกสารเป็นสิ่งสำคัญเพื่อให้แน่ใจว่าชัดเจนความเป็นมืออาชีพและความถูกต้อง เอกสารที่เขียนได้ดีทำให้เกิดความประทับใจในเชิงบวกและหลีกเลี่ยงความเข้าใจผิด การตรวจสอบไวยากรณ์ช่วยระบุและแก้ไขข้อผิดพลาดได้อย่างรวดเร็วช่วยประหยัดเวลาและปรับปรุงคุณภาพ.

Aspose.Wordsช่วยให้ผู้ใช้สามารถตรวจสอบไวยากรณ์และตรวจจับข้อผิดพลาดในเอกสารโดยใช้แบบจำลอง**OpenAI** ใช้วิธีการ[CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions)ที่มีอยู่ในเนมสเปซ[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) **CheckGrammar**วิเคราะห์ข้อความในเอกสารและเน้นปัญหาทางไวยากรณ์.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีใช้GPT-4o miniรุ่นในAspose.Wordsเพื่อตรวจสอบไวยากรณ์:

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

การตรวจสอบไวยากรณ์ด้วยAspose.Wordsปรับปรุงคุณภาพของการทำงานของคุณและทำให้มันง่ายที่จะ สำหรับข้อมูลเพิ่มเติมให้ตรวจสอบเอกสาร[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)API.

{{% /alert %}}