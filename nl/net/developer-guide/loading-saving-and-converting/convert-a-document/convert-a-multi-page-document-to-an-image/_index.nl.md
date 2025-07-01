---
title: Een Document met meerdere pagina ' s converteren naar een afbeelding in C#
second_title: Aspose.Words voor .NET
articleTitle: Een Document met meerdere pagina ' s converteren naar een afbeelding
linktitle: Een Document met meerdere pagina ' s converteren naar een afbeelding
type: docs
description: "Documenten met meerdere pagina ' s exporteren naar rasterafbeeldingen (JPG, PNG, GIF, BMP, TIFF, WebP) gebruik C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nl/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Met Aspose.Words voor .NET kunnen gebruikers documenten van meerdere pagina ' s exporteren naar rasterafbeeldingen. Dit kan handig zijn voor het genereren van voorvertoningen, Archieven of visuele weergaven van documenten voor niet-bewerkbaar gebruik.

## Welke formaten ondersteunen multi-page Export?

Aspose.Words ondersteunt het exporteren van meerdere pagina ' s naar de volgende rasterafbeeldingen:

* Jpeg
* Gif
* Png
* Bmp
* TIFF
* WebP

## Een Document met meerdere pagina ' s exporteren naar een afbeelding

De functie van het exporteren van een document met meerdere pagina 's naar een afbeelding wordt geïmplementeerd met behulp van de klasse [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) - U kunt opgeven hoe de pagina' s moeten worden georganiseerd bij het opslaan naar een afbeelding:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - sla alleen de eerste van de opgegeven pagina ' s op
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - rangschik de pagina ' s in een raster, van links naar rechts en van boven naar beneden, met vermelding van het aantal kolommen
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - Schik de pagina ' s horizontaal naast elkaar, van links naar rechts, in één uitvoer
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - Schik de pagina ' s verticaal onder elkaar in één uitvoer
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - schik elke pagina als een apart frame in een multi-frame TIFF afbeelding, geldt alleen voor TIFF afbeeldingsindelingen

Het volgende codevoorbeeld laat zien hoe u een DOCX-document met meerdere pagina ' s kunt opslaan als JPEG - afbeelding met horizontale lay-out:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

U kunt ook het uiterlijk van de uitvoerbestandspagina aanpassen-Geef [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) en [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/) op.

Het volgende codevoorbeeld laat zien hoe u een DOCX-document met meerdere pagina ' s kunt opslaan als PNG - afbeelding met rasterindeling:

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