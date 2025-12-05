---
title: Chuyển Đổi Tài liệu Nhiều trang thành Hình ảnh trong Python
second_title: Aspose.Words cho Python
articleTitle: Chuyển Đổi Tài liệu Nhiều trang thành Hình Ảnh
linktitle: Chuyển Đổi Tài liệu Nhiều trang thành Hình Ảnh
type: docs
description: "Xuất tài liệu nhiều trang sang hình ảnh raster(JPG, PNG, GIF, BMP, TIFF, WebP) sử dụng Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /vi/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words cho Python via .NET cho phép người dùng xuất tài liệu nhiều trang sang hình ảnh raster. Điều này có thể hữu ích để tạo bản xem trước, lưu trữ hoặc biểu diễn trực quan các tài liệu để sử dụng không thể chỉnh sửa.

## Những Định dạng Nào Hỗ trợ Xuất Nhiều trang?

Aspose.Words hỗ trợ xuất nhiều trang sang các định dạng hình ảnh raster sau:

* Jpeg
* Gio
* Tg
* Bt
* Tiff
* WebP

## Cách Xuất Tài liệu Nhiều trang Sang Hình Ảnh

Tính năng xuất tài liệu nhiều trang sang hình ảnh được triển khai bằng lớp [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/)-bạn có thể chỉ định cách tổ chức các trang khi lưu vào hình ảnh:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) – chỉ lưu trang đầu tiên trong số các trang được chỉ định
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) – sắp xếp các trang theo dạng lưới, từ trái sang phải và từ trên xuống dưới, đồng thời chỉ định số cột
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) – sắp xếp các trang theo chiều ngang, cạnh nhau, từ trái sang phải, trong một đầu ra duy nhất
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) – sắp xếp các trang theo chiều dọc, trang này nằm dưới trang kia trong một đầu ra duy nhất
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) – sắp xếp mỗi trang dưới dạng một khung riêng biệt trong hình ảnh TIFF nhiều khung, chỉ áp dụng cho các định dạng hình ảnh TIFF 

Ví dụ mã sau đây cho thấy cách lưu tài liệu DOCX nhiều trang dưới dạng hình ảnh JPEG với bố Cục Ngang:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Bạn cũng có thể tùy chỉnh giao diện trang tệp đầu ra – chỉ định [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) và [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

Ví dụ mã sau đây cho thấy cách lưu tài liệu DOCX nhiều trang dưới dạng hình ảnh PNG với Bố Cục Lưới:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.PNG)
# Set up a grid layout with:
# - 3 columns per row.
# - 10pts spacing between pages (horizontal and vertical).
options.page_layout = aw.saving.MultiPageLayout.grid(3, 10, 10)

# Customize the background and border.
options.page_layout.back_color = aspose.pydrawing.Color.light_gray
options.page_layout.border_color = aspose.pydrawing.Color.blue
options.page_layout.border_width = 2

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}