---
title: Convertiți un Document cu mai multe pagini într-o imagine în C#
second_title: Aspose.Words pentru .NET
articleTitle: Conversia unui Document cu mai multe pagini într-o imagine
linktitle: Conversia unui Document cu mai multe pagini într-o imagine
type: docs
description: "Exportați documente cu mai multe pagini în imagini raster(JPG, PNG, GIF, BMP, TIFF, WebP) Folosind C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ro/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words pentru .NET permite utilizatorilor să exporte documente cu mai multe pagini în imagini raster. Acest lucru poate fi util pentru generarea de previzualizări, arhive sau reprezentări vizuale ale documentelor pentru utilizare needitabilă.

## Ce formate acceptă exportul pe mai multe pagini?

Aspose.Words suportă exportul pe mai multe pagini în următoarele formate de imagine raster:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Cum să exportați un Document cu mai multe pagini într-o imagine

Caracteristica exportului unui document cu mai multe pagini într-o imagine este implementată folosind clasa [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) – puteți specifica modul în care trebuie organizate paginile atunci când salvați într-o imagine:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - salvați doar prima dintre paginile specificate
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - aranjați paginile într - o grilă, de la stânga la dreapta și de sus în jos, specificând în același timp numărul de coloane
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - aranjați paginile orizontal unul lângă altul, de la stânga la dreapta, într-o singură ieșire
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - aranjați paginile vertical una sub cealaltă într-o singură ieșire
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - aranjați fiecare pagină ca un cadru separat într-o imagine cu mai multe cadre TIFF, se aplică numai formatelor de imagine TIFF 

Următorul exemplu de cod arată cum să salvați un document DOCX cu mai multe pagini ca imagine JPEG cu aspect orizontal:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

De asemenea, puteți personaliza aspectul paginii fișierului de ieșire – specificați [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) și [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

Următorul exemplu de cod arată cum să salvați un document DOCX cu mai multe pagini ca PNG imagine cu aspect grilă:

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