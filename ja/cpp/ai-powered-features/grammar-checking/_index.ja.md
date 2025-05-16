---
title: AI文法チェック
second_title: Aspose.WordsのためのC++
articleTitle: 文法チェック
linktitle: 文法チェック
type: docs
weight: 40
description: "文書の文法を確認してください。 Aspose.WordsのためのC++ ユーザーはOpenAI、Google、Claudeモデルを使用して文法をチェックし、文書のエラーを検出できます。"
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ja/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

文書の文法をチェックすることは、明快さ、プロ意識、正確さを確保するために重要です。 よく書かれた文書は肯定的な印象を残し、誤解を避ける。 文法チェックは、エラーを迅速に特定して修正するのに役立ち、時間を節約し、品質を向上させます。

Aspose.Wordsを使用すると、ユーザーは[AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/)列挙にリストされているOpenAI、Google、およびClaudeモデルのファミリを使用して、文法をチェックし、文書のエラーを検出できます。 [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)名前空間で使用できる[CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/)メソッドを使用します。 **CheckGrammar**は、文書内のテキストを分析し、文法上の問題を強調表示します。

次のコード例は、Aspose.WordsのGPT-4o miniモデルを使用して文法をチェックする方法を示しています:

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

Aspose.Wordsで文法をチェックすると、作業の質が向上し、校正をプロジェクトに簡単に統合できます。 詳細については、[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)APIのドキュメントを確認してください。

{{% /alert %}}