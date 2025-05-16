---
title: Dịch Một Tài liệu
second_title: Aspose.Words cho Java
articleTitle: Dịch Một Tài liệu
linktitle: Dịch Một Tài liệu
type: docs
weight: 30
description: "Dịch một tài liệu. Aspose.Words cho Java đơn giản hóa dịch tài liệu bằng Các mô hình Google AI, cho phép bạn chỉ định ngôn ngữ đích."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /vi/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Dịch tài liệu là một lựa chọn thường xuyên cần thiết trong thời đại số hóa cao. Aspose.Words hỗ trợ dịch tài liệu bằng cách sử dụng các mô hình ngôn ngữ tạo *Google*, cho phép các nhà phát triển dịch nội dung văn bản sang hơn 300 ngôn ngữ.

Sử dụng phương thức [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) để dịch tài liệu của bạn sang bất kỳ ngôn ngữ nào được biểu thị trong liệt kê [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). Lưu ý rằng nếu tài liệu nguồn chứa một số ngôn ngữ, Mô hình Dựa Trên Google AI sẽ có thể dịch tất cả các ngôn ngữ được hỗ trợ. Nếu mô hình không thể nhận ra ngôn ngữ trong một số đoạn văn bản, thì bạn sẽ được trả về một tài liệu với các đoạn chưa được dịch này và với phần còn lại của văn bản được dịch.

Ví dụ mã sau đây cho thấy cách sử dụng mô hình *Gemini 1.5 Flash* trong Aspose.Words để dịch tài liệu sang tiếng ả rập:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Dịch tài liệu với Aspose.Words tiết kiệm thời gian và giúp dễ dàng tích hợp chức năng dịch vào các dự án của bạn. Để biết thêm thông tin, hãy kiểm tra [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}