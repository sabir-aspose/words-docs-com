---
title: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
second_title: Aspose.WordsสำหรับJava
articleTitle: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
linktitle: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
type: docs
weight: 30
description: "แปลเอกสาร Aspose.WordsสำหรับJava ช่วยลดความยุ่งยากในการแปลเอกสารโดยใช้รุ่นของกูเกิลAIช่วยให้คุณสามารถระบุภาษาเป้าหมาย."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /th/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

แปลเอกสารเป็นตัวเลือกที่จำเป็นบ่อยครั้งในยุคของการแปลงเป็นดิจิทัลสูง Aspose.Wordsรองรับการแปลเอกสารโดยใช้แบบจำลองภาษาสร้าง*Google*ซึ่งช่วยให้นักพัฒนาในการแปลข้อความเนื้อหาเป็นมากกว่า 300 ภาษา.

ใช้วิธีการ[Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int)เพื่อแปลเอกสารของคุณเป็นภาษาใดก็ได้ที่แสดงในการแจงนับ[Language](https://reference.aspose.com/words/java/com.aspose.words/language/) โปรดทราบว่าหากเอกสารต้นฉบับประกอบด้วยหลายภาษารูปแบบที่ใช้ของกูเกิลAIจะสามา หากแบบจำลองไม่สามารถจดจำภาษาในบางส่วนของข้อความคุณจะถูกส่งคืนเอกสารพร้อ.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการใช้*Gemini 1.5 Flash*รุ่นในAspose.Wordsเพื่อแปลเอกสารเป็นภาษาอาหรับ:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

แปลเอกสารด้วยAspose.Wordsช่วยประหยัดเวลาและทำให้ง่ายต่อการบูรณาการฟังก์ชั่นการแปลในโค สำหรับข้อมูลเพิ่มเติมให้ตรวจสอบ[Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}