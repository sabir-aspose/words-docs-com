---
title: Làm Việc với Watermark trong Java
second_title: Aspose.Words cho Java
articleTitle: Làm việc Với Watermark
linktitle: Làm việc Với Watermark
type: docs
description: "Thao tác hình mờ tài liệu bằng Java."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /vi/java/working-with-watermark/
timestamp: 2025-04-22-08-07-04
---

Chủ đề này thảo luận về cách làm việc theo chương trình với hình mờ bằng Aspose.Words. Hình mờ là hình nền hiển thị phía sau văn bản trong tài liệu. Hình mờ có thể chứa văn bản hoặc hình ảnh được biểu thị bằng lớp [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/).

{{% alert color="primary" %}}

**Thử trực tuyến**

Bạn có thể thử chức năng này với chúng tôi [Hình mờ tài liệu trực tuyến miễn phí](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Thêm Hình Mờ Vào Tài liệu

Trong Microsoft Word, một hình mờ có thể dễ dàng được chèn vào tài liệu bằng lệnh Chèn Hình Mờ. Aspose.Words cung cấp lớp [watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) để thêm hoặc xóa hình mờ trong tài liệu. Aspose.Words cung cấp liệt kê [WatermarkType ](https://reference.aspose.com/words/java/com.aspose.words/watermarktype/) xác định ba loại hình mờ có thể có (Văn bản, Hình ảnh và Không có) để làm việc.

### Thêm Hình Mờ Văn Bản

Ví dụ mã sau đây trình bày cách chèn hình mờ văn bản trong tài liệu bằng cách xác định [TextWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/textwatermarkoptions/) bằng phương thức [SetText](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setText-java.lang.String):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddTextWatermarkWithSpecificOptions.java" >}}

### Thêm Hình Mờ Hình Ảnh

Ví dụ mã sau đây trình bày cách chèn hình mờ hình ảnh trong tài liệu bằng cách xác định [ImageWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/imagewatermarkoptions/) bằng phương thức [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.awt.image.BufferedImage):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddImageWatermarkWithSpecificOptions.java" >}}

Hình mờ hình ảnh có thể được chèn dưới dạng hình ảnh, chuỗi hoặc luồng.

Hình mờ cũng có thể được chèn bằng lớp hình dạng. Rất dễ dàng để chèn bất kỳ hình dạng hoặc hình ảnh nào vào đầu trang hoặc chân trang và do đó tạo ra một hình mờ thuộc bất kỳ loại nào có thể tưởng tượng được.

Ví dụ mã sau đây chèn hình mờ vào tài liệu Word:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-AddWatermarkToADocument-AddWatermarkToADocument.java" >}}

{{% alert color="primary" %}}

Bạn có thể tải xuống tệp mẫu của ví dụ này từ [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Document.doc).

{{% /alert %}}


## Xóa Hình Mờ Khỏi Tài liệu

Lớp [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) cung cấp phương thức `Remove` để xóa hình mờ khỏi tài liệu.

Các ví dụ mã sau đây cho thấy cách xóa hình mờ khỏi tài liệu:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-RemoveWatermarkFromDocument.java" >}}

Để xóa hình mờ khỏi tài liệu, bạn chỉ phải đặt tên của hình mờ trong khi chèn và sau đó xóa hình mờ bằng tên được gán.

Ví dụ mã sau đây chỉ cho bạn cách đặt tên của hình mờ và xóa nó khỏi tài liệu:

{{< highlight csharp >}}

// Set name to be able to remove it afterwards
watermark.Name("WaterMark");
{{< /highlight >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-RemoveWatermark-RemoveWatermark.java" >}}

## Thêm Hình Mờ vào Ô Bảng

Đôi khi bạn cần chèn hình mờ/hình ảnh vào ô của bảng và hiển thị nó bên ngoài bảng, bạn có thể sử dụng thuộc tính [IsLayoutInCell](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#isLayoutInCell-boolean). Thuộc tính này nhận hoặc đặt cờ cho biết hình dạng được hiển thị bên trong bảng hay bên ngoài bảng. Lưu ý rằng thuộc tính này chỉ hoạt động khi bạn tối ưu hóa tài liệu cho Microsoft Word 2010 bằng phương thức [OptimizeFor](https://reference.aspose.com/words/java/com.aspose.words/compatibilityoptions/#optimizeFor-int).

Ví dụ mã sau đây cho thấy cách sử dụng thuộc tính này:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-Shapes-WorkingWithShapes-SetShapeLayoutInCell.java" >}}
