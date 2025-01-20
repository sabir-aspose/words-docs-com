---
title: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
second_title: Aspose.WordsสำหรับPython via .NET
articleTitle: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
linktitle: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
type: docs
weight: 30
description: "แปลเอกสาร Aspose.WordsสำหรับPython ช่วยลดความยุ่งยากในการแปลเอกสารโดยใช้รุ่นของกูเกิลAIช่วยให้คุณสามารถระบุภาษาเป้าหมาย."
url: /th/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

แปลเอกสารเป็นตัวเลือกที่จำเป็นบ่อยครั้งในยุคของการแปลงเป็นดิจิทัลสูง Aspose.Wordsรองรับการแปลเอกสารโดยใช้แบบจำลองภาษาสร้าง*Google*ซึ่งช่วยให้นักพัฒนาในการแปลข้อความเนื้อหาเป็นมากกว่า 300 ภาษา.

ใช้วิธีการ[Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language)เพื่อแปลเอกสารของคุณเป็นภาษาใดก็ได้ที่แสดงในการแจงนับ[Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) โปรดทราบว่าหากเอกสารต้นฉบับประกอบด้วยหลายภาษารูปแบบที่ใช้ของกูเกิลAIจะสามา หากแบบจำลองไม่สามารถจดจำภาษาในบางส่วนของข้อความคุณจะถูกส่งคืนเอกสารพร้อ.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการใช้*Gemini 1.5 Flash*รุ่นในAspose.Wordsเพื่อแปลเอกสารเป็นภาษาอาหรับ:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

แปลเอกสารด้วยAspose.Wordsช่วยประหยัดเวลาและทำให้ง่ายต่อการบูรณาการฟังก์ชั่นการแปลในโค สำหรับข้อมูลเพิ่มเติมให้ตรวจสอบเอกสาร[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)API.

{{% /alert %}}