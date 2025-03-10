---
title: AI文法チェック
second_title: Aspose.WordsのためのPython via .NET
articleTitle: 文法チェック
linktitle: 文法チェック
type: docs
weight: 40
description: "文書の文法を確認してください。 Aspose.WordsのためのPython ユーザーはOpenAIモデルを使用して文法をチェックし、文書のエラーを検出できます。"
url: /ja/python-net/grammar-checking/
timestamp: 2025-01-15-16-40-05
---

文書の文法をチェックすることは、明快さ、プロ意識、正確さを確保するために重要です。 よく書かれた文書は肯定的な印象を残し、誤解を避ける。 文法チェックは、エラーを迅速に特定して修正するのに役立ち、時間を節約し、品質を向上させます。

Aspose.Wordsは、文法をチェックし、**OpenAI**生成モデルを使用して文書内のエラーを検出することができます。 [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)名前空間で使用できる[CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions)メソッドを使用します。 **CheckGrammar**は、文書内のテキストを分析し、文法上の問題を強調表示します。

次のコード例は、Aspose.WordsのGPT-4o miniモデルを使用して文法をチェックする方法を示しています:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + 'Big document.docx')

api_key = system_helper.environment.Environment.get_environment_variable('API_KEY')
# Use OpenAI generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GPT_4O_MINI).with_api_key(api_key).as_open_ai_model()

grammar_options = aw.ai.CheckGrammarOptions()
grammar_options.improve_stylistics = True

proofed_doc = model.check_grammar(doc, grammar_options)
proofed_doc.save(file_name='AI.AiGrammar.docx')
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Wordsで文法をチェックすると、作業の質が向上し、校正をプロジェクトに簡単に統合できます。 詳細については、[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)APIのドキュメントを確認してください。

{{% /alert %}}