---
title: Low Code
second_title: Aspose.Words cho .NET
articleTitle: Làm việc Với Các Tài liệu sử dụng LowCode API
linktitle: Low Code
type: docs
description: "Đơn giản hóa các tác vụ xử lý tài liệu như so sánh, chuyển đổi, tách, hợp nhất, tìm và thay thế và các tác vụ khác bằng cách sử dụng Low Code API. Aspose.Words LowCode API với cú pháp sạch, kết quả nhanh và nỗ lực mã hóa tối thiểu."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /vi/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words cho .NET cung cấp không gian tên [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/), giúp đơn giản hóa các tác vụ xử lý tài liệu phổ biến. API này được thiết kế cho các nhà phát triển muốn thực hiện các hoạt động cấp cao như so sánh tài liệu, trích xuất nội dung, chuyển đổi hình ảnh và thay thế văn bản với nỗ lực tối thiểu.

LowCode API là lý tưởng cho các kịch bản mà việc thực hiện nhanh chóng quan trọng hơn kiểm soát hạt mịn. Chúng ta hãy xem xét kỹ hơn các khả năng LowCode của Aspose.Words cho .NET.

{{% alert color="primary" %}}

Điều quan trọng cần lưu ý là LowCode API không cho phép bạn thay đổi cấu trúc tài liệu.

{{% /alert %}}

## Các Tính năng có sẵn trong LowCode API

Không gian tên `Aspose.Words.LowCode` hiện hỗ trợ:

* **Converting** tài liệu từ định dạng này sang định dạng khác
* **Comparing** tài liệu
* **Mail merging**
* **Reporting** dựa trên cú pháp LINQ
* **Merging** tài liệu
* **Search and replace**
* **Digital signing** tài liệu
* **Splitting** một tài liệu thành các phần sử dụng các tiêu chí khác nhau
* Thêm một **watermark**

{{% alert color="primary" %}}

Xin lưu ý rằng có thể tìm thấy mô tả chi tiết về từng chức năng bên ngoài Low Code trong Phần Hướng dẫn Dành cho Nhà phát triển.

{{% /alert %}}

## Thông thạo và Không Thông thạo API

Aspose.Words cho .NET hỗ trợ Cả Thông thạo và Không Thông thạo APIs, cho phép các nhà phát triển chọn kiểu phù hợp nhất với sở thích mã hóa và nhu cầu dự án của họ. Chúng ta hãy xem xét một số ví dụ để xem hai loại API này khác nhau như thế nào.

{{% alert color="primary" %}}

Trong Fluent API, các hoạt động có thể được cấu hình và thực thi thông qua một ngữ cảnh (chẳng hạn như ComparerContext hoặc ReplacerContext). Bối cảnh này chứa các tùy chọn phổ biến. Nó đảm bảo rằng tất cả các phương thức liên quan hoạt động với cấu hình nhất quán, làm cho API mạnh mẽ và dễ quản lý trong các tình huống phức tạp.

{{% /alert %}}

### So Sánh Tài Liệu

Sử dụng `LowCode` để so sánh hai tài liệu Word và lưu kết quả.

**ví dụ api không thông thạo:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**ví dụ api thông thạo:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

Bạn cũng có thể vượt qua `CompareOptions` để so sánh tinh chỉnh.

**ví dụ api không thông thạo:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

CompareOptions options = new CompareOptions
{
    IgnoreFormatting = true,
    IgnoreCaseChanges = true
};

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc, options);
{{< /highlight >}}

**ví dụ api thông thạo:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

ComparerContext comparerContext = new ComparerContext();
comparerContext.CompareOptions.IgnoreCaseChanges = true;

Comparer.Create(comparerContext)
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.3.docx")
   .Execute();
{{< /highlight >}}

### Chuyển Đổi Tài liệu Thành Hình ảnh

Sử dụng `LowCode` để chuyển đổi tài liệu Word thành PDF.

**ví dụ api không thông thạo:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**ví dụ api thông thạo:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Tìm Và Thay Thế Văn Bản

Sử dụng `LowCode` để nhanh chóng thay thế văn bản trên toàn bộ tài liệu.

**ví dụ api không thông thạo:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**ví dụ api thông thạo:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";

ReplacerContext replacerContext = new ReplacerContext();
replacerContext.SetReplacement("ReplaceMe", "Replacement");

Replacer.Create(replacerContext)
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

## Tại Sao Sử Dụng Aspose.Words Low Code

Không gian tên **Aspose.Words.LowCode** giúp bạn thực hiện các tác vụ xử lý tài liệu cấp cao một cách nhanh chóng với cú pháp sạch, có thể đọc được. Nó đặc biệt hữu ích cho các nhà phát triển cần tốc độ, đơn giản và mã có thể bảo trì khi làm việc với các tài liệu Word.

Để khám phá các tùy chọn nâng cao hơn, bạn luôn có thể kết hợp LowCode APIs với mô hình đối tượng Aspose.Words đầy đủ. Xem thêm Low Code ví dụ trong [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).