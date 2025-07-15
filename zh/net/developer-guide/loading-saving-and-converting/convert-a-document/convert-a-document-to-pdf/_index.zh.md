---
title: 在 C# 中将 Word 转换为 PDF
second_title: Aspose.Words for .NET
articleTitle: 将文档转化为 PDF
linktitle: 将文档转化为 PDF
description: "在 C# 中将 Word 转换为 PDF。DOCX 转 PDF 的简单代码示例。支持所有 Word 格式和图片。"
type: docs
weight: 10
url: /zh/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

轻松可靠地将文档从一种格式转换为另一种格式的能力是 Aspose.Words 的核心功能。PDF 是最受欢迎的转换格式之一——它是一种固定布局格式，在不同平台上渲染时保持文档的原始外观。术语"渲染"在 Aspose.Words 中用于描述将文档转化为分页文件格式或具有页面概念的文件格式的过程。

## 将 Word 文档转换为 PDF

从 Word 转换为 PDF 是一个相当复杂的过程，需要多个计算阶段。Aspose.Words 布局引擎模仿 Microsoft Word 页面布局引擎的工作方式，使输出的 PDF 文档看起来尽可能接近您在 Microsoft Word 中看到的内容。

使用 Aspose.Words，您可以编程方式将文档从 Word 格式（如 DOC 或 DOCX）转化为 PDF，而无需使用 Microsoft Office。本文解释了如何执行此转换。

{{% alert color="primary" %}}

注意，文档中的页面数量会影响转换时间。

{{% /alert %}}

### 将 DOCX 或 DOC 转换为 PDF

在 Aspose.Words 中将 DOC 或 DOCX 文档格式转化为 PDF 格式非常简单，只需两行代码即可完成：

1. 使用其构造函数之一将文档加载到 [Document](https://reference.aspose.com/words/net/aspose.words/document/) 对象中，通过指定文档名称及其格式扩展名。
1. 在 **Document** 对象上调用 [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) 方法之一，通过输入带有".PDF"扩展名的文件名来指定所需的输出格式为 PDF。

以下代码示例显示了如何使用 [Save](https://reference.aspose.com/words/net/aspose.words/document/save/) 方法将文档从 DOCX 转换为 PDF：

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

您可以从 [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx) 下载此示例的模板文件。

{{% alert color="primary" %}}

有时需要指定可能影响将文档保存为 PDF 结果的附加选项。这些选项可以通过使用 [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) 类来指定，该类包含确定 PDF 输出显示方式的属性。

请注意，使用相同的技术，您可以将任何流式布局格式的文档变换为 PDF 格式。

{{% /alert %}}

### 转化为不同的 PDF 标准

Aspose.Words 提供 [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) 枚举来支持将 DOC 或 DOCX 转换为各种 PDF 格式标准（如 PDF 1.7、PDF 1.5 等）。

以下代码示例演示如何使用 [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) 并符合 PDF17 标准将文档转换为 PDF 1.7：

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## 将图像转换为 PDF

转换为 PDF 并不限于 Microsoft Word 文档格式。Aspose.Words 支持的任何格式，包括以编程方式创建的格式，也可以转化为 PDF。例如，我们可以将单页图像（如 JPEG、PNG、BMP、EMF 或 WMF）以及多页图像（如 TIFF 和 GIF）转换为 PDF。

以下代码示例显示了如何将 JPEG 和 TIFF 图像变换为 PDF：

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

要使此代码正常工作，您需要在项目中添加对 Aspose.Words 和 `System.Drawing` 的引用。

## 减少 PDF 输出大小

保存为 PDF 时，您可以指定是否要优化输出。为此，您需要将 [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) 标志设置为 true，然后将删除冗余的嵌套和空白画布，相邻的具有相同格式的字形将被连接。

以下代码示例显示了如何优化输出：

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

使用 **OptimizeOutput** 属性可能会影响内容显示的准确性。

{{% /alert %}}

## 另请参阅

- 文章 [渲染](/words/zh/net/rendering/) 了解有关固定页面和流式布局格式的更多信息
- 文章 [转换为固定页面格式](/words/net/converting-to-fixed-page-format/#what-is-a-page-layout) 了解有关页面布局的更多信息
- 文章 [转化为 PDF 时指定渲染选项](/words/zh/net/specify-rendering-options-when-converting-to-pdf/) 了解有关使用 `PdfSaveOptions` 类的更多信息
- 文章 [了解转换为 PDF/A 和 PDF/UA 的功能](/words/zh/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) 描述了 Aspose.Words 支持的 PDF 标准和 PDF 标准的相关 ISO
- 文章 [选择哪种 PDF 标准更好](/words/zh/net/which-pdf-standard-is-better-to-choose/) 确定哪些 PDF 标准适合哪些情况

- 文章 [使用 PDF/A 或 PDF/UA](/words/zh/net/working-with-pdfa-or-pdfua/) 描述了 PDF/A 和 PDF/UA 格式中文档内容的要求——主要是结构和字体的要求

- 文章 [保存为 PDF/A 和 PDF/UA 时的可访问性问题警告](/words/zh/net/warnings-when-saving-to-pdfa-and-pdfua/) 描述了 PDF/A 和 PDF/UA 对内容可访问性的要求
