---
title: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
second_title: Aspose.WordsสำหรับC++
articleTitle: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
linktitle: การแปลภาษา,อังกฤษ(สหราชอาณาจักร)
type: docs
weight: 30
description: "แปลเอกสาร Aspose.WordsสำหรับC++ ช่วยลดความยุ่งยากในการแปลเอกสารโดยใช้รุ่นของกูเกิลAIช่วยให้คุณสามารถระบุภาษาเป้าหมาย."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /th/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

แปลเอกสารเป็นตัวเลือกที่จำเป็นบ่อยครั้งในยุคของการแปลงเป็นดิจิทัลสูง Aspose.Wordsรองรับการแปลเอกสารโดยใช้แบบจำลองภาษาสร้าง*Google*ซึ่งช่วยให้นักพัฒนาในการแปลข้อความเนื้อหาเป็นมากกว่า 300 ภาษา.

ใช้วิธีการ[Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/)เพื่อแปลเอกสารของคุณเป็นภาษาใดก็ได้ที่แสดงในการแจงนับ[Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) โปรดทราบว่าหากเอกสารต้นฉบับประกอบด้วยหลายภาษารูปแบบที่ใช้ของกูเกิลAIจะสามา หากแบบจำลองไม่สามารถจดจำภาษาในบางส่วนของข้อความคุณจะถูกส่งคืนเอกสารพร้อ.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการใช้*Gemini 1.5 Flash*รุ่นในAspose.Wordsเพื่อแปลเอกสารเป็นภาษาอาหรับ:

{{< highlight cpp >}}
void AiTranslate()
{
    auto doc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<GoogleAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto translatedDoc = model->Translate(doc, Language::Arabic);
    translatedDoc->Save(ArtifactsDir + u"AI.AiTranslate.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

แปลเอกสารด้วยAspose.Wordsช่วยประหยัดเวลาและทำให้ง่ายต่อการบูรณาการฟังก์ชั่นการแปลในโค สำหรับข้อมูลเพิ่มเติมให้ตรวจสอบเอกสาร[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)API.

{{% /alert %}}