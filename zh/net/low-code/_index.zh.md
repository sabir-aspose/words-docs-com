---
title: Low Code
second_title: Aspose.Words为.NET
articleTitle: 使用LowCodeAPI处理文档
linktitle: Low Code
type: docs
description: "使用Low CodeAPI简化比较、转换、拆分、合并、查找和替换等文档处理任务。 Aspose.WordsLowCodeAPI具有简洁的语法，快速的结果和最小的编码努力。"
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /zh/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words为.NET 提供[Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/)命名空间，可简化常见的文档处理任务。 此API专为希望以最小的努力完成文档比较，内容提取，图像转换和文本替换等高级操作的开发人员而设计。

LowCodeAPI非常适合快速实现比细粒度控制更重要的场景。 让我们仔细看看LowCode功能 Aspose.Words为.NET.

{{% alert color="primary" %}}

需要注意的是，LowCodeAPI不允许您更改文档结构。

{{% /alert %}}

## LowCodeAPI中的可用特性

`Aspose.Words.LowCode`命名空间当前支持:

* **Converting**从一种格式到另一种格式的文档
* **Comparing**文件
* **Mail merging**
* **Reporting**基于LINQ语法
* **Merging**文件
* **Search and replace**
* **Digital signing**文件
* **Splitting**使用不同标准将文档分成多个部分
* 添加**watermark**

{{% alert color="primary" %}}

请注意，可以在开发人员指南部分中找到Low Code之外的每个功能的详细描述。

{{% /alert %}}

## 流利和非流利API

Aspose.Words为.NET 支持Fluent和Non-FluentAPIs，允许开发人员选择最适合其编码偏好和项目需求的样式。 让我们看看一些例子，看看这两种类型的API是如何不同的。

{{% alert color="primary" %}}

在FluentAPI中，可以通过上下文（如ComparerContext或ReplacerContext）配置和执行操作。 此上下文包含常用选项。 它确保所有相关方法以一致的配置运行，使API功能强大，易于在复杂场景中管理。

{{% /alert %}}

### 比较文件

使用`LowCode`比较两个Word文档并保存结果。

**非fluent api示例:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**fluent api示例:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

您也可以通过`CompareOptions`进行微调比较。

**非fluent api示例:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

CompareOptions options = new CompareOptions
{
    IgnoreFormatting = true,
    IgnoreCaseChanges = true
};

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc, options);
{{< /highlight >}}

**fluent api示例:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

ComparerContext comparerContext = new ComparerContext();
comparerContext.CompareOptions.IgnoreCaseChanges = true;

Comparer.Create(comparerContext)
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.3.docx")
   .Execute();
{{< /highlight >}}

### 将文档转换为图像

使用`LowCode`将Word文档转换为PDF。

**非fluent api示例:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**fluent api示例:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### 查找和替换文本

使用`LowCode`快速替换整个文档中的文本。

**非fluent api示例:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**fluent api示例:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";

ReplacerContext replacerContext = new ReplacerContext();
replacerContext.SetReplacement("ReplaceMe", "Replacement");

Replacer.Create(replacerContext)
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

## 为什么使用Aspose.WordsLow Code

**Aspose.Words.LowCode**命名空间可帮助您使用干净、可读的语法快速实现高级文档处理任务。 它对于在处理Word文档时需要速度，简单性和可维护代码的开发人员尤其有用。

要探索更高级的选项，您始终可以将LowCodeAPIs与完整的Aspose.Words对象模型结合使用。 在[API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/)中查看更多Low Code示例。