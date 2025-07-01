---
title: Convierta un documento de varias páginas en una Imagen en C#
second_title: Aspose.Words por .NET
articleTitle: Convertir un Documento de Varias páginas en una Imagen
linktitle: Convertir un Documento de Varias páginas en una Imagen
type: docs
description: "Exportar documentos de varias páginas a imágenes rasterizadas(JPG, PNG, GIF, BMP, TIFF, WebP) usando C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /es/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words para .NET permite a los usuarios exportar documentos de varias páginas a imágenes rasterizadas. Esto puede ser útil para generar vistas previas, archivos o representaciones visuales de documentos para uso no editable.

## ¿Qué Formatos Admiten La Exportación de Varias páginas?

Aspose.Words admite la exportación de varias páginas a los siguientes formatos de imagen rasterizada:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Cómo Exportar un Documento de varias páginas a una Imagen

La función de exportar un documento de varias páginas a una imagen se implementa utilizando la clase [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/); puede especificar cómo se deben organizar las páginas al guardar en una imagen:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - guardar solo la primera de las páginas especificadas
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/): organice las páginas en una cuadrícula, de izquierda a derecha y de arriba a abajo, al tiempo que especifica el número de columnas
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - organice las páginas horizontalmente una al lado de la otra, de izquierda a derecha, en una sola salida
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - organice las páginas verticalmente una debajo de la otra en una sola salida
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/): organice cada página como un marco separado en una imagen TIFF de varios marcos, se aplica solo a los formatos de imagen TIFF

El siguiente ejemplo de código muestra cómo guardar un documento DOCX de varias páginas como una imagen JPEG con diseño horizontal:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

También puede personalizar la apariencia de la página del archivo de salida: especifique [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) y [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

El siguiente ejemplo de código muestra cómo guardar un documento DOCX de varias páginas como una imagen PNG con diseño de cuadrícula:

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