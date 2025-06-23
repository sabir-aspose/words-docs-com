---
title: Skakel'n Multi-bladsy Dokument na'n Beeld in C#
second_title: Aspose.Words vir .NET
articleTitle: Skakel'n Multi-bladsy Dokument na'n Beeld
linktitle: Skakel'n Multi-bladsy Dokument na'n Beeld
type: docs
description: "Voer multi-bladsy dokumente na raster beelde (JPG, PNG, GIF, BMP, TIFF, WebP) gebruik C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /af/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words vir .NET laat gebruikers toe om meerbladsy-dokumente na rasterbeelde uit te voer. Dit kan nuttig wees vir die opwekking van voorskoue, argiewe of visuele voorstellings van dokumente vir nie-bewerkbare gebruik.

## Watter Formate Ondersteun Multi-bladsy Uitvoer?

Aspose.Words ondersteun multi-bladsy uitvoer na die volgende raster beeld formate:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Hoe Om'n Multi-bladsy Dokument Na'n Beeld Uit Te Voer

Die kenmerk van die uitvoer van'n multi-bladsy dokument na'n beeld word geïmplementeer met behulp van die [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) klas-jy kan spesifiseer hoe die bladsye georganiseer moet word wanneer jy na'n beeld stoor:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - stoor slegs die eerste van die gespesifiseerde bladsye
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - rangskik die bladsye in'n rooster, van links na regs en van bo na onder, terwyl die aantal kolomme gespesifiseer word
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - rangskik die bladsye horisontaal langs mekaar, van links na regs, in'n enkele uitset
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - rangskik die bladsye vertikaal een onder die ander in'n enkele uitset
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - rangskik elke bladsy as'n aparte raam in'n multi-raam TIFF beeld, is slegs van toepassing op TIFF beeldformate

Die volgende kode voorbeeld toon hoe om'n multi-bladsy DOCX dokument te red as JPEG beeld met Horisontale uitleg:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Jy kan ook pasmaak die uitset lêer bladsy voorkoms-spesifiseer [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/), en [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

Die volgende kode voorbeeld toon hoe om'n multi-bladsy DOCX dokument as PNG beeld met Rooster uitleg te red:

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