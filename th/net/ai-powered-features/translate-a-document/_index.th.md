---
title: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
second_title: Aspose.Wordsสำหรับ.NET
articleTitle: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
linktitle: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
type: docs
weight: 30
description: "แปลเอกสาร Aspose.Wordsสำหรับ.NET ช่วยลดความยุ่งยากในการแปลเอกสารโดยใช้รุ่นของกูเกิลAIช่วยให้คุณสามารถระบุภาษาเป้าหมาย."
url: /th/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

แปลเอกสารเป็นตัวเลือกที่จำเป็นบ่อยครั้งในยุคของการแปลงเป็นดิจิทัลสูง Aspose.Wordsรองรับการแปลเอกสารโดยใช้แบบจำลองภาษาสร้าง*Google*ซึ่งช่วยให้นักพัฒนาในการแปลข้อความเนื้อหาเป็นมากกว่า 300 ภาษา.

ใช้วิธีการ[Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/)เพื่อแปลเอกสารของคุณเป็นภาษาใดก็ได้ที่แสดงในการแจงนับ[Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) โปรดทราบว่าหากเอกสารต้นฉบับประกอบด้วยหลายภาษารูปแบบที่ใช้ของกูเกิลAIจะสามา หากแบบจำลองไม่สามารถจดจำภาษาในบางส่วนของข้อความคุณจะถูกส่งคืนเอกสารพร้อ.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการใช้*Gemini 1.5 Flash*รุ่นในAspose.Wordsเพื่อแปลเอกสารเป็นภาษาอาหรับ:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

แปลเอกสารด้วยAspose.Wordsช่วยประหยัดเวลาและทำให้ง่ายต่อการบูรณาการฟังก์ชั่นการแปลในโค สำหรับข้อมูลเพิ่มเติมให้ตรวจสอบเอกสาร[Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)API.

{{% /alert %}}