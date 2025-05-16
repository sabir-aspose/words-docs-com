---
title: AI Kiểm Tra Ngữ Pháp
second_title: Aspose.Words cho Java
articleTitle: Kiểm Tra Ngữ Pháp
linktitle: Kiểm Tra Ngữ Pháp
type: docs
weight: 40
description: "Kiểm tra ngữ pháp tài liệu. Aspose.Words cho Java cho phép người dùng kiểm tra ngữ pháp và phát hiện lỗi trong tài liệu bằng cách sử dụng các mô hình OpenAI, Google và Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /vi/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Kiểm tra ngữ pháp trong tài liệu là rất quan trọng để đảm bảo sự rõ ràng, chuyên nghiệp và chính xác. Các tài liệu được viết tốt để lại ấn tượng tích cực và tránh hiểu lầm. Kiểm tra ngữ pháp giúp xác định và sửa lỗi nhanh chóng, tiết kiệm thời gian và cải thiện chất lượng.

Aspose.Words cho phép người dùng kiểm tra ngữ pháp và phát hiện lỗi trong tài liệu bằng cách sử dụng gia đình OpenAI, Google và Claude mô hình được liệt kê trong bảng liệt kê [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). Sử dụng phương pháp [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) để phân tích văn bản trong tài liệu và làm nổi bật các vấn đề ngữ pháp.

Ví dụ mã sau đây cho thấy cách sử dụng mô hình GPT-4o mini trong Aspose.Words để kiểm tra ngữ pháp:

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

Kiểm tra ngữ pháp với Aspose.Words cải thiện chất lượng công việc của bạn và giúp bạn dễ dàng tích hợp hiệu đính vào các dự án của mình. Để biết thêm thông tin, hãy kiểm tra [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}