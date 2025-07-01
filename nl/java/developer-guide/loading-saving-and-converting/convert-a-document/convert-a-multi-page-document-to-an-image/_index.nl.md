---
title: Een Document met meerdere pagina ' s converteren naar een afbeelding in Java
second_title: Aspose.Words voor Java
articleTitle: Een Document met meerdere pagina ' s converteren naar een afbeelding
linktitle: Een Document met meerdere pagina ' s converteren naar een afbeelding
type: docs
description: "Documenten met meerdere pagina ' s exporteren naar rasterafbeeldingen (JPG, PNG, GIF, BMP, TIFF, WebP) gebruik Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nl/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Met Aspose.Words voor Java kunnen gebruikers documenten van meerdere pagina ' s exporteren naar rasterafbeeldingen. Dit kan handig zijn voor het genereren van voorvertoningen, Archieven of visuele weergaven van documenten voor niet-bewerkbaar gebruik.

## Welke formaten ondersteunen multi-page Export?

Aspose.Words ondersteunt het exporteren van meerdere pagina ' s naar de volgende rasterafbeeldingen:

* Jpeg
* Gif
* Png
* Bmp
* TIFF
* WebP

## Een Document met meerdere pagina ' s exporteren naar een afbeelding

De functie van het exporteren van een document met meerdere pagina 's naar een afbeelding wordt geïmplementeerd met behulp van de klasse [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) - U kunt opgeven hoe de pagina' s moeten worden georganiseerd bij het opslaan naar een afbeelding:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - sla alleen de eerste van de opgegeven pagina ' s op
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - rangschik de pagina ' s in een raster, van links naar rechts en van boven naar beneden, met vermelding van het aantal kolommen
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - Schik de pagina ' s horizontaal naast elkaar, van links naar rechts, in één uitvoer
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - Schik de pagina ' s verticaal onder elkaar in één uitvoer
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - schik elke pagina als een apart frame in een multi-frame TIFF afbeelding, geldt alleen voor TIFF afbeeldingsindelingen

Het volgende codevoorbeeld laat zien hoe u een DOCX-document met meerdere pagina ' s kunt opslaan als JPEG - afbeelding met horizontale lay-out:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

U kunt ook het uiterlijk van de uitvoerbestandspagina aanpassen-Geef [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) en [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth) op.

Het volgende codevoorbeeld laat zien hoe u een DOCX-document met meerdere pagina ' s kunt opslaan als PNG - afbeelding met rasterindeling:

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