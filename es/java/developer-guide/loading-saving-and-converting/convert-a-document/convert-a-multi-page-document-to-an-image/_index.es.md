---
title: Convierta un documento de varias páginas en una Imagen en Java
second_title: Aspose.Words por Java
articleTitle: Convertir un Documento de Varias páginas en una Imagen
linktitle: Convertir un Documento de Varias páginas en una Imagen
type: docs
description: "Exportar documentos de varias páginas a imágenes rasterizadas(JPG, PNG, GIF, BMP, TIFF, WebP) usando Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /es/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words para Java permite a los usuarios exportar documentos de varias páginas a imágenes rasterizadas. Esto puede ser útil para generar vistas previas, archivos o representaciones visuales de documentos para uso no editable.

## ¿Qué Formatos Admiten La Exportación de Varias páginas?

Aspose.Words admite la exportación de varias páginas a los siguientes formatos de imagen rasterizada:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Cómo Exportar un Documento de varias páginas a una Imagen

La función de exportar un documento de varias páginas a una imagen se implementa utilizando la clase [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/); puede especificar cómo se deben organizar las páginas al guardar en una imagen:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - guardar solo la primera de las páginas especificadas
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float): organice las páginas en una cuadrícula, de izquierda a derecha y de arriba a abajo, al tiempo que especifica el número de columnas
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - organice las páginas horizontalmente una al lado de la otra, de izquierda a derecha, en una sola salida
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - organice las páginas verticalmente una debajo de la otra en una sola salida
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames): organice cada página como un marco separado en una imagen TIFF de varios marcos, se aplica solo a los formatos de imagen TIFF

El siguiente ejemplo de código muestra cómo guardar un documento DOCX de varias páginas como una imagen JPEG con diseño horizontal:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

También puede personalizar la apariencia de la página del archivo de salida: especifique [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) y [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

El siguiente ejemplo de código muestra cómo guardar un documento DOCX de varias páginas como una imagen PNG con diseño de cuadrícula:

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