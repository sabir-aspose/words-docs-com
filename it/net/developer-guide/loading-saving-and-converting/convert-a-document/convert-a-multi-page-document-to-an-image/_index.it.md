---
title: Convertire un documento multipagina in un'immagine in C#
second_title: Aspose.Words per .NET
articleTitle: Convertire un documento multipagina in un'immagine
linktitle: Convertire un documento multipagina in un'immagine
type: docs
description: "Esportare documenti multipagina in immagini raster(JPG, PNG, GIF, BMP, TIFF, WebP) usando C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /it/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words per .NET consente agli utenti di esportare documenti multipagina in immagini raster. Questo può essere utile per generare anteprime, archivi o rappresentazioni visive di documenti per uso non modificabile.

## Quali formati supportano l'esportazione multipagina?

Aspose.Words supporta l'esportazione multipagina nei seguenti formati di immagine raster:

* JPEG
* GIF
* Png
* BMP
* TIFF
* WebP

## Come esportare un documento multipagina in un'immagine

La funzione di esportazione di un documento multipagina in un'immagine viene implementata utilizzando la classe [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) : è possibile specificare come organizzare le pagine quando si salva in un'immagine:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - salva solo la prima delle pagine specificate
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) – disporre le pagine in una griglia, da sinistra a destra e dall'alto verso il basso, specificando il numero di colonne
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) – disporre le pagine orizzontalmente affiancate, da sinistra a destra, in un unico output
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) – disporre le pagine verticalmente una sotto l'altra in un unico output
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) – disponi ogni pagina come un fotogramma separato in un'immagine multi-frame TIFF, si applica solo ai formati immagine TIFF

Il seguente esempio di codice mostra come salvare un documento DOCX multipagina come immagine JPEG con layout orizzontale:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

È inoltre possibile personalizzare l'aspetto della pagina del file di output, specificando [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) e [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

Il seguente esempio di codice mostra come salvare un documento DOCX multipagina come immagine PNG con layout a griglia:

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