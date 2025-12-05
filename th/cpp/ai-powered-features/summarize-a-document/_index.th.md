---
title: สรุปเอกสาร
second_title: Aspose.WordsสำหรับC++
articleTitle: สรุปเอกสาร
linktitle: สรุปเอกสาร
type: docs
weight: 20
description: "สรุปเอกสาร Aspose.WordsสำหรับC++ ช่วยลดความยุ่งยากในการสรุปเอกสารโดยใช้รุ่นOpenAIและกูเกิลAIโดยให้คุณระบุความยาวสรุป."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /th/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

การสรุปเอกสารเป็นเครื่องมือที่มีคุณค่าสำหรับการตรวจทานเนื้อหาข้อมูลเชิงลึกอย่างรว Aspose.Wordsรองรับการสรุปเอกสารโดยใช้รุ่นAIขับเคลื่อน,ทำให้ง่ายต่อการประมวลผลข้อความยาว. คุณลักษณะนี้สามารถใช้ได้ใน[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)เนมสเปซรวมโมเดลภาษาสืบพันธุ์ขั้นสูงจาก*OpenAI*และ*Google*รวมทั้งโมเดลภาษาสืบพันธุ์ของมนุษย์ด้วย*Claude's* รายการรุ่นที่รองรับมีอยู่ในการแจงนับ[AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/)

คุณสามารถระบุตัวเลือกต่างๆสำหรับการสรุปเนื้อหาเอกสาร ใช้วิธีการ[Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/)เพื่อสร้างสรุปเอกสารของคุณ คุณยังสามารถตั้งค่าความยาวสรุปโดยใช้คุณสมบัติ[SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

ด้วยAspose.Wordsการดำเนินการสรุปเอกสารจะตรงไปตรงมา ตัวอย่างรหัสต่อไปนี้แสดงวิธีการสรุปเอกสารโดยใช้รูปแบบGPT-4o:

{{< highlight cpp >}}
void AiSummarize()
{
    auto firstDoc = MakeObject<Document>(MyDir + u"Big document.docx");
    auto secondDoc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"))->WithOrganization(u"Organization")->WithProject(u"Project");

    auto options = MakeObject<SummarizeOptions>();

    options->set_SummaryLength(SummaryLength::Short);
    auto firstDocumentSummary = model->Summarize(firstDoc, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.One.docx");

    System::ArrayPtr<System::SharedPtr<Document>> documents = System::MakeArray<System::SharedPtr<Document>>(2);
    documents[0] = firstDoc;
    documents[1] = secondDoc;

    options->set_SummaryLength(SummaryLength::Long);
    auto multiDocumentSummary = model->Summarize(documents, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.Multi.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

สรุปเอกสารด้วยAspose.Wordsช่วยประหยัดเวลาและช่วยให้คุณมุ่งเน้นไปที่ข้อมูลที่จำเป็น สำหรับข้อมูลเพิ่มเติมให้ตรวจสอบเอกสาร[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)API.

{{% /alert %}}
