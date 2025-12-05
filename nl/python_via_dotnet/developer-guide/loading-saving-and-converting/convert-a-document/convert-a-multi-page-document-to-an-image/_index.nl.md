---
title: Een Document met meerdere pagina ' s converteren naar een afbeelding in Python
second_title: Aspose.Words voor Python
articleTitle: Een Document met meerdere pagina ' s converteren naar een afbeelding
linktitle: Een Document met meerdere pagina ' s converteren naar een afbeelding
type: docs
description: "Documenten met meerdere pagina ' s exporteren naar rasterafbeeldingen (JPG, PNG, GIF, BMP, TIFF, WebP) Python gebruiken."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nl/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Met Aspose.Words Voor Python via .NET kunnen gebruikers documenten van meerdere pagina ' s exporteren naar rasterafbeeldingen. Dit kan handig zijn voor het genereren van voorvertoningen, Archieven of visuele weergaven van documenten voor niet-bewerkbaar gebruik.

## Welke formaten ondersteunen multi-page Export?

Aspose.Words ondersteunt het exporteren van meerdere pagina ' s naar de volgende rasterafbeeldingen:

* Jpeg
* Gif
* Png
* Bmp
* TIFF
* WebP

## Een Document met meerdere pagina ' s exporteren naar een afbeelding

De functie van het exporteren van een document met meerdere pagina 's naar een afbeelding wordt geïmplementeerd met behulp van de klasse [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) - U kunt opgeven hoe de pagina' s moeten worden georganiseerd bij het opslaan naar een afbeelding:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - sla alleen de eerste van de opgegeven pagina ' s op
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - rangschik de pagina ' s in een raster, van links naar rechts en van boven naar beneden, met vermelding van het aantal kolommen
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - Schik de pagina ' s horizontaal naast elkaar, van links naar rechts, in één uitvoer
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - Schik de pagina ' s verticaal onder elkaar in één uitvoer
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - schik elke pagina als een apart frame in een multi-frame TIFF afbeelding, geldt alleen voor TIFF afbeeldingsindelingen

Het volgende codevoorbeeld laat zien hoe u een DOCX-document met meerdere pagina ' s kunt opslaan als JPEG - afbeelding met horizontale lay-out:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

U kunt ook het uiterlijk van de uitvoerbestandspagina aanpassen-Geef [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) en [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/) op.

Het volgende codevoorbeeld laat zien hoe u een DOCX-document met meerdere pagina ' s kunt opslaan als PNG - afbeelding met rasterindeling:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.PNG)
# Set up a grid layout with:
# - 3 columns per row.
# - 10pts spacing between pages (horizontal and vertical).
options.page_layout = aw.saving.MultiPageLayout.grid(3, 10, 10)

# Customize the background and border.
options.page_layout.back_color = aspose.pydrawing.Color.light_gray
options.page_layout.border_color = aspose.pydrawing.Color.blue
options.page_layout.border_width = 2

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}