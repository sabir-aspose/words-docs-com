---
title: Praca ze znakiem wodnym w C#
second_title: Aspose.Words dla .NET
articleTitle: Praca ze znakiem wodnym
linktitle: Praca ze znakiem wodnym
description: "Manipulacja znakiem wodnym dokumentu przy użyciu C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pl/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

W tym temacie omówiono programową pracę ze znakiem wodnym przy użyciu Aspose.Words. Znak wodny to obraz tła wyświetlany za tekstem w dokumencie. Znak wodny może zawierać tekst lub obraz reprezentowany przez klasę [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Spróbuj online**

Możesz wypróbować tę funkcjonalność z naszym [Darmowy znak wodny dokumentu online](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Dodawanie znaku wodnego do dokumentu

W Microsoft Word Znak wodny można łatwo wstawić do dokumentu za pomocą polecenia Wstaw Znak wodny. Aspose.Words zapewnia klasę [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) do dodawania lub usuwania znaku wodnego w dokumentach. Aspose.Words zapewnia wyliczenie [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)definiujące trzy możliwe typy znaków wodnych (tekst, obraz i brak) do pracy.

### Dodaj Tekstowy Znak Wodny

Poniższy przykład kodu pokazuje, jak wstawić tekstowy znak wodny do dokumentu, definiując [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) przy użyciu metody [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Dodaj Znak Wodny Obrazu

Poniższy przykład kodu pokazuje, jak wstawić znak wodny obrazu do dokumentu, definiując [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) przy użyciu metody [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Znak wodny obrazu można wstawić jako obraz, ciąg lub strumień.

Znak wodny można również wstawić za pomocą klasy kształtu. Bardzo łatwo jest wstawić dowolny kształt lub obraz do nagłówka lub stopki, a tym samym utworzyć znak wodny dowolnego możliwego typu.

Poniższy przykład kodu wstawia znak wodny do dokumentu Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Możesz pobrać przykładowy plik tego przykładu z [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Usuń znak wodny z dokumentu

Klasa [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) zapewnia metodę usuwania, aby usunąć znak wodny z dokumentu.

Poniższy przykład kodu pokazuje, jak usunąć znak wodny z dokumentów:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Jeśli znaki wodne są dodawane za pomocą obiektu klasy [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/), aby usunąć znak wodny z dokumentu, musisz ustawić tylko nazwę kształtu znaku wodnego podczas wstawiania, a następnie usunąć kształt znaku wodnego za pomocą przypisanej nazwy.

Poniższy przykład kodu pokazuje, jak ustawić nazwę kształtu znaku wodnego i usunąć go z dokumentu:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Dodaj znak wodny do komórki tabeli

Czasami musisz wstawić znak wodny / obraz do komórki tabeli i wyświetlić go poza tabelą, możesz użyć właściwości [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). Ta Właściwość pobiera lub ustawia flagę wskazującą, czy kształt jest wyświetlany wewnątrz tabeli, czy poza nią. Zauważ, że ta właściwość działa tylko wtedy, gdy zoptymalizujesz dokument dla Microsoft Word 2010 przy użyciu metody [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

Poniższy przykład kodu pokazuje, jak korzystać z tej właściwości:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
