---
title: Skakel'n Multi-bladsy Dokument na'n Beeld in Java
second_title: Aspose.Words vir Java
articleTitle: Skakel'n Multi-bladsy Dokument na'n Beeld
linktitle: Skakel'n Multi-bladsy Dokument na'n Beeld
type: docs
description: "Voer multi-bladsy dokumente na raster beelde (JPG, PNG, GIF, BMP, TIFF, WebP) gebruik Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /af/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words vir Java laat gebruikers toe om meerbladsy-dokumente na rasterbeelde uit te voer. Dit kan nuttig wees vir die opwekking van voorskoue, argiewe of visuele voorstellings van dokumente vir nie-bewerkbare gebruik.

## Watter Formate Ondersteun Multi-bladsy Uitvoer?

Aspose.Words ondersteun multi-bladsy uitvoer na die volgende raster beeld formate:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Hoe Om'n Multi-bladsy Dokument Na'n Beeld Uit Te Voer

Die kenmerk van die uitvoer van'n multi-bladsy dokument na'n beeld word geïmplementeer met behulp van die [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) klas-jy kan spesifiseer hoe die bladsye georganiseer moet word wanneer jy na'n beeld stoor:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - stoor slegs die eerste van die gespesifiseerde bladsye
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - rangskik die bladsye in'n rooster, van links na regs en van bo na onder, terwyl die aantal kolomme gespesifiseer word
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - rangskik die bladsye horisontaal langs mekaar, van links na regs, in'n enkele uitset
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - rangskik die bladsye vertikaal een onder die ander in'n enkele uitset
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - rangskik elke bladsy as'n aparte raam in'n multi-raam TIFF beeld, is slegs van toepassing op TIFF beeldformate

Die volgende kode voorbeeld toon hoe om'n multi-bladsy DOCX dokument te red as JPEG beeld met Horisontale uitleg:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Jy kan ook pasmaak die uitset lêer bladsy voorkoms-spesifiseer [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor), en [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

Die volgende kode voorbeeld toon hoe om'n multi-bladsy DOCX dokument as PNG beeld met Rooster uitleg te red:

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