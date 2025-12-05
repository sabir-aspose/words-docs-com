---
title: Konwertuj wielostronicowy dokument na obraz w C#
second_title: Aspose.Words dla .NET
articleTitle: Konwertuj wielostronicowy dokument na obraz
linktitle: Konwertuj wielostronicowy dokument na obraz
type: docs
description: "Eksportuj wielostronicowe dokumenty do obrazów rastrowych(JPG, PNG, GIF, BMP, TIFF, WebP) używając C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pl/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words for .NET umożliwia użytkownikom eksportowanie wielostronicowych dokumentów do obrazów rastrowych. Może to być przydatne do generowania podglądów, archiwów lub wizualnych reprezentacji dokumentów do użytku nieedytowalnego.

## Jakie formaty obsługują eksport wielostronicowy?

Aspose.Words obsługuje wielostronicowy eksport do następujących formatów obrazów rastrowych:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Jak wyeksportować wielostronicowy dokument do obrazu

Funkcja eksportowania wielostronicowego dokumentu do obrazu jest zaimplementowana przy użyciu klasy [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) – możesz określić sposób organizacji stron podczas zapisywania na obrazie:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - Zapisz tylko pierwszą z podanych stron
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - ułóż strony w siatce, od lewej do prawej i od góry do dołu, określając liczbę kolumn
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - ułóż strony poziomo obok siebie, od lewej do prawej, w jednym wyjściu
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - ułóż strony pionowo jedna pod drugą w jednym wyjściu
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - Rozmieść każdą stronę jako osobną ramkę w obrazie z wieloma klatkami TIFF, dotyczy tylko formatów obrazów TIFF 

Poniższy przykład kodu pokazuje, jak zapisać wielostronicowy dokument DOCX jako obraz JPEG z układem poziomym:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Możesz także dostosować wygląd strony pliku wyjściowego-określ [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) i [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

Poniższy przykład kodu pokazuje, jak zapisać wielostronicowy dokument DOCX jako obraz PNG z układem siatki:

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