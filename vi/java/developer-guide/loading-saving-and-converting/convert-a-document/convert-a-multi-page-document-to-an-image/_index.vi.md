---
title: Chuyển Đổi Tài liệu Nhiều trang thành Hình ảnh trong Java
second_title: Aspose.Words cho Java
articleTitle: Chuyển Đổi Tài liệu Nhiều trang thành Hình Ảnh
linktitle: Chuyển Đổi Tài liệu Nhiều trang thành Hình Ảnh
type: docs
description: "Xuất tài liệu nhiều trang sang hình ảnh raster(JPG, PNG, GIF, BMP, TIFF, WebP) sử dụng Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /vi/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words cho Java cho phép người dùng xuất tài liệu nhiều trang sang hình ảnh raster. Điều này có thể hữu ích để tạo bản xem trước, lưu trữ hoặc biểu diễn trực quan các tài liệu để sử dụng không thể chỉnh sửa.

## Những Định dạng Nào Hỗ trợ Xuất Nhiều trang?

Aspose.Words hỗ trợ xuất nhiều trang sang các định dạng hình ảnh raster sau:

* Jpeg
* Gio
* Tg
* Bt
* Tiff
* WebP

## Cách Xuất Tài liệu Nhiều trang Sang Hình Ảnh

Tính năng xuất tài liệu nhiều trang sang hình ảnh được triển khai bằng lớp [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/)-bạn có thể chỉ định cách tổ chức các trang khi lưu vào hình ảnh:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) – chỉ lưu trang đầu tiên trong số các trang được chỉ định
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) – sắp xếp các trang theo dạng lưới, từ trái sang phải và từ trên xuống dưới, đồng thời chỉ định số cột
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) – sắp xếp các trang theo chiều ngang, cạnh nhau, từ trái sang phải, trong một đầu ra duy nhất
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) – sắp xếp các trang theo chiều dọc, trang này nằm dưới trang kia trong một đầu ra duy nhất
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) – sắp xếp mỗi trang dưới dạng một khung riêng biệt trong hình ảnh TIFF nhiều khung, chỉ áp dụng cho các định dạng hình ảnh TIFF 

Ví dụ mã sau đây cho thấy cách lưu tài liệu DOCX nhiều trang dưới dạng hình ảnh JPEG với bố Cục Ngang:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Bạn cũng có thể tùy chỉnh giao diện trang tệp đầu ra – chỉ định [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) và [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

Ví dụ mã sau đây cho thấy cách lưu tài liệu DOCX nhiều trang dưới dạng hình ảnh PNG với Bố Cục Lưới:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.PNG);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.setPageLayout(MultiPageLayout.grid(3, 10f, 10f));

// Customize the background and border.
options.getPageLayout().setBackColor(Color.lightGray);
options.getPageLayout().setBorderColor(Color.BLUE);
options.getPageLayout().setBorderWidth(2f);

doc.save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}