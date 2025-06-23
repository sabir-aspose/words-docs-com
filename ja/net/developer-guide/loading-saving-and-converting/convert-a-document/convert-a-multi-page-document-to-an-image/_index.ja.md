---
title: 複数ページの文書をC#内の画像に変換する
second_title: Aspose.Wordsのための.NET
articleTitle: 複数ページのドキュメントを画像に変換する
linktitle: 複数ページのドキュメントを画像に変換する
type: docs
description: "複数ページのドキュメントをラスターイメージにエクスポートする(JPG, PNG, GIF, BMP, TIFF, WebP) C#を使用します。"
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ja/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Wordsfor.NETを使用すると、ユーザーは複数ページのドキュメントをラスターイメージに書き出すことができます。 これは、編集不可能な使用のためにドキュメントのプレビュー、アーカイブ、または視覚的な表現を生成するのに役立ちます。

## 複数ページのエクスポートをサポートする形式は何ですか？

Aspose.Wordsは、次のラスターイメージ形式へのマルチページエクスポートをサポートします:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## 複数ページのドキュメントを画像にエクスポートする方法

複数ページのドキュメントを画像にエクスポートする機能は[MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/)クラスを使用して実装されています–画像に保存するときにページをどのように整理す:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/)–指定されたページの最初のページのみを保存します
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/)-列の数を指定しながら、ページを左から右、上から下にグリッドに配置します
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/)–単一の出力でページを水平に並べ、左から右に配置します
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/)-単一の出力でページを上下に垂直に配置します
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/)-各ページをマルチフレームTIFF画像内の個別のフレームとして配置します。TIFF画像形式にのみ適用されます

次のコード例は、複数ページDOCXドキュメントを水平レイアウトでJPEGイメージとして保存する方法を示しています:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

出力ファイルのページの外観をカスタマイズすることもできます–[BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/)、[BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/)、および[BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/)を指定します。

次のコード例は、グリッドレイアウトを使用して複数ページDOCXドキュメントをPNGイメージとして保存する方法を示しています:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Png);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.PageLayout = MultiPageLayout.Grid(3, 10, 10);

// Customize the background and border.
options.PageLayout.BackColor = Color.LightGray;
options.PageLayout.BorderColor = Color.Blue;
options.PageLayout.BorderWidth = 2;

doc.Save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}