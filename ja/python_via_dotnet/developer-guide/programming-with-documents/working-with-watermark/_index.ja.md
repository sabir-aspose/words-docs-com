---
title: Pythonでの透かしの操作
second_title: Aspose.WordsのためのPython via .NET
articleTitle: 透かしの操作
linktitle: 透かしの操作
description: "Pythonを使用して文書内の透かしを作成および管理します。"
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ja/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

このトピックでは、Aspose.Wordsを使用してwatermarkをプログラムで操作する方法について説明します。 透かしは、ドキュメント内のテキストの後ろに表示される背景画像です。 透かしには、[Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/)クラスで表されるテキストまたは画像を含めることができます。

{{% alert color="primary" %}}

**オンラインで試す**

あなたは私たちのこの機能を試すことができます [無料のオンライン文書透かし](https://products.aspose.app/words/watermark).

{{% /alert %}}

## 文書に透かしを追加する方法

Microsoft Wordでは、[透かしの挿入]コマンドを使用して、文書に透かしを簡単に挿入できます。 Aspose.Wordsは、ドキュメント内の透かしを追加または削除するための[Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/)クラスを提供します。 Aspose.Wordsは、動作する透かしの三つのタイプ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text)、[IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image)、[NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none))を定義する[WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/)列挙体を提供します。

### テキスト透かしを追加

次のコード例は、[set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/)メソッドを使用して[TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/)を定義して、ドキュメントにテキスト透かしを挿入する方法を示しています:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### 画像の透かしを追加

次のコード例は、[set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/)メソッドを使用して[ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/)を定義して、ドキュメントに画像透かしを挿入する方法を示しています:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

画像の透かしは、画像、文字列、またはストリームとして挿入できます。

透かしは、shapeクラスを使用して挿入することもできます。 ヘッダーやフッターに任意の形状や画像を挿入し、したがって、任意の想像できるタイプの透かしを作成することは非常に簡単です。

次のコード例では、Wordドキュメントに透かしを挿入します:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

この例のテンプレートファイルは、次の場所からダウンロードできます [ここに](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## 文書から透かしを削除する

[Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/)クラスは、ドキュメントから透かしを削除するremoveメソッドを提供します。

次のコード例は、ドキュメントから透かしを削除する方法を示しています:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

透かしが[Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/)クラスオブジェクトを使用して追加されている場合、文書から透かしを削除するには、挿入中に透かし形状の名前のみを設定し、割り当て

次のコード例は、透かし図形の名前を設定してドキュメントから削除する方法を示しています:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## テーブルセルに透かしを追加する

テーブルのセルに透かし/画像を挿入してテーブルの外に表示する必要がある場合は、[is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/)プロパティを使用できます。 このプロパティは、図形がテーブルの内側に表示されるか、テーブルの外側に表示されるかを示すフラグを取得または設定します。 このプロパティは、[optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/)メソッドを使用してMicrosoft Word2010のドキュメントを最適化する場合にのみ機能することに注意してください。

次のコード例は、このプロパティを使用する方法を示しています:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
