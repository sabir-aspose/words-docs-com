---
title: Làm Việc với Watermark trong Python
second_title: Aspose.Words cho Python via .NET
articleTitle: Làm việc Với Watermark
linktitle: Làm việc Với Watermark
description: "Tạo và quản lý hình mờ trong tài liệu bằng Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /vi/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Chủ đề này thảo luận về cách làm việc theo chương trình với watermark bằng Aspose.Words. Hình mờ là hình nền hiển thị phía sau văn bản trong tài liệu. Hình mờ có thể chứa văn bản hoặc hình ảnh được biểu thị bằng lớp [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Thử trực tuyến**

Bạn có thể thử chức năng này với chúng tôi [Hình mờ tài liệu trực tuyến miễn phí](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Cách Thêm Hình Mờ Vào Tài liệu

Trong Microsoft Word, một hình mờ có thể dễ dàng được chèn vào tài liệu bằng lệnh Chèn Hình Mờ. Aspose.Words cung cấp lớp [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) để thêm hoặc xóa hình mờ trong tài liệu. Aspose.Words cung cấp liệt kê [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) xác định ba loại hình mờ có thể có ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) và [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) để làm việc.

### Thêm Hình Mờ Văn Bản

Ví dụ mã sau đây trình bày cách chèn hình mờ văn bản trong tài liệu bằng cách xác định [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) bằng phương thức [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### Thêm Hình Mờ Hình Ảnh

Ví dụ mã sau đây trình bày cách chèn hình mờ hình ảnh trong tài liệu bằng cách xác định [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) bằng phương thức [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

Hình mờ hình ảnh có thể được chèn dưới dạng hình ảnh, chuỗi hoặc luồng.

Hình mờ cũng có thể được chèn bằng lớp hình dạng. Rất dễ dàng để chèn bất kỳ hình dạng hoặc hình ảnh nào vào đầu trang hoặc chân trang và do đó tạo ra một hình mờ thuộc bất kỳ loại nào có thể tưởng tượng được.

Ví dụ mã sau đây chèn hình mờ vào tài liệu Word:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

Bạn có thể tải xuống tệp mẫu của ví dụ này từ [đây](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Xóa Hình Mờ Khỏi Tài liệu

Lớp [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) cung cấp phương thức xóa để xóa hình mờ khỏi tài liệu.

Ví dụ mã sau đây cho thấy cách xóa hình mờ khỏi tài liệu:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

Nếu các hình mờ được thêm vào bằng cách sử dụng đối tượng lớp [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/) thì để xóa hình mờ khỏi tài liệu, bạn chỉ phải đặt tên của hình mờ trong khi chèn và sau đó xóa hình mờ bằng tên được gán.

Ví dụ mã sau đây chỉ cho bạn cách đặt tên của hình mờ và xóa nó khỏi tài liệu:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## Thêm Hình Mờ Trong Ô Bảng

Đôi khi bạn cần chèn hình mờ/hình ảnh vào ô của bảng và hiển thị nó bên ngoài bảng, bạn có thể sử dụng thuộc tính [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/). Thuộc tính này nhận hoặc đặt cờ cho biết hình dạng được hiển thị bên trong bảng hay bên ngoài bảng. Lưu ý rằng thuộc tính này chỉ hoạt động khi bạn tối ưu hóa tài liệu cho Microsoft Word 2010 bằng phương thức [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

Ví dụ mã sau đây cho thấy cách sử dụng thuộc tính này:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
