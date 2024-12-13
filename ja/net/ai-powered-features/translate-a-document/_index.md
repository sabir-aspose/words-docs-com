---
title: ドキュメントを翻訳する
second_title: Aspose.Words for .NET
articleTitle: ドキュメントを翻訳する
linktitle: ドキュメントを翻訳する
type: docs
weight: 30
description: "ドキュメントを翻訳します。Aspose.Words for .NET は、Google AI モデルを使用してドキュメントの翻訳を簡素化し、ターゲット言語を指定できるようにします。"
url: /ja/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

ドキュメントの翻訳は、高度なデジタル化の時代に頻繁に必要とされるオプションです。Aspose.Words は、*Google* 生成言語モデルを使用したドキュメントの翻訳をサポートしており、開発者はテキスト コンテンツを 300 を超える言語に翻訳できます。

[Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) メソッドを使用して、ドキュメントを [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) 列挙体で表される任意の言語に翻訳します。ソース ドキュメントに複数の言語が含まれている場合、Google AI ベースのモデルはサポートされているすべての言語を翻訳できることに注意してください。モデルが一部のテキスト フラグメントの言語を認識できない場合は、これらの未翻訳フラグメントと残りのテキストが翻訳されたドキュメントが返されます。

次のコード例は、Aspose.Words で *Gemini 1.5 Flash* モデルを使用してドキュメントをアラビア語に翻訳する方法を示しています:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Words を使用してドキュメントを翻訳すると、時間が節約され、プロジェクトに翻訳機能を簡単に統合できます。詳細については、[Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API ドキュメントを確認してください。

{{% /alert %}}