---
title: Convertiți un Document cu mai multe pagini într-o imagine în Python
second_title: Aspose.Words pentru Python
articleTitle: Conversia unui Document cu mai multe pagini într-o imagine
linktitle: Conversia unui Document cu mai multe pagini într-o imagine
type: docs
description: "Exportați documente cu mai multe pagini în imagini raster(JPG, PNG, GIF, BMP, TIFF, WebP) folosind Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ro/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words Pentru Python via .NET permite utilizatorilor să exporte documente cu mai multe pagini în imagini raster. Acest lucru poate fi util pentru generarea de previzualizări, arhive sau reprezentări vizuale ale documentelor pentru utilizare needitabilă.

## Ce formate acceptă exportul pe mai multe pagini?

Aspose.Words suportă exportul pe mai multe pagini în următoarele formate de imagine raster:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Cum să exportați un Document cu mai multe pagini într-o imagine

Caracteristica exportului unui document cu mai multe pagini într-o imagine este implementată folosind clasa [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) – puteți specifica modul în care trebuie organizate paginile atunci când salvați într-o imagine:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - salvați doar prima dintre paginile specificate
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - aranjați paginile într - o grilă, de la stânga la dreapta și de sus în jos, specificând în același timp numărul de coloane
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - aranjați paginile orizontal unul lângă altul, de la stânga la dreapta, într-o singură ieșire
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - aranjați paginile vertical una sub cealaltă într-o singură ieșire
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - aranjați fiecare pagină ca un cadru separat într-o imagine cu mai multe cadre TIFF, se aplică numai formatelor de imagine TIFF 

Următorul exemplu de cod arată cum să salvați un document DOCX cu mai multe pagini ca imagine JPEG cu aspect orizontal:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

De asemenea, puteți personaliza aspectul paginii fișierului de ieșire – specificați [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) și [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

Următorul exemplu de cod arată cum să salvați un document DOCX cu mai multe pagini ca PNG imagine cu aspect grilă:

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