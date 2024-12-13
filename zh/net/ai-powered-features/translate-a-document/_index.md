---
title: 翻译文档
second_title: Aspose.Words for .NET
articleTitle: 翻译文档
linktitle: 翻译文档
type: 文档
weight: 30
description: "翻译文档。Aspose.Words for .NET 使用 Google AI 模型简化文档翻译，允许您指定目标语言。"
url: /zh/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

文档翻译是高度数字化时代经常需要的选项。Aspose.Words 使用 *Google* 生成语言模型支持文档翻译，允许开发人员将文本内容翻译成 300 多种语言。

使用 [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) 方法将您的文档翻译成 [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) 枚举中表示的任何语言。请注意，如果源文档包含多种语言，则基于 Google AI 的模型将能够翻译所有支持的语言。如果模型无法识别某些文本片段中的语言，则将返回一份包含这些未翻译片段和其余文本已翻译的文档。

以下代码示例展示了如何使用 Aspose.Words 中的 *Gemini 1.5 Flash* 模型将文档翻译成阿拉伯语：

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

使用 Aspose.Words 翻译文档可节省时间，并可轻松将翻译功能集成到您的项目中。有关更多信息，请查看 [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API 文档。

{{% /alert %}}