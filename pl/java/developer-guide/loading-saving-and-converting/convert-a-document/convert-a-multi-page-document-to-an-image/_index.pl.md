---
title: Konwertuj wielostronicowy dokument na obraz w Java
second_title: Aspose.Words dla Java
articleTitle: Konwertuj wielostronicowy dokument na obraz
linktitle: Konwertuj wielostronicowy dokument na obraz
type: docs
description: "Eksportuj wielostronicowe dokumenty do obrazów rastrowych(JPG, PNG, GIF, BMP, TIFF, WebP) używając Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pl/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words for Java umożliwia użytkownikom eksportowanie wielostronicowych dokumentów do obrazów rastrowych. Może to być przydatne do generowania podglądów, archiwów lub wizualnych reprezentacji dokumentów do użytku nieedytowalnego.

## Jakie formaty obsługują eksport wielostronicowy?

Aspose.Words obsługuje wielostronicowy eksport do następujących formatów obrazów rastrowych:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Jak wyeksportować wielostronicowy dokument do obrazu

Funkcja eksportowania wielostronicowego dokumentu do obrazu jest zaimplementowana przy użyciu klasy [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) – możesz określić sposób organizacji stron podczas zapisywania na obrazie:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - Zapisz tylko pierwszą z podanych stron
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - ułóż strony w siatce, od lewej do prawej i od góry do dołu, określając liczbę kolumn
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - ułóż strony poziomo obok siebie, od lewej do prawej, w jednym wyjściu
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - ułóż strony pionowo jedna pod drugą w jednym wyjściu
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - Rozmieść każdą stronę jako osobną ramkę w obrazie z wieloma klatkami TIFF, dotyczy tylko formatów obrazów TIFF 

Poniższy przykład kodu pokazuje, jak zapisać wielostronicowy dokument DOCX jako obraz JPEG z układem poziomym:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Możesz także dostosować wygląd strony pliku wyjściowego-określ [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) i [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

Poniższy przykład kodu pokazuje, jak zapisać wielostronicowy dokument DOCX jako obraz PNG z układem siatki:

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