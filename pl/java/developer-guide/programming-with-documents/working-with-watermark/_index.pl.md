---
title: Praca ze znakiem wodnym w Java
second_title: Aspose.Words dla Java
articleTitle: Praca ze znakiem wodnym
linktitle: Praca ze znakiem wodnym
type: docs
description: "Manipulacja znakiem wodnym dokumentu przy użyciu Java."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pl/java/working-with-watermark/
timestamp: 2025-04-22-08-07-04
---

W tym temacie omówiono programową pracę ze znakiem wodnym przy użyciu Aspose.Words. Znak wodny to obraz tła wyświetlany za tekstem w dokumencie. Znak wodny może zawierać tekst lub obraz reprezentowany przez klasę [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/).

{{% alert color="primary" %}}

**Spróbuj online**

Możesz wypróbować tę funkcjonalność z naszym [Darmowy znak wodny dokumentu online](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Dodawanie znaku wodnego do dokumentu

W Microsoft Word Znak wodny można łatwo wstawić do dokumentu za pomocą polecenia Wstaw Znak wodny. Aspose.Words zapewnia klasę [watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) do dodawania lub usuwania znaku wodnego w dokumentach. Aspose.Words zapewnia wyliczenie [WatermarkType ](https://reference.aspose.com/words/java/com.aspose.words/watermarktype/)definiujące trzy możliwe typy znaków wodnych (tekst, obraz i brak) do pracy.

### Dodaj Tekstowy Znak Wodny

Poniższy przykład kodu pokazuje, jak wstawić tekstowy znak wodny do dokumentu, definiując [TextWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/textwatermarkoptions/) przy użyciu metody [SetText](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setText-java.lang.String):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddTextWatermarkWithSpecificOptions.java" >}}

### Dodaj Znak Wodny Obrazu

Poniższy przykład kodu pokazuje, jak wstawić znak wodny obrazu do dokumentu, definiując [ImageWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/imagewatermarkoptions/) przy użyciu metody [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.awt.image.BufferedImage):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddImageWatermarkWithSpecificOptions.java" >}}

Znak wodny obrazu można wstawić jako obraz, ciąg lub strumień.

Znak wodny można również wstawić za pomocą klasy kształtu. Bardzo łatwo jest wstawić dowolny kształt lub obraz do nagłówka lub stopki, a tym samym utworzyć znak wodny dowolnego możliwego typu.

Poniższy przykład kodu wstawia znak wodny do dokumentu Word:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-AddWatermarkToADocument-AddWatermarkToADocument.java" >}}

{{% alert color="primary" %}}

Możesz pobrać przykładowy plik tego przykładu z [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Document.doc).

{{% /alert %}}


## Usuń znak wodny z dokumentu

Klasa [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) zapewnia `Remove` metodę usuwania znaku wodnego z dokumentu.

Poniższe przykłady kodu pokazują, jak usunąć znak wodny z dokumentów:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-RemoveWatermarkFromDocument.java" >}}

Aby usunąć znak wodny z dokumentu, musisz ustawić tylko nazwę kształtu znaku wodnego podczas wstawiania, a następnie usunąć kształt znaku wodnego za pomocą przypisanej nazwy.

Poniższy przykład kodu pokazuje, jak ustawić nazwę kształtu znaku wodnego i usunąć go z dokumentu:

{{< highlight csharp >}}

// Set name to be able to remove it afterwards
watermark.Name("WaterMark");
{{< /highlight >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-RemoveWatermark-RemoveWatermark.java" >}}

## Dodaj znak wodny do komórki tabeli

Czasami musisz wstawić znak wodny / obraz do komórki tabeli i wyświetlić go poza tabelą, możesz użyć właściwości [IsLayoutInCell](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#isLayoutInCell-boolean). Ta Właściwość pobiera lub ustawia flagę wskazującą, czy kształt jest wyświetlany wewnątrz tabeli, czy poza nią. Zauważ, że ta właściwość działa tylko wtedy, gdy zoptymalizujesz dokument dla Microsoft Word 2010 przy użyciu metody [OptimizeFor](https://reference.aspose.com/words/java/com.aspose.words/compatibilityoptions/#optimizeFor-int).

Poniższy przykład kodu pokazuje, jak korzystać z tej właściwości:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-Shapes-WorkingWithShapes-SetShapeLayoutInCell.java" >}}
