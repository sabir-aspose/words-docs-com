---
title: AI语法检查
second_title: Aspose.Words为C++
articleTitle: 语法检查
linktitle: 语法检查
type: docs
weight: 40
description: "检查文档语法。 Aspose.Words为C++ 允许用户使用OpenAI，Google和Claude模型检查语法并检测文档中的错误。"
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /zh/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

检查文档中的语法对于确保清晰度，专业性和准确性非常重要。 写得好的文件给人留下积极的印象,避免误解. 语法检查有助于快速识别和纠正错误，节省时间并提高质量。

Aspose.Words允许用户使用[AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/)枚举中列出的OpenAI，Google和Claude模型系列检查语法并检测文档中的错误。 使用[CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/)方法，在[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)命名空间中可用。 **CheckGrammar**分析文档中的文本并突出语法问题。

下面的代码示例演示如何使用Aspose.Words中的GPT-4o mini模型来检查语法:

{{< highlight cpp >}}
void AiGrammar()
{
    auto doc = MakeObject<Document>(MyDir + u"Big document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto grammarOptions = MakeObject<CheckGrammarOptions>();
    grammarOptions->set_ImproveStylistics(true);

    auto proofedDoc = model->CheckGrammar(doc, grammarOptions);
    proofedDoc->Save(ArtifactsDir + u"AI.AiGrammar.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

使用Aspose.Words检查语法可以提高工作质量，并可以轻松地将校对集成到项目中。 有关更多信息，请查看[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)API文档。

{{% /alert %}}