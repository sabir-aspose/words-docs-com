---
title: Low Code
second_title: Aspose.Wordsのための.NET
articleTitle: LowCodeAPIを使用した文書の操作
linktitle: Low Code
type: docs
description: "比較、変換、分割、マージ、検索、置換などの文書処理タスクをLow CodeAPIを使用して簡素化します。 Aspose.WordsLowCodeAPIクリーンな構文、高速な結果、最小限のコーディング労力を備えています。"
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ja/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Wordsのための.NET 一般的な文書処理タスクを簡素化する[Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/)名前空間を提供します。 このAPIは、ドキュメント比較、コンテンツ抽出、画像変換、テキスト置換などの高レベルの操作を最小限の労力で実行したい開発者向けに設計されてい

LowCodeAPIは、きめ細かい制御よりも迅速な実装が重要なシナリオに最適です。 のLowCode機能を詳しく見てみましょう Aspose.Wordsのための.NET.

{{% alert color="primary" %}}

LowCodeAPIでは文書構造を変更できないことに注意することが重要です。

{{% /alert %}}

## LowCodeAPIで利用可能な機能

`Aspose.Words.LowCode`名前空間は現在サポートしています:

* **Converting**ある形式から別の形式への文書
* **Comparing**ドキュメント
* **Mail merging**
* LINQ構文に基づく**Reporting**
* **Merging**ドキュメント
* **Search and replace**
* ドキュメントの**Digital signing**
* **Splitting**異なる基準を使用した部品への文書
* **watermark**を追加する

{{% alert color="primary" %}}

Low Code以外の各関数の詳細な説明は、開発者ガイドのセクションにあります。

{{% /alert %}}

## 流暢なものと非流暢なものAPI

Aspose.Wordsのための.NET 流暢なAPIsと非流暢なAPIsの両方をサポートし、開発者はコーディングの好みやプロジェクトのニーズに最も適したスタイルを選択できます。 いくつかの例を見て、これら2つのタイプのAPIがどのように異なるかを見てみましょう。

{{% alert color="primary" %}}

FluentAPIでは、操作はコンテキスト(ComparerContextやReplacerContextなど)を介して構成および実行できます。 このコンテキストには、一般的なオプションが含まれます。 これにより、関連するすべてのメソッドが一貫した構成で動作することが保証され、APIは強力で複雑なシナリオで管理が容易になります。

{{% /alert %}}

### 文書の比較

2つのWord文書を比較して結果を保存するには`LowCode`を使用します。

**非流暢なapiの例:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**fluent apiの例:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

また、微調整された比較のために`CompareOptions`を渡すこともできます。

**非流暢なapiの例:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

CompareOptions options = new CompareOptions
{
    IgnoreFormatting = true,
    IgnoreCaseChanges = true
};

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc, options);
{{< /highlight >}}

**fluent apiの例:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

ComparerContext comparerContext = new ComparerContext();
comparerContext.CompareOptions.IgnoreCaseChanges = true;

Comparer.Create(comparerContext)
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.3.docx")
   .Execute();
{{< /highlight >}}

### 文書を画像に変換する

`LowCode`を使用してWord文書をPDFに変換します。

**非流暢なapiの例:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**fluent apiの例:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### テキストの検索と置換

`LowCode`を使用すると、文書全体のテキストをすばやく置換できます。

**非流暢なapiの例:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**fluent apiの例:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";

ReplacerContext replacerContext = new ReplacerContext();
replacerContext.SetReplacement("ReplaceMe", "Replacement");

Replacer.Create(replacerContext)
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

## なぜAspose.WordsLow Codeを使うのか

**Aspose.Words.LowCode**名前空間は、きれいで読みやすい構文で高レベルの文書処理タスクを迅速に実装するのに役立ちます。 これは、Wordドキュメントを操作するときに速度、シンプルさ、保守可能なコードを必要とする開発者にとって特に便利です。

より高度なオプションを探索するには、LowCodeAPIsと完全なAspose.Wordsオブジェクトモデルをいつでも組み合わせることができます。 [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/)のより多くのLow Codeの例を参照してください。