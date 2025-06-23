---
title: Convertiți un Document cu mai multe pagini într-o imagine în Java
second_title: Aspose.Words pentru Java
articleTitle: Conversia unui Document cu mai multe pagini într-o imagine
linktitle: Conversia unui Document cu mai multe pagini într-o imagine
type: docs
description: "Exportați documente cu mai multe pagini în imagini raster(JPG, PNG, GIF, BMP, TIFF, WebP) Folosind Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ro/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words pentru Java permite utilizatorilor să exporte documente cu mai multe pagini în imagini raster. Acest lucru poate fi util pentru generarea de previzualizări, arhive sau reprezentări vizuale ale documentelor pentru utilizare needitabilă.

## Ce formate acceptă exportul pe mai multe pagini?

Aspose.Words suportă exportul pe mai multe pagini în următoarele formate de imagine raster:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Cum să exportați un Document cu mai multe pagini într-o imagine

Caracteristica exportului unui document cu mai multe pagini într-o imagine este implementată folosind clasa [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) – puteți specifica modul în care trebuie organizate paginile atunci când salvați într-o imagine:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - salvați doar prima dintre paginile specificate
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - aranjați paginile într - o grilă, de la stânga la dreapta și de sus în jos, specificând în același timp numărul de coloane
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - aranjați paginile orizontal unul lângă altul, de la stânga la dreapta, într-o singură ieșire
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - aranjați paginile vertical una sub cealaltă într-o singură ieșire
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - aranjați fiecare pagină ca un cadru separat într-o imagine cu mai multe cadre TIFF, se aplică numai formatelor de imagine TIFF 

Următorul exemplu de cod arată cum să salvați un document DOCX cu mai multe pagini ca imagine JPEG cu aspect orizontal:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

De asemenea, puteți personaliza aspectul paginii fișierului de ieșire – specificați [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) și [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

Următorul exemplu de cod arată cum să salvați un document DOCX cu mai multe pagini ca PNG imagine cu aspect grilă:

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