---
title: 文書を翻訳する
second_title: Aspose.WordsのためのPython via .NET
articleTitle: 文書を翻訳する
linktitle: 文書を翻訳する
type: docs
weight: 30
description: "文書を翻訳します。 Aspose.WordsのためのPython GoogleAIモデルを使用して文書翻訳を簡素化し、ターゲット言語を指定できるようにします。"
url: /ja/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

文書翻訳は、高度なデジタル化の時代に頻繁に必要とされるオプションです。 Aspose.Wordsは、*Google*生成言語モデルを使用した文書翻訳をサポートし、開発者はテキストコンテンツを300以上の言語に翻訳することができます。

ドキュメントを[Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/)列挙体で表される任意の言語に変換するには、[Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language)メソッドを使用します。 ソース文書に複数の言語が含まれている場合、GoogleAIベースのモデルはサポートされているすべての言語を翻訳できることに注意してください。 モデルが一部のテキストフラグメントで言語を認識できない場合は、これらの翻訳されていないフラグメントと残りのテキストが翻訳された文書が返されます。

次のコード例は、Aspose.Wordsの*Gemini 1.5 Flash*モデルを使用して文書をアラビア語に翻訳する方法を示しています:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Wordsを使用して文書を翻訳すると、時間が節約され、翻訳機能をプロジェクトに簡単に統合できます。 詳細については、[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)APIのドキュメントを確認してください。

{{% /alert %}}