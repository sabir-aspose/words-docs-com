---
title: Arbeiten mit Wasserzeichen in C#
second_title: Aspose.Words für .NET
articleTitle: Arbeiten mit Wasserzeichen
linktitle: Arbeiten mit Wasserzeichen
description: "Manipulation des Dokumentwasserzeichens mit C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /de/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

In diesem Thema wird erläutert, wie Sie mit Aspose.Words programmgesteuert mit Wasserzeichen arbeiten. Ein Wasserzeichen ist ein Hintergrundbild, das hinter dem Text in einem Dokument angezeigt wird. Ein Wasserzeichen kann einen Text oder ein Bild enthalten, das durch die Klasse [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) dargestellt wird.

{{% alert color="primary" %}}

**Online ausprobieren**

Sie können diese Funktionalität mit unserem ausprobieren [Kostenloses Online Wasserzeichen für Dokumente](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Hinzufügen eines Wasserzeichens zu einem Dokument

In Microsoft Word kann ein Wasserzeichen einfach mit dem Befehl Wasserzeichen einfügen in ein Dokument eingefügt werden. Aspose.Words stellt die Klasse [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) zum Hinzufügen oder Entfernen von Wasserzeichen in Dokumenten bereit. Aspose.Words stellt die [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)-Aufzählung bereit, die drei mögliche Arten von Wasserzeichen (Text, Bild und Keine) definiert, mit denen gearbeitet werden soll.

### Text-Wasserzeichen hinzufügen

Das folgende Codebeispiel zeigt, wie Sie ein Textwasserzeichen in ein Dokument einfügen, indem Sie [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) mit der Methode [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext) definieren:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Bild-Wasserzeichen hinzufügen

Das folgende Codebeispiel zeigt, wie Sie ein Bildwasserzeichen in ein Dokument einfügen, indem Sie [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) mit der Methode [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage) definieren:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Bildwasserzeichen können als Bild, Zeichenfolge oder Stream eingefügt werden.

Das Wasserzeichen kann auch mit der Formklasse eingefügt werden. Es ist sehr einfach, eine beliebige Form oder ein beliebiges Bild in eine Kopf- oder Fußzeile einzufügen und so ein Wasserzeichen jeder erdenklichen Art zu erstellen.

Das folgende Codebeispiel fügt ein Wasserzeichen in ein Word -Dokument ein:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Sie können die Beispieldatei dieses Beispiels herunterladen von [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Wasserzeichen aus einem Dokument entfernen

Die Klasse [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) stellt die Methode remove bereit, um das Wasserzeichen aus einem Dokument zu entfernen.

Das folgende Codebeispiel zeigt, wie Sie ein Wasserzeichen aus Dokumenten entfernen:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Wenn die Wasserzeichen mit dem Klassenobjekt [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/) hinzugefügt werden, müssen Sie zum Entfernen des Wasserzeichens aus einem Dokument beim Einfügen nur den Namen der Wasserzeichenform festlegen und dann die Wasserzeichenform mit einem zugewiesenen Namen entfernen.

Das folgende Codebeispiel zeigt Ihnen, wie Sie den Namen der Wasserzeichenform festlegen und aus dem Dokument entfernen:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Fügen Sie ein Wasserzeichen in eine Tabellenzelle ein

Manchmal müssen Sie ein Wasserzeichen / Bild in die Zelle einer Tabelle einfügen und es außerhalb der Tabelle anzeigen. Sie können die Eigenschaft [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/) verwenden. Diese Eigenschaft ruft ein Flag ab oder legt es fest, das angibt, ob das Shape innerhalb oder außerhalb einer Tabelle angezeigt wird. Beachten Sie, dass diese Eigenschaft nur funktioniert, wenn Sie das Dokument für Microsoft Word 2010 mit der Methode [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/) optimieren.

Das folgende Codebeispiel zeigt, wie diese Eigenschaft verwendet wird:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
