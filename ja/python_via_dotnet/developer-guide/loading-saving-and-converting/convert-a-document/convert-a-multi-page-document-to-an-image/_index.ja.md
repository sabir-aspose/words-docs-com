---
title: 複数ページの文書をPython内の画像に変換する
second_title: Aspose.WordsのためのPython
articleTitle: 複数ページのドキュメントを画像に変換する
linktitle: 複数ページのドキュメントを画像に変換する
type: docs
description: "複数ページのドキュメントをラスターイメージにエクスポートする(JPG, PNG, GIF, BMP, TIFF, WebP) Pythonを使用します。"
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ja/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.WordsforPython via .NETユーザーは、複数ページのドキュメントをラスターイメージにエクスポートできます。 これは、編集不可能な使用のためにドキュメントのプレビュー、アーカイブ、または視覚的な表現を生成するのに役立ちます。

## 複数ページのエクスポートをサポートする形式は何ですか？

Aspose.Wordsは、次のラスターイメージ形式へのマルチページエクスポートをサポートします:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## 複数ページのドキュメントを画像にエクスポートする方法

複数ページのドキュメントを画像にエクスポートする機能は[MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/)クラスを使用して実装されています–画像に保存するときにページをどのように整理す:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/)–指定されたページの最初のページのみを保存します
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float)-列の数を指定しながら、ページを左から右、上から下にグリッドに配置します
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float)–単一の出力でページを水平に並べ、左から右に配置します
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float)-単一の出力でページを上下に垂直に配置します
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/)-各ページをマルチフレームTIFF画像内の個別のフレームとして配置します。TIFF画像形式にのみ適用されます

次のコード例は、複数ページDOCXドキュメントを水平レイアウトでJPEGイメージとして保存する方法を示しています:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

出力ファイルのページの外観をカスタマイズすることもできます–[back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/)、[border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/)、および[border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/)を指定します。

次のコード例は、グリッドレイアウトを使用して複数ページDOCXドキュメントをPNGイメージとして保存する方法を示しています:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.PNG)
# Set up a grid layout with:
# - 3 columns per row.
# - 10pts spacing between pages (horizontal and vertical).
options.page_layout = aw.saving.MultiPageLayout.grid(3, 10, 10)

# Customize the background and border.
options.page_layout.back_color = aspose.pydrawing.Color.light_gray
options.page_layout.border_color = aspose.pydrawing.Color.blue
options.page_layout.border_width = 2

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}