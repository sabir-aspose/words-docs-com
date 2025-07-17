---
title: Chuyển đổi Word sang PDF trong C#
second_title: Aspose.Words cho .NET
articleTitle: Biến đổi tài liệu thành PDF
linktitle: Biến đổi tài liệu thành PDF
description: "Chuyển đổi Word sang PDF trong C#. Ví dụ mã đơn giản để chuyển đổi DOCX sang PDF. Hỗ trợ tất cả định dạng Word và hình ảnh."
type: docs
weight: 10
url: /vi/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Khả năng chuyển đổi tài liệu một cách dễ dàng và đáng tin cậy từ định dạng này sang định dạng khác là tính năng chính của Aspose.Words. PDF là một trong những định dạng phổ biến nhất để chuyển đổi – đây là định dạng có bố cục cố định giữ nguyên diện mạo gốc của tài liệu khi hiển thị trên các nền tảng khác nhau. Thuật ngữ "hiển thị" được sử dụng trong Aspose.Words để mô tả quá trình biến đổi tài liệu thành định dạng tệp được phân trang hoặc có khái niệm về trang.

## Chuyển đổi tài liệu Word sang PDF

Chuyển đổi từ Word sang PDF là một quá trình khá phức tạp đòi hỏi nhiều giai đoạn tính toán. Công cụ bố cục của Aspose.Words bắt chước cách thức hoạt động của công cụ bố cục trang Microsoft Word, làm cho các tài liệu PDF đầu ra trông gần giống nhất với những gì bạn có thể thấy trong Microsoft Word.

Với Aspose.Words, bạn có thể biến đổi tài liệu theo chương trình từ các định dạng Word, chẳng hạn như DOC hoặc DOCX, sang PDF mà không cần sử dụng Microsoft Office. Bài viết này giải thích cách thực hiện chuyển đổi này.

{{% alert color="primary" %}}

Lưu ý rằng số lượng trang trong tài liệu ảnh hưởng đến thời gian chuyển đổi.

{{% /alert %}}

### Chuyển đổi DOCX hoặc DOC sang PDF

Biến đổi từ định dạng tài liệu DOC hoặc DOCX sang định dạng PDF trong Aspose.Words rất đơn giản và có thể đạt được chỉ với hai dòng mã:

1. Tải tài liệu của bạn vào đối tượng [Document](https://reference.aspose.com/words/net/aspose.words/document/) bằng cách sử dụng một trong các constructor của nó bằng cách chỉ định tên tài liệu với phần mở rộng định dạng.
1. Gọi một trong các phương thức [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) trên đối tượng **Document** và chỉ định định dạng đầu ra mong muốn là PDF bằng cách nhập tên tệp với phần mở rộng ".PDF".

Ví dụ mã sau đây cho thấy cách chuyển đổi tài liệu từ DOCX sang PDF bằng phương thức [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Bạn có thể tải xuống tệp mẫu của ví dụ này từ [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Đôi khi cần thiết phải chỉ định các tùy chọn bổ sung có thể ảnh hưởng đến kết quả lưu tài liệu dưới dạng PDF. Các tùy chọn này có thể được chỉ định bằng cách sử dụng lớp [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), chứa các thuộc tính xác định cách hiển thị đầu ra PDF.

Lưu ý rằng với cùng một kỹ thuật, bạn có thể chuyển sang bất kỳ tài liệu định dạng bố cục luồng nào sang định dạng PDF.

{{% /alert %}}

### Biến đổi sang các tiêu chuẩn PDF khác nhau

Aspose.Words cung cấp bảng liệt kê [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) để hỗ trợ chuyển đổi DOC hoặc DOCX sang các tiêu chuẩn định dạng PDF khác nhau (như PDF 1.7, PDF 1.5, v.v.).

Ví dụ mã sau đây minh họa cách chuyển đổi tài liệu sang PDF 1.7 bằng cách sử dụng [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) với tuân thủ PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Chuyển đổi hình ảnh sang PDF

Chuyển đổi sang PDF không giới hạn ở các định dạng tài liệu Microsoft Word. Bất kỳ định dạng nào được Aspose.Words hỗ trợ, bao gồm cả những định dạng được tạo theo chương trình, cũng có thể được chuyển sang PDF. Ví dụ, chúng ta có thể biến đổi hình ảnh một trang, như JPEG, PNG, BMP, EMF, hoặc WMF, cũng như hình ảnh nhiều trang, như TIFF và GIF, sang PDF.

Ví dụ mã sau đây cho thấy cách chuyển sang hình ảnh JPEG và TIFF sang PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Để mã này hoạt động, bạn cần thêm tham chiếu đến Aspose.Words và `System.Drawing` vào dự án của mình.

## Giảm kích thước đầu ra PDF

Khi lưu sang PDF, bạn có thể chỉ định liệu bạn có muốn tối ưu hóa đầu ra hay không. Để làm điều này, bạn cần đặt cờ [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) thành true, và sau đó các canvas lồng nhau dư thừa và trống sẽ được loại bỏ, các ký tự liền kề có cùng định dạng sẽ được nối lại.

Ví dụ mã sau đây cho thấy cách tối ưu hóa đầu ra:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Sử dụng thuộc tính **OptimizeOutput** có thể ảnh hưởng đến độ chính xác của việc hiển thị nội dung.

{{% /alert %}}

## Xem thêm

- Bài viết [Hiển thị](/words/vi/net/rendering/) để biết thêm thông tin về các định dạng trang cố định và bố cục luồng
- Bài viết [Chuyển đổi sang định dạng trang cố định](/words/vi/net/converting-to-fixed-page-format/#what-is-a-page-layout) để biết thêm thông tin về bố cục trang
- Bài viết [Chỉ định tùy chọn hiển thị khi biến đổi sang PDF](/words/vi/net/specify-rendering-options-when-converting-to-pdf/) để biết thêm thông tin về việc sử dụng lớp `PdfSaveOptions`
- Bài viết [Tìm hiểu các tính năng chuyển đổi sang PDF/A và PDF/UA](/words/vi/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) mô tả tiêu chuẩn PDF nào và ISO liên quan cho các tiêu chuẩn PDF được Aspose.Words hỗ trợ
- Bài viết [Tiêu chuẩn PDF nào tốt hơn để chọn](/words/vi/net/which-pdf-standard-is-better-to-choose/) để xác định tiêu chuẩn PDF nào có ý nghĩa cho trường hợp nào

- Bài viết [Làm việc với PDF/A hoặc PDF/UA](/words/vi/net/working-with-pdfa-or-pdfua/) mô tả các yêu cầu cho nội dung tài liệu ở định dạng PDF/A và PDF/UA – chủ yếu là các yêu cầu về cấu trúc và phông chữ

- Bài viết [Cảnh báo về các vấn đề truy cập khi lưu sang PDF/A và PDF/UA](/words/vi/net/warnings-when-saving-to-pdfa-and-pdfua/) mô tả các yêu cầu về khả năng truy cập nội dung mà PDF/A và PDF/UA áp đặt
