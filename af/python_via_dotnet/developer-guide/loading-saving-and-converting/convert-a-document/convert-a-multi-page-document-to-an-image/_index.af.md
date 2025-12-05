---
title: Skakel'n Multi-bladsy Dokument na'n Beeld in Python
second_title: Aspose.Words vir Python
articleTitle: Skakel'n Multi-bladsy Dokument na'n Beeld
linktitle: Skakel'n Multi-bladsy Dokument na'n Beeld
type: docs
description: "Voer multi-bladsy dokumente na raster beelde (JPG, PNG, GIF, BMP, TIFF, WebP) gebruik Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /af/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words vir Python via .NET laat gebruikers toe om meerbladsy-dokumente na rasterbeelde uit te voer. Dit kan nuttig wees vir die opwekking van voorskoue, argiewe of visuele voorstellings van dokumente vir nie-bewerkbare gebruik.

## Watter Formate Ondersteun Multi-bladsy Uitvoer?

Aspose.Words ondersteun multi-bladsy uitvoer na die volgende raster beeld formate:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Hoe Om'n Multi-bladsy Dokument Na'n Beeld Uit Te Voer

Die kenmerk van die uitvoer van'n multi-bladsy dokument na'n beeld word geïmplementeer met behulp van die [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) klas-jy kan spesifiseer hoe die bladsye georganiseer moet word wanneer jy na'n beeld stoor:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - stoor slegs die eerste van die gespesifiseerde bladsye
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - rangskik die bladsye in'n rooster, van links na regs en van bo na onder, terwyl die aantal kolomme gespesifiseer word
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - rangskik die bladsye horisontaal langs mekaar, van links na regs, in'n enkele uitset
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - rangskik die bladsye vertikaal een onder die ander in'n enkele uitset
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - rangskik elke bladsy as'n aparte raam in'n multi-raam TIFF beeld, is slegs van toepassing op TIFF beeldformate

Die volgende kode voorbeeld toon hoe om'n multi-bladsy DOCX dokument te red as JPEG beeld met Horisontale uitleg:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Jy kan ook pasmaak die uitset lêer bladsy voorkoms-spesifiseer [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/), en [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

Die volgende kode voorbeeld toon hoe om'n multi-bladsy DOCX dokument as PNG beeld met Rooster uitleg te red:

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