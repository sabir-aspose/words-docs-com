---
title: AI Kiểm Tra Ngữ Pháp
second_title: Aspose.Words cho Python via .NET
articleTitle: Kiểm Tra Ngữ Pháp
linktitle: Kiểm Tra Ngữ Pháp
type: docs
weight: 40
description: "Kiểm tra ngữ pháp tài liệu. Aspose.Words cho Python cho phép người dùng kiểm tra ngữ pháp và phát hiện lỗi trong tài liệu bằng cách sử dụng các mô hình OpenAI, Google và Claude."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /vi/python-net/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Kiểm tra ngữ pháp trong tài liệu là rất quan trọng để đảm bảo sự rõ ràng, chuyên nghiệp và chính xác. Các tài liệu được viết tốt để lại ấn tượng tích cực và tránh hiểu lầm. Kiểm tra ngữ pháp giúp xác định và sửa lỗi nhanh chóng, tiết kiệm thời gian và cải thiện chất lượng.

Aspose.Words cho phép người dùng kiểm tra ngữ pháp và phát hiện lỗi trong tài liệu bằng cách sử dụng các họ của OpenAI, Google và Claude được liệt kê trong bảng liệt kê [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). Sử dụng phương thức [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), có sẵn trong không gian tên [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** phân tích văn bản trong tài liệu và nêu bật các vấn đề ngữ pháp.

Ví dụ mã sau đây cho thấy cách sử dụng mô hình GPT-4o mini trong Aspose.Words để kiểm tra ngữ pháp:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + 'Big document.docx')

api_key = system_helper.environment.Environment.get_environment_variable('API_KEY')
# Use OpenAI generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GPT_4O_MINI).with_api_key(api_key).as_open_ai_model()

grammar_options = aw.ai.CheckGrammarOptions()
grammar_options.improve_stylistics = True

proofed_doc = model.check_grammar(doc, grammar_options)
proofed_doc.save(file_name='AI.AiGrammar.docx')
{{< /highlight >}}

{{% alert color="primary" %}}

Kiểm tra ngữ pháp với Aspose.Words cải thiện chất lượng công việc của bạn và giúp bạn dễ dàng tích hợp hiệu đính vào các dự án của mình. Để biết thêm thông tin, hãy kiểm tra tài liệu [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}