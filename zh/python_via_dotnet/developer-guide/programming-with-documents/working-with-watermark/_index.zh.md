---
title: 在Python中使用水印
second_title: Aspose.Words为Python via .NET
articleTitle: 使用水印
linktitle: 使用水印
description: "使用Python在文档中创建和管理水印。"
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /zh/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

本主题讨论如何使用Aspose.Words以编程方式处理水印。 水印是在文档中的文本后面显示的背景图像。 水印可以包含由[Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/)类表示的文本或图像。

{{% alert color="primary" %}}

**在线试用**

您可以使用我们的 [免费在线文档水印](https://products.aspose.app/words/watermark).

{{% /alert %}}

## 如何为文档添加水印

在Microsoft Word中，可以使用Insert Watermark命令轻松地在文档中插入水印。 Aspose.Words提供[Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/)类以在文档中添加或删除水印。 Aspose.Words提供[WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/)枚举，定义要使用的三种可能类型的水印（[TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text)、[IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image)和[NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)）。

### 添加文字水印

下面的代码示例演示如何通过使用[set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/)方法定义[TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/)在文档中插入文本水印:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### 添加图像水印

下面的代码示例演示如何通过使用[set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/)方法定义[ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/)在文档中插入图像水印:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

图像水印可以作为图像、字符串或流插入.

水印也可以使用形状类插入。 将任何形状或图像插入页眉或页脚非常容易，从而创建任何可以想象的类型的水印。

下面的代码示例将水印插入到Word文档中:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

您可以从以下位置下载此示例的模板文件 [这里](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## 从文档中删除水印

[Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/)类提供remove方法从文档中删除水印。

下面的代码示例演示如何从文档中删除水印:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

如果使用[Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/)类对象添加水印，那么要从文档中删除水印，您必须在插入过程中仅设置水印形状的名称，然后通过指定的名称删除水印形状。

下面的代码示例演示如何设置水印形状的名称并将其从文档中删除:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## 在表格单元格中添加水印

有时您需要将水印/图像插入表格的单元格并将其显示在表格之外，您可以使用[is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/)属性。 此属性获取或设置一个标志，该标志指示形状是显示在表内部还是表外部。 请注意，仅当您使用[optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/)方法优化Microsoft Word2010的文档时，此属性才有效。

下面的代码示例演示如何使用此属性:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
