---
title: C#での透かしの操作
second_title: Aspose.Wordsのための.NET
articleTitle: 透かしの操作
linktitle: 透かしの操作
description: "C#を使用した文書の透かし操作。"
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ja/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

このトピックでは、Aspose.Wordsを使用してwatermarkをプログラムで操作する方法について説明します。 透かしは、ドキュメント内のテキストの後ろに表示される背景画像です。 透かしには、[Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/)クラスで表されるテキストまたは画像を含めることができます。

{{% alert color="primary" %}}

**オンラインで試す**

あなたは私たちのこの機能を試すことができます [無料のオンライン文書透かし](https://products.aspose.app/words/watermark).

{{% /alert %}}

## 文書に透かしを追加する

Microsoft Wordでは、[透かしの挿入]コマンドを使用して、文書に透かしを簡単に挿入できます。 Aspose.Wordsは、ドキュメント内の透かしを追加または削除するための[watermark](https://reference.aspose.com/words/net/aspose.words/watermark/)クラスを提供します。 Aspose.Wordsは[WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)列挙体を提供し、使用する透かしの3つのタイプ(テキスト、イメージ、およびなし)を定義します。

### テキスト透かしを追加

次のコード例は、[SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext)メソッドを使用して[TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/)を定義して、ドキュメントにテキスト透かしを挿入する方法を示しています:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### 画像の透かしを追加

次のコード例は、[SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage)メソッドを使用して[ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/)を定義して、ドキュメントに画像透かしを挿入する方法を示しています:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

画像の透かしは、画像、文字列、またはストリームとして挿入できます。

透かしは、shapeクラスを使用して挿入することもできます。 ヘッダーやフッターに任意の形状や画像を挿入し、したがって、任意の想像できるタイプの透かしを作成することは非常に簡単です。

次のコード例では、Wordドキュメントに透かしを挿入します:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

この例のサンプルファイルは、次の場所からダウンロードできます [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## 文書から透かしを削除する

[Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/)クラスは、ドキュメントから透かしを削除するremoveメソッドを提供します。

次のコード例は、ドキュメントから透かしを削除する方法を示しています:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

透かしが[Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/)クラスオブジェクトを使用して追加されている場合、文書から透かしを削除するには、挿入中に透かし形状の名前のみを設定し、割り当て

次のコード例は、透かし図形の名前を設定してドキュメントから削除する方法を示しています:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## 表のセルに透かしを追加する

テーブルのセルに透かし/画像を挿入してテーブルの外に表示する必要がある場合は、[IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/)プロパティを使用できます。 このプロパティは、図形がテーブルの内側に表示されるか、テーブルの外側に表示されるかを示すフラグを取得または設定します。 このプロパティは、[OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/)メソッドを使用してMicrosoft Word2010のドキュメントを最適化する場合にのみ機能することに注意してください。

次のコード例は、このプロパティを使用する方法を示しています:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
