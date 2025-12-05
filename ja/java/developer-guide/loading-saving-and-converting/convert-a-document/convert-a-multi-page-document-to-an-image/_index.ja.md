---
title: 複数ページの文書をJava内の画像に変換する
second_title: Aspose.WordsのためのJava
articleTitle: 複数ページのドキュメントを画像に変換する
linktitle: 複数ページのドキュメントを画像に変換する
type: docs
description: "複数ページのドキュメントをラスターイメージにエクスポートする(JPG, PNG, GIF, BMP, TIFF, WebP) Javaを使用します。"
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ja/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.WordsforJavaを使用すると、ユーザーは複数ページのドキュメントをラスターイメージに書き出すことができます。 これは、編集不可能な使用のためにドキュメントのプレビュー、アーカイブ、または視覚的な表現を生成するのに役立ちます。

## 複数ページのエクスポートをサポートする形式は何ですか？

Aspose.Wordsは、次のラスターイメージ形式へのマルチページエクスポートをサポートします:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## 複数ページのドキュメントを画像にエクスポートする方法

複数ページのドキュメントを画像にエクスポートする機能は[MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/)クラスを使用して実装されています–画像に保存するときにページをどのように整理す:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage)–指定されたページの最初のページのみを保存します
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float)-列の数を指定しながら、ページを左から右、上から下にグリッドに配置します
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float)–単一の出力でページを水平に並べ、左から右に配置します
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float)-単一の出力でページを上下に垂直に配置します
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames)-各ページをマルチフレームTIFF画像内の個別のフレームとして配置します。TIFF画像形式にのみ適用されます

次のコード例は、複数ページDOCXドキュメントを水平レイアウトでJPEGイメージとして保存する方法を示しています:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

出力ファイルのページの外観をカスタマイズすることもできます–[BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor)、[BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor)、および[BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth)を指定します。

次のコード例は、グリッドレイアウトを使用して複数ページDOCXドキュメントをPNGイメージとして保存する方法を示しています:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.PNG);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.setPageLayout(MultiPageLayout.grid(3, 10f, 10f));

// Customize the background and border.
options.getPageLayout().setBackColor(Color.lightGray);
options.getPageLayout().setBorderColor(Color.BLUE);
options.getPageLayout().setBorderWidth(2f);

doc.save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}