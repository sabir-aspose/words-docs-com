---
title: AI Grammar Checking
second_title: Aspose.Words for C++
articleTitle: Grammar Checking
linktitle: Grammar Checking
type: docs
weight: 40
description: "Check a document grammar. Aspose.Words for C++ allows users to check grammar and detect errors in documents using OpenAI, Google, and Claude models."
url: /cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Checking grammar in documents is important to ensure clarity, professionalism, and accuracy. Well-written documents leave a positive impression and avoid misunderstandings. Grammar checks help identify and correct errors quickly, saving time and improving quality.

Aspose.Words allows users to check grammar and detect errors in documents using the OpenAI, Google, and Claude models' families listed in the [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/) enumeration. Use the [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/) method, available in the [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) namespace. **CheckGrammar** analyzes the text in a document and highlights grammatical problems.

The following code example shows how to use the GPT-4o mini model in Aspose.Words to check grammar:

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

Checking grammar with Aspose.Words improves the quality of your work and makes it easy to integrate proofreading into your projects. For more information, check the [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API documentation.

{{% /alert %}}