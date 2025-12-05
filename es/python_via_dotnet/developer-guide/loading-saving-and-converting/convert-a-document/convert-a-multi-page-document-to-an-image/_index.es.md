---
title: Convierta un documento de varias páginas en una Imagen en Python
second_title: Aspose.Words por Python
articleTitle: Convertir un Documento de Varias páginas en una Imagen
linktitle: Convertir un Documento de Varias páginas en una Imagen
type: docs
description: "Exportar documentos de varias páginas a imágenes rasterizadas(JPG, PNG, GIF, BMP, TIFF, WebP) usando Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /es/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words para Python via .NET permite a los usuarios exportar documentos de varias páginas a imágenes rasterizadas. Esto puede ser útil para generar vistas previas, archivos o representaciones visuales de documentos para uso no editable.

## ¿Qué Formatos Admiten La Exportación de Varias páginas?

Aspose.Words admite la exportación de varias páginas a los siguientes formatos de imagen rasterizada:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Cómo Exportar un Documento de varias páginas a una Imagen

La función de exportar un documento de varias páginas a una imagen se implementa utilizando la clase [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/); puede especificar cómo se deben organizar las páginas al guardar en una imagen:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - guardar solo la primera de las páginas especificadas
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float): organice las páginas en una cuadrícula, de izquierda a derecha y de arriba a abajo, al tiempo que especifica el número de columnas
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - organice las páginas horizontalmente una al lado de la otra, de izquierda a derecha, en una sola salida
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - organice las páginas verticalmente una debajo de la otra en una sola salida
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/): organice cada página como un marco separado en una imagen TIFF de varios marcos, se aplica solo a los formatos de imagen TIFF

El siguiente ejemplo de código muestra cómo guardar un documento DOCX de varias páginas como una imagen JPEG con diseño horizontal:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

También puede personalizar la apariencia de la página del archivo de salida: especifique [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) y [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

El siguiente ejemplo de código muestra cómo guardar un documento DOCX de varias páginas como una imagen PNG con diseño de cuadrícula:

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