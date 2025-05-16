---
title: AIการตรวจสอบไวยากรณ์
second_title: Aspose.WordsสำหรับJava
articleTitle: การตรวจสอบไวยากรณ์
linktitle: การตรวจสอบไวยากรณ์
type: docs
weight: 40
description: "ตรวจสอบไวยากรณ์เอกสาร Aspose.WordsสำหรับJava อนุญาตให้ผู้ใช้ตรวจสอบไวยากรณ์และตรวจจับข้อผิดพลาดในเอกสารโดยใช้รุ่นOpenAIกูเกิลและClaude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /th/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

การตรวจสอบไวยากรณ์ในเอกสารเป็นสิ่งสำคัญเพื่อให้แน่ใจว่าชัดเจนความเป็นมืออาชีพและความถูกต้อง เอกสารที่เขียนได้ดีทำให้เกิดความประทับใจในเชิงบวกและหลีกเลี่ยงความเข้าใจผิด การตรวจสอบไวยากรณ์ช่วยระบุและแก้ไขข้อผิดพลาดได้อย่างรวดเร็วช่วยประหยัดเวลาและปรับปรุงคุณภาพ.

Aspose.Wordsอนุญาตให้ผู้ใช้ตรวจสอบไวยากรณ์และตรวจจับข้อผิดพลาดในเอกสารโดยใช้ครอบครัวOpenAI,กูเกิล,และClaudeรุ่นที่ระบุไว้ในการแจงนับ[AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/) ใช้วิธีการ[CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions)เพื่อวิเคราะห์ข้อความในเอกสารและเน้นปัญหาทางไวยากรณ์.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีใช้GPT-4o miniรุ่นในAspose.Wordsเพื่อตรวจสอบไวยากรณ์:

{{< highlight java >}}
 Document doc = new Document("Big document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI generative language models.
 IAiModelText model = (OpenAiModel)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
 grammarOptions.setImproveStylistics(true);

 Document proofedDoc = model.checkGrammar(doc, grammarOptions);
 proofedDoc.save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

การตรวจสอบไวยากรณ์ด้วยAspose.Wordsปรับปรุงคุณภาพของการทำงานของคุณและทำให้มันง่ายที่จะ สำหรับข้อมูลเพิ่มเติมให้ตรวจสอบ[Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}