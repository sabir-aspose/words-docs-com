---
title: 文書を翻訳する
second_title: Aspose.Wordsのための.NET
articleTitle: 文書を翻訳する
linktitle: 文書を翻訳する
type: docs
weight: 30
description: "文書を翻訳します。 Aspose.Wordsのための.NET GoogleAIモデルを使用して文書翻訳を簡素化し、ターゲット言語を指定できるようにします。"
url: /ja/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

文書翻訳は、高度なデジタル化の時代に頻繁に必要とされるオプションです。 Aspose.Wordsは、*Google*生成言語モデルを使用した文書翻訳をサポートし、開発者はテキストコンテンツを300以上の言語に翻訳することができます。

ドキュメントを[Language](https://reference.aspose.com/words/net/aspose.words.ai/language/)列挙体で表される任意の言語に変換するには、[Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/)メソッドを使用します。 ソース文書に複数の言語が含まれている場合、GoogleAIベースのモデルはサポートされているすべての言語を翻訳できることに注意してください。 モデルが一部のテキストフラグメントで言語を認識できない場合は、これらの翻訳されていないフラグメントと残りのテキストが翻訳された文書が返されます。

次のコード例は、Aspose.Wordsの*Gemini 1.5 Flash*モデルを使用して文書をアラビア語に翻訳する方法を示しています:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Wordsを使用して文書を翻訳すると、時間が節約され、翻訳機能をプロジェクトに簡単に統合できます。 詳細については、[Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)APIのドキュメントを確認してください。

{{% /alert %}}