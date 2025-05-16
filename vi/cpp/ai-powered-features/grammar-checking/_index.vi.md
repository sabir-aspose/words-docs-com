---
title: AI Kiểm Tra Ngữ Pháp
second_title: Aspose.Words cho C++
articleTitle: Kiểm Tra Ngữ Pháp
linktitle: Kiểm Tra Ngữ Pháp
type: docs
weight: 40
description: "Kiểm tra ngữ pháp tài liệu. Aspose.Words cho C++ cho phép người dùng kiểm tra ngữ pháp và phát hiện lỗi trong tài liệu bằng cách sử dụng các mô hình OpenAI, Google và Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /vi/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Kiểm tra ngữ pháp trong tài liệu là rất quan trọng để đảm bảo sự rõ ràng, chuyên nghiệp và chính xác. Các tài liệu được viết tốt để lại ấn tượng tích cực và tránh hiểu lầm. Kiểm tra ngữ pháp giúp xác định và sửa lỗi nhanh chóng, tiết kiệm thời gian và cải thiện chất lượng.

Aspose.Words cho phép người dùng kiểm tra ngữ pháp và phát hiện lỗi trong tài liệu bằng cách sử dụng các họ của OpenAI, Google và Claude được liệt kê trong bảng liệt kê [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). Sử dụng phương thức [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), có sẵn trong không gian tên [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** phân tích văn bản trong tài liệu và nêu bật các vấn đề ngữ pháp.

Ví dụ mã sau đây cho thấy cách sử dụng mô hình GPT-4o mini trong Aspose.Words để kiểm tra ngữ pháp:

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

Kiểm tra ngữ pháp với Aspose.Words cải thiện chất lượng công việc của bạn và giúp bạn dễ dàng tích hợp hiệu đính vào các dự án của mình. Để biết thêm thông tin, hãy kiểm tra tài liệu [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}