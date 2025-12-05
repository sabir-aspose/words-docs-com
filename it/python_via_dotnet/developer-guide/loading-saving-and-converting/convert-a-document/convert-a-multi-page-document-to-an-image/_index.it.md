---
title: Convertire un documento multipagina in un'immagine in Python
second_title: Aspose.Words per Python
articleTitle: Convertire un documento multipagina in un'immagine
linktitle: Convertire un documento multipagina in un'immagine
type: docs
description: "Esportare documenti multipagina in immagini raster(JPG, PNG, GIF, BMP, TIFF, WebP) usando Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /it/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words per Python via .NET consente agli utenti di esportare documenti multipagina in immagini raster. Questo può essere utile per generare anteprime, archivi o rappresentazioni visive di documenti per uso non modificabile.

## Quali formati supportano l'esportazione multipagina?

Aspose.Words supporta l'esportazione multipagina nei seguenti formati di immagine raster:

* JPEG
* GIF
* Png
* BMP
* TIFF
* WebP

## Come esportare un documento multipagina in un'immagine

La funzione di esportazione di un documento multipagina in un'immagine viene implementata utilizzando la classe [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) : è possibile specificare come organizzare le pagine quando si salva in un'immagine:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - salva solo la prima delle pagine specificate
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) – disporre le pagine in una griglia, da sinistra a destra e dall'alto verso il basso, specificando il numero di colonne
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) – disporre le pagine orizzontalmente affiancate, da sinistra a destra, in un unico output
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) – disporre le pagine verticalmente una sotto l'altra in un unico output
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) – disponi ogni pagina come un fotogramma separato in un'immagine multi-frame TIFF, si applica solo ai formati immagine TIFF

Il seguente esempio di codice mostra come salvare un documento DOCX multipagina come immagine JPEG con layout orizzontale:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

È inoltre possibile personalizzare l'aspetto della pagina del file di output, specificando [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) e [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

Il seguente esempio di codice mostra come salvare un documento DOCX multipagina come immagine PNG con layout a griglia:

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