---
title: 将多页文档转换为Python中的图像
second_title: Aspose.Words为Python
articleTitle: 将多页文档转换为图像
linktitle: 将多页文档转换为图像
type: docs
description: "将多页文档导出为光栅图像(JPG, PNG, GIF, BMP, TIFF, WebP) 使用Python。"
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /zh/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.WordsforPython via .NET允许用户将多页文档导出为光栅图像。 这对于生成预览、存档或文档的可视化表示以供不可编辑使用非常有用。

## 什么格式支持多页导出？

Aspose.Words支持将多页导出为以下栅格图像格式:

* Jpeg格式
* Gif
* 巴布亚新几内亚
* Bmp
* 蒂夫
* WebP

## 如何将多页文档导出到图像

将多页文档导出到图像的功能是使用[MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/)类实现的–您可以指定保存到图像时应如何组织页面:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/)-只保存指定的第一个页面
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float)-在网格中排列页面，从左到右和从上到下，同时指定列数
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float)-在单个输出中水平并排，从左到右排列页面
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float)-在单个输出中，将页面垂直排列在另一个下方
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/)-在多帧TIFF图像中将每个页面排列为单独的帧，仅适用于TIFF图像格式

下面的代码示例演示如何将多页DOCX文档保存为具有水平布局的JPEG图像:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

您还可以自定义输出文件页面外观-指定[back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/)、[border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/)和[border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/)。

下面的代码示例演示如何使用网格布局将多页DOCX文档保存为PNG图像:

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