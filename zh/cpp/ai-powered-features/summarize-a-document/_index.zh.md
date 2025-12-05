---
title: 总结文档
second_title: Aspose.Words为C++
articleTitle: 总结文档
linktitle: 总结文档
type: docs
weight: 20
description: "总结一个文档。 Aspose.Words为C++ 通过允许您指定摘要长度，使用OpenAI和GoogleAI模型简化文档摘要。"
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /zh/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

摘要文档是内容审查，快速见解或准备摘要的宝贵工具。 Aspose.Words支持使用AI支持的模型进行文档摘要，从而更容易处理长文本。 此功能在[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)命名空间中可用，集成了来自*OpenAI*和*Google*的高级生成语言模型以及*Claude's*人类生成语言模型。 支持的模型列表在[AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/)枚举中可用。

您可以指定用于汇总文档内容的各种选项。 使用[Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/)方法生成文档摘要。 您还可以使用[SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/)属性设置摘要长度。

使用Aspose.Words，实现文档摘要非常简单。 下面的代码示例演示如何使用GPT-4o模型汇总文档:

{{< highlight cpp >}}
void AiSummarize()
{
    auto firstDoc = MakeObject<Document>(MyDir + u"Big document.docx");
    auto secondDoc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"))->WithOrganization(u"Organization")->WithProject(u"Project");

    auto options = MakeObject<SummarizeOptions>();

    options->set_SummaryLength(SummaryLength::Short);
    auto firstDocumentSummary = model->Summarize(firstDoc, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.One.docx");

    System::ArrayPtr<System::SharedPtr<Document>> documents = System::MakeArray<System::SharedPtr<Document>>(2);
    documents[0] = firstDoc;
    documents[1] = secondDoc;

    options->set_SummaryLength(SummaryLength::Long);
    auto multiDocumentSummary = model->Summarize(documents, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.Multi.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

使用Aspose.Words汇总文档可以节省时间并帮助您专注于基本信息。 有关更多信息，请查看[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)API文档。

{{% /alert %}}
