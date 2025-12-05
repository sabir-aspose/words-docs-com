---
title: Chuyển Đổi Tài liệu Nhiều trang thành Hình ảnh trong C#
second_title: Aspose.Words cho .NET
articleTitle: Chuyển Đổi Tài liệu Nhiều trang thành Hình Ảnh
linktitle: Chuyển Đổi Tài liệu Nhiều trang thành Hình Ảnh
type: docs
description: "Xuất tài liệu nhiều trang sang hình ảnh raster(JPG, PNG, GIF, BMP, TIFF, WebP) sử dụng C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /vi/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words cho .NET cho phép người dùng xuất tài liệu nhiều trang sang hình ảnh raster. Điều này có thể hữu ích để tạo bản xem trước, lưu trữ hoặc biểu diễn trực quan các tài liệu để sử dụng không thể chỉnh sửa.

## Những Định dạng Nào Hỗ trợ Xuất Nhiều trang?

Aspose.Words hỗ trợ xuất nhiều trang sang các định dạng hình ảnh raster sau:

* Jpeg
* Gio
* Tg
* Bt
* Tiff
* WebP

## Cách Xuất Tài liệu Nhiều trang Sang Hình Ảnh

Tính năng xuất tài liệu nhiều trang sang hình ảnh được triển khai bằng lớp [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/)-bạn có thể chỉ định cách tổ chức các trang khi lưu vào hình ảnh:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) – chỉ lưu trang đầu tiên trong số các trang được chỉ định
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) – sắp xếp các trang theo dạng lưới, từ trái sang phải và từ trên xuống dưới, đồng thời chỉ định số cột
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) – sắp xếp các trang theo chiều ngang, cạnh nhau, từ trái sang phải, trong một đầu ra duy nhất
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) – sắp xếp các trang theo chiều dọc, trang này nằm dưới trang kia trong một đầu ra duy nhất
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) – sắp xếp mỗi trang dưới dạng một khung riêng biệt trong hình ảnh TIFF nhiều khung, chỉ áp dụng cho các định dạng hình ảnh TIFF 

Ví dụ mã sau đây cho thấy cách lưu tài liệu DOCX nhiều trang dưới dạng hình ảnh JPEG với bố Cục Ngang:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Bạn cũng có thể tùy chỉnh giao diện trang tệp đầu ra – chỉ định [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) và [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

Ví dụ mã sau đây cho thấy cách lưu tài liệu DOCX nhiều trang dưới dạng hình ảnh PNG với Bố Cục Lưới:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Png);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.PageLayout = MultiPageLayout.Grid(3, 10, 10);

// Customize the background and border.
options.PageLayout.BackColor = Color.LightGray;
options.PageLayout.BorderColor = Color.Blue;
options.PageLayout.BorderWidth = 2;

doc.Save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}