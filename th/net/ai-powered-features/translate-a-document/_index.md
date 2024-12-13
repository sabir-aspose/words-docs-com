---
title: แปลเอกสาร
second_title: Aspose.Words สำหรับ .NET
articleTitle: แปลเอกสาร
linktitle: แปลเอกสาร
type: เอกสาร
weight: 30
description: "แปลเอกสาร Aspose.Words สำหรับ .NET ทำให้การแปลเอกสารง่ายขึ้นโดยใช้โมเดล AI ของ Google ช่วยให้คุณระบุภาษาเป้าหมายได้"
url: /th/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

การแปลเอกสารเป็นตัวเลือกที่จำเป็นบ่อยครั้งในยุคดิจิทัล Aspose.Words รองรับการแปลเอกสารโดยใช้โมเดลภาษากำเนิดของ *Google* ซึ่งช่วยให้นักพัฒนาสามารถแปลเนื้อหาข้อความเป็นภาษาต่างๆ ได้มากกว่า 300 ภาษา

ใช้เมธอด [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) เพื่อแปลเอกสารของคุณเป็นภาษาใดๆ ที่แสดงในการแจงนับ [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) โปรดทราบว่าหากเอกสารต้นฉบับมีหลายภาษา โมเดลที่ใช้ AI ของ Google จะสามารถแปลภาษาที่รองรับทั้งหมดได้ หากโมเดลไม่สามารถจดจำภาษาในข้อความบางส่วนได้ คุณจะได้รับเอกสารที่ประกอบด้วยข้อความบางส่วนที่ยังไม่ได้แปลเหล่านี้และข้อความที่เหลือที่ได้รับการแปลแล้ว

ตัวอย่างโค้ดต่อไปนี้แสดงวิธีใช้โมเดล *Gemini 1.5 Flash* ใน Aspose.Words เพื่อแปลเอกสารเป็นภาษาอาหรับ:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

การแปลเอกสารด้วย Aspose.Words ช่วยประหยัดเวลาและทำให้การผสานรวมฟังก์ชันการแปลเข้ากับโปรเจ็กต์ของคุณเป็นเรื่องง่าย สำหรับข้อมูลเพิ่มเติม โปรดดูเอกสาร API [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)

{{% /alert %}}