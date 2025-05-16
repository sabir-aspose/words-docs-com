---
title: Tóm tắt Một Tài liệu
second_title: Aspose.Words cho C++
articleTitle: Tóm tắt Một Tài liệu
linktitle: Tóm tắt Một Tài liệu
type: docs
weight: 20
description: "Tóm tắt một tài liệu. Aspose.Words cho C++ đơn giản hóa việc tóm tắt tài liệu bằng cách sử dụng Các mô hình OpenAI Và Google AI bằng cách cho phép bạn chỉ định độ dài tóm tắt."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /vi/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Tóm tắt tài liệu là một công cụ có giá trị để xem xét nội dung, hiểu biết nhanh hoặc chuẩn bị tóm tắt. Aspose.Words hỗ trợ tóm tắt tài liệu bằng cách sử dụng các mô hình được hỗ trợ AI, giúp xử lý văn bản dài dễ dàng hơn. Tính năng này, có sẵn trong không gian tên [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), tích hợp các mô hình ngôn ngữ tạo nâng cao từ *OpenAI* và *Google*, cũng như các mô hình ngôn ngữ tạo nhân học *Claude's*. Danh sách các mô hình được hỗ trợ có sẵn trong bảng liệt kê [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

Bạn có thể chỉ định các tùy chọn khác nhau để tóm tắt nội dung tài liệu. Sử dụng phương thức [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) để tạo bản tóm tắt tài liệu của bạn. Bạn cũng có thể đặt độ dài tóm tắt bằng thuộc tính [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

Với Aspose.Words, việc thực hiện tóm tắt tài liệu rất đơn giản. Ví dụ mã sau đây cho thấy cách tóm tắt tài liệu bằng mô hình GPT-4o:

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

Tóm tắt tài liệu với Aspose.Words tiết kiệm thời gian và giúp bạn tập trung vào thông tin cần thiết. Để biết thêm thông tin, hãy kiểm tra tài liệu [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
