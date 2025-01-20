---
title: AIการตรวจสอบไวยากรณ์
second_title: Aspose.Wordsสำหรับ.NET
articleTitle: การตรวจสอบไวยากรณ์
linktitle: การตรวจสอบไวยากรณ์
type: docs
weight: 40
description: "ตรวจสอบไวยากรณ์เอกสาร Aspose.Wordsสำหรับ.NET อนุญาตให้ผู้ใช้สามารถตรวจสอบไวยากรณ์และตรวจจับข้อผิดพลาดในเอกสารโดยใช้รุ่นOpenAI."
url: /th/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

การตรวจสอบไวยากรณ์ในเอกสารเป็นสิ่งสำคัญเพื่อให้แน่ใจว่าชัดเจนความเป็นมืออาชีพและความถูกต้อง เอกสารที่เขียนได้ดีทำให้เกิดความประทับใจในเชิงบวกและหลีกเลี่ยงความเข้าใจผิด การตรวจสอบไวยากรณ์ช่วยระบุและแก้ไขข้อผิดพลาดได้อย่างรวดเร็วช่วยประหยัดเวลาและปรับปรุงคุณภาพ.

Aspose.Wordsช่วยให้ผู้ใช้สามารถตรวจสอบไวยากรณ์และตรวจจับข้อผิดพลาดในเอกสารโดยใช้แบบจำลอง**OpenAI** ใช้วิธีการ[CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/)ที่มีอยู่ในเนมสเปซ[Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) **CheckGrammar**วิเคราะห์ข้อความในเอกสารและเน้นปัญหาทางไวยากรณ์.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีใช้GPT-4o miniรุ่นในAspose.Wordsเพื่อตรวจสอบไวยากรณ์:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Big document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use OpenAI generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gpt4OMini).WithApiKey(apiKey);

CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
grammarOptions.ImproveStylistics = true;

Document proofedDoc = model.CheckGrammar(doc, grammarOptions);
proofedDoc.Save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

การตรวจสอบไวยากรณ์ด้วยAspose.Wordsปรับปรุงคุณภาพของการทำงานของคุณและทำให้มันง่ายที่จะ สำหรับข้อมูลเพิ่มเติมให้ตรวจสอบเอกสาร[Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)API.

{{% /alert %}}