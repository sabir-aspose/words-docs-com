---
title: AIการตรวจสอบไวยากรณ์
second_title: Aspose.WordsสำหรับC++
articleTitle: การตรวจสอบไวยากรณ์
linktitle: การตรวจสอบไวยากรณ์
type: docs
weight: 40
description: "ตรวจสอบไวยากรณ์เอกสาร Aspose.WordsสำหรับC++ อนุญาตให้ผู้ใช้ตรวจสอบไวยากรณ์และตรวจจับข้อผิดพลาดในเอกสารโดยใช้รุ่นOpenAIกูเกิลและClaude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /th/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

การตรวจสอบไวยากรณ์ในเอกสารเป็นสิ่งสำคัญเพื่อให้แน่ใจว่าชัดเจนความเป็นมืออาชีพและความถูกต้อง เอกสารที่เขียนได้ดีทำให้เกิดความประทับใจในเชิงบวกและหลีกเลี่ยงความเข้าใจผิด การตรวจสอบไวยากรณ์ช่วยระบุและแก้ไขข้อผิดพลาดได้อย่างรวดเร็วช่วยประหยัดเวลาและปรับปรุงคุณภาพ.

Aspose.Wordsอนุญาตให้ผู้ใช้ตรวจสอบไวยากรณ์และตรวจจับข้อผิดพลาดในเอกสารโดยใช้ครอบครัวOpenAI,กูเกิล,และClaudeรุ่นที่ระบุไว้ในการแจงนับ[AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/) ใช้วิธีการ[CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/)ที่มีอยู่ในเนมสเปซ[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) **CheckGrammar**วิเคราะห์ข้อความในเอกสารและเน้นปัญหาทางไวยากรณ์.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีใช้GPT-4o miniรุ่นในAspose.Wordsเพื่อตรวจสอบไวยากรณ์:

{{< highlight cpp >}}
void AiGrammar()
{
    auto doc = MakeObject<Document>(MyDir + u"Big document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto grammarOptions = MakeObject<CheckGrammarOptions>();
    grammarOptions->set_ImproveStylistics(true);

    auto proofedDoc = model->CheckGrammar(doc, grammarOptions);
    proofedDoc->Save(ArtifactsDir + u"AI.AiGrammar.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

การตรวจสอบไวยากรณ์ด้วยAspose.Wordsปรับปรุงคุณภาพของการทำงานของคุณและทำให้มันง่ายที่จะ สำหรับข้อมูลเพิ่มเติมให้ตรวจสอบเอกสาร[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)API.

{{% /alert %}}