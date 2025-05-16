---
title: สรุปเอกสาร
second_title: Aspose.WordsสำหรับJava
articleTitle: สรุปเอกสาร
linktitle: สรุปเอกสาร
type: docs
weight: 20
description: "สรุปเอกสาร Aspose.WordsสำหรับJava ช่วยลดความยุ่งยากในการสรุปเอกสารโดยใช้รุ่นOpenAIและกูเกิลAIโดยให้คุณระบุความยาวสรุป."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /th/java/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

การสรุปเอกสารเป็นเครื่องมือที่มีคุณค่าสำหรับการตรวจทานเนื้อหาข้อมูลเชิงลึกอย่างรว Aspose.Wordsรองรับการสรุปเอกสารโดยใช้AI-รุ่นขับเคลื่อน,ทำให้ง่ายต่อการประมวลผลข้อความยาว. ฟังก์ชันAIตามAspose.Wordsจะรวมโมเดลภาษาสร้างขั้นสูงจาก*OpenAI*และ*Google*รวมทั้ง*Claude's*โมเดลภาษาสร้างมนุษย์ รายการรุ่นที่รองรับมีอยู่ในการแจงนับ[AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/).

คุณสามารถระบุตัวเลือกต่างๆสำหรับการสรุปเนื้อหาเอกสาร ใช้วิธีการ[Summarize](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#summarize-com.aspose.words.Document-com.aspose.words.SummarizeOptions)เพื่อสร้างสรุปเอกสารของคุณ นอกจากนี้คุณยังสามารถตั้งค่าความยาวสรุปโดยใช้คุณสมบัติ[SummaryLength](https://reference.aspose.com/words/java/com.aspose.words/summarizeoptions/#getSummaryLength).

ด้วยAspose.Wordsการดำเนินการสรุปเอกสารจะตรงไปตรงมา ตัวอย่างรหัสต่อไปนี้แสดงวิธีการสรุปเอกสารโดยใช้รูปแบบGPT-4o:

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

สรุปเอกสารด้วยAspose.Wordsช่วยประหยัดเวลาและช่วยให้คุณมุ่งเน้นไปที่ข้อมูลที่จำเป็น สำหรับข้อมูลเพิ่มเติมให้ตรวจสอบ[Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}