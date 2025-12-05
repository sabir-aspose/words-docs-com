---
title: Dịch Một Tài liệu
second_title: Aspose.Words cho Python via .NET
articleTitle: Dịch Một Tài liệu
linktitle: Dịch Một Tài liệu
type: docs
weight: 30
description: "Dịch một tài liệu. Aspose.Words cho Python đơn giản hóa dịch tài liệu bằng Các mô hình Google AI, cho phép bạn chỉ định ngôn ngữ đích."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /vi/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Dịch tài liệu là một lựa chọn thường xuyên cần thiết trong thời đại số hóa cao. Aspose.Words hỗ trợ dịch tài liệu bằng cách sử dụng các mô hình ngôn ngữ tạo *Google*, cho phép các nhà phát triển dịch nội dung văn bản sang hơn 300 ngôn ngữ.

Sử dụng phương thức [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) để dịch tài liệu của bạn sang bất kỳ ngôn ngữ nào được biểu thị trong liệt kê [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). Lưu ý rằng nếu tài liệu nguồn chứa một số ngôn ngữ, Mô hình Dựa Trên Google AI sẽ có thể dịch tất cả các ngôn ngữ được hỗ trợ. Nếu mô hình không thể nhận ra ngôn ngữ trong một số đoạn văn bản, thì bạn sẽ được trả về một tài liệu với các đoạn chưa được dịch này và với phần còn lại của văn bản được dịch.

Ví dụ mã sau đây cho thấy cách sử dụng mô hình *Gemini 1.5 Flash* trong Aspose.Words để dịch tài liệu sang tiếng ả rập:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Dịch tài liệu với Aspose.Words tiết kiệm thời gian và giúp dễ dàng tích hợp chức năng dịch vào các dự án của bạn. Để biết thêm thông tin, hãy kiểm tra tài liệu [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}