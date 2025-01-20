---
title: 翻译文档
second_title: Aspose.Words为.NET
articleTitle: 翻译文档
linktitle: 翻译文档
type: docs
weight: 30
description: "翻译文档。 Aspose.Words为.NET 使用GoogleAI模型简化文档翻译，允许您指定目标语言。"
url: /zh/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

在高度数字化的时代，文档翻译是一个经常需要的选择。 Aspose.Words支持使用*Google*生成语言模型的文档翻译，它允许开发人员将文本内容翻译成300多种语言。

使用[Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/)方法将文档翻译成[Language](https://reference.aspose.com/words/net/aspose.words.ai/language/)枚举中表示的任何语言。 请注意，如果源文档包含多种语言，则基于GoogleAI的模型将能够翻译所有支持的语言。 如果模型无法识别某些文本片段中的语言，那么您将返回一个包含这些未翻译片段并翻译其余文本的文档。

下面的代码示例演示如何使用Aspose.Words中的*Gemini 1.5 Flash*模型将文档翻译成阿拉伯语:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

使用Aspose.Words翻译文档可以节省时间，并且可以轻松地将翻译功能集成到您的项目中。 有关更多信息，请查看[Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)API文档。

{{% /alert %}}