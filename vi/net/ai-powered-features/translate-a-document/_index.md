---
title: Dịch một tài liệu
second_title: Aspose.Words cho .NET
articleTitle: Dịch một tài liệu
linktitle: Dịch một tài liệu
type: docs
weight: 30
description: "Dịch một tài liệu. Aspose.Words cho .NET đơn giản hóa việc dịch tài liệu bằng các mô hình AI của Google, cho phép bạn chỉ định ngôn ngữ đích."
url: /vi/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Dịch tài liệu là một tùy chọn thường xuyên cần thiết trong thời đại số hóa cao. Aspose.Words hỗ trợ dịch tài liệu bằng các mô hình ngôn ngữ tạo *Google*, cho phép các nhà phát triển dịch nội dung văn bản sang hơn 300 ngôn ngữ.

Sử dụng phương thức [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) để dịch tài liệu của bạn sang bất kỳ ngôn ngữ nào được biểu diễn trong phép liệt kê [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Lưu ý rằng nếu tài liệu nguồn chứa nhiều ngôn ngữ, mô hình dựa trên AI của Google sẽ có thể dịch tất cả các ngôn ngữ được hỗ trợ. Nếu mô hình không thể nhận dạng ngôn ngữ trong một số đoạn văn bản, thì bạn sẽ nhận được một tài liệu có các đoạn chưa dịch này và phần còn lại của văn bản đã được dịch.

Ví dụ mã sau đây cho thấy cách sử dụng mô hình *Gemini 1.5 Flash* trong Aspose.Words để dịch tài liệu sang tiếng Ả Rập:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Dịch tài liệu bằng Aspose.Words giúp tiết kiệm thời gian và dễ dàng tích hợp chức năng dịch vào các dự án của bạn. Để biết thêm thông tin, hãy xem tài liệu API [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

{{% /alert %}}