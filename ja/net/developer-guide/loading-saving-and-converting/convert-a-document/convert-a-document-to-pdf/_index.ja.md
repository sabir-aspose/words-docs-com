---
title: C#でWordをPDFに変換
second_title: Aspose.Words for .NET
articleTitle: ドキュメントをPDFに変更
linktitle: ドキュメントをPDFに変更
description: "C#でWordをPDFに変換。DOCXからPDFへの変換の簡単なコード例。すべてのWordフォーマットと画像をサポート。"
type: docs
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ja/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

文書をあるフォーマットから別のフォーマットに簡単かつ確実に変換する機能は、Aspose.Wordsの主要な機能です。PDFは変換で最も人気のあるフォーマットの1つです – 固定レイアウトフォーマットで、さまざまなプラットフォームでのレンダリング時に文書の元の外観を保持します。「レンダリング」という用語は、Aspose.Wordsでページ分割されたファイルフォーマットまたはページの概念を持つファイルフォーマットに文書を変換するプロセスを表すために使用されます。

## Word文書をPDFに変換

WordからPDFへの変換は、複数の計算段階を必要とする非常に複雑なプロセスです。Aspose.Wordsのレイアウトエンジンは、Microsoft Wordのページレイアウトエンジンの動作を模倣し、PDF出力文書をMicrosoft Wordで見ることができるものに可能な限り近づけます。

Aspose.Wordsを使用すると、Microsoft Officeを使用せずに、DOCやDOCXなどのWordフォーマットから文書をプログラムでPDFに変更できます。この記事では、この変換を実行する方法について説明します。

{{% alert color="primary" %}}

文書のページ数は変換時間に影響することに注意してください。

{{% /alert %}}

### DOCXまたはDOCをPDFに変換

Aspose.WordsでDOCまたはDOCXドキュメントフォーマットからPDFフォーマットへの変換は非常に簡単で、次の2行のコードで実行できます：

1. フォーマット拡張子を含むドキュメント名を指定して、コンストラクタの1つを使用してドキュメントを[Document](https://reference.aspose.com/words/net/aspose.words/document/)オブジェクトに読み込みます。
1. **Document**オブジェクトで[Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/)メソッドの1つを呼び出し、".PDF"拡張子を持つファイル名を入力してPDFとして希望の出力フォーマットを指定します。

次のコード例は、[Save](https://reference.aspose.com/words/net/aspose.words/document/save/)メソッドを使用してドキュメントをDOCXからPDFに変換する方法を示しています：

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

この例のテンプレートファイルは[Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx)からダウンロードできます。

{{% alert color="primary" %}}

時々、文書をPDFとして保存する結果に影響を与える可能性がある追加オプションを指定する必要があります。これらのオプションは、PDF出力の表示方法を決定するプロパティを含む[PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)クラスを使用して指定できます。

同じ技術により、任意の流動レイアウトフォーマットドキュメントをPDFフォーマットに変更できることに注意してください。

{{% /alert %}}

### 異なるPDF規格に変換

Aspose.Wordsは、DOCまたはDOCXをさまざまなPDFフォーマット規格（PDF 1.7、PDF 1.5など）に変換することをサポートする[PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/)列挙を提供します。

次のコード例は、PDF17準拠で[PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)を使用してドキュメントをPDF 1.7に変換する方法を示しています：

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## 画像をPDFに変換

PDFへの変換はMicrosoft Wordドキュメントフォーマットに制限されません。プログラムで作成されたものを含む、Aspose.Wordsでサポートされている任意のフォーマットもPDFに変更できます。たとえば、JPEG、PNG、BMP、EMF、WMFなどの単一ページ画像や、TIFFやGIFなどの複数ページ画像をPDFに変換できます。

次のコード例は、JPEG画像とTIFF画像をPDFに変更する方法を示しています：

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

このコードを動作させるには、プロジェクトにAspose.Wordsと`System.Drawing`への参照を追加する必要があります。

## PDF出力サイズの削減

PDFに保存する際、出力を最適化するかどうかを指定できます。これを行うには、[OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/)フラグをtrueに設定する必要があります。その後、冗長なネストされた空のキャンバスが削除され、同じフォーマットの隣接するグリフが連結されます。

次のコード例は、出力を最適化する方法を示しています：

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

**OptimizeOutput**プロパティの使用は、コンテンツ表示の精度に影響を与える可能性があります。

{{% /alert %}}

## 関連項目

- [レンダリング](/words/ja/net/rendering/)記事で、固定ページと流動レイアウトフォーマットの詳細情報
- [固定ページフォーマットへの変換](/words/ja/net/converting-to-fixed-page-format/#what-is-a-page-layout)記事で、ページレイアウトの詳細情報
- [PDFに変換する際のレンダリングオプションの指定](/words/ja/net/specify-rendering-options-when-converting-to-pdf/)記事で、`PdfSaveOptions`クラスの使用に関する詳細情報
- [PDF/AおよびPDF/UAへの変換機能について](/words/ja/net/learn-features-of-conversion-to-pdf-a-pdf-ua/)記事で、Aspose.WordsがサポートするPDF規格と関連するISO PDF規格について説明
- [選択すべきPDF規格](/words/ja/net/which-pdf-standard-is-better-to-choose/)記事で、どのPDF規格がどのケースに適しているかを判断

- [PDF/AまたはPDF/UAでの作業](/words/ja/net/working-with-pdfa-or-pdfua/)記事で、PDF/AおよびPDF/UAフォーマットでのドキュメントコンテンツの要件について説明 – 主に構造とフォントの要件

- [PDF/AおよびPDF/UAへの保存時のアクセシビリティ問題の警告](/words/ja/net/warnings-when-saving-to-pdfa-and-pdfua/)記事で、PDF/AとPDF/UAが課すコンテンツアクセシビリティ要件について説明
