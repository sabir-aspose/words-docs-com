---
title: AI语法检查
second_title: Aspose.Words为Java
articleTitle: 语法检查
linktitle: 语法检查
type: docs
weight: 40
description: "检查文档语法。 Aspose.Words为Java 允许用户使用OpenAI，Google和Claude模型检查语法并检测文档中的错误。"
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /zh/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

检查文档中的语法对于确保清晰度，专业性和准确性非常重要。 写得好的文件给人留下积极的印象,避免误解. 语法检查有助于快速识别和纠正错误，节省时间并提高质量。

Aspose.Words允许用户使用[AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/)枚举中列出的OpenAI，Google和Claude模型系列检查语法并检测文档中的错误。 使用[CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions)方法分析文档中的文本并突出显示语法问题。

下面的代码示例演示如何使用Aspose.Words中的GPT-4o mini模型来检查语法:

{{< highlight java >}}
 Document doc = new Document("Big document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI generative language models.
 IAiModelText model = (OpenAiModel)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
 grammarOptions.setImproveStylistics(true);

 Document proofedDoc = model.checkGrammar(doc, grammarOptions);
 proofedDoc.save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

使用Aspose.Words检查语法可以提高工作质量，并可以轻松地将校对集成到项目中。 有关更多信息，请检查[Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/)。

{{% /alert %}}