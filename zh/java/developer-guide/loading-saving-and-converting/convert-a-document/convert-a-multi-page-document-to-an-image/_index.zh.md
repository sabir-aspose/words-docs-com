---
title: 将多页文档转换为Java中的图像
second_title: Aspose.Words为Java
articleTitle: 将多页文档转换为图像
linktitle: 将多页文档转换为图像
type: docs
description: "将多页文档导出为光栅图像(JPG, PNG, GIF, BMP, TIFF, WebP) 使用Java。"
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /zh/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.WordsforJava允许用户将多页文档导出为光栅图像。 这对于生成预览、存档或文档的可视化表示以供不可编辑使用非常有用。

## 什么格式支持多页导出？

Aspose.Words支持将多页导出为以下栅格图像格式:

* Jpeg格式
* Gif
* 巴布亚新几内亚
* Bmp
* 蒂夫
* WebP

## 如何将多页文档导出到图像

将多页文档导出到图像的功能是使用[MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/)类实现的–您可以指定保存到图像时应如何组织页面:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage)-只保存指定的第一个页面
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float)-在网格中排列页面，从左到右和从上到下，同时指定列数
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float)-在单个输出中水平并排，从左到右排列页面
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float)-在单个输出中垂直排列页面
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames)-在多帧TIFF图像中将每个页面排列为单独的帧，仅适用于TIFF图像格式

下面的代码示例演示如何将多页DOCX文档保存为具有水平布局的JPEG图像:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

您还可以自定义输出文件页面外观-指定[BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor)、[BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor)和[BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth)。

下面的代码示例演示如何使用网格布局将多页DOCX文档保存为PNG图像:

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