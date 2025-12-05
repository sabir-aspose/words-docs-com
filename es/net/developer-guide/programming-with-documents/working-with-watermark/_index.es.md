---
title: Trabajar con marca de agua en C#
second_title: Aspose.Words por .NET
articleTitle: Trabajar con Marca de Agua
linktitle: Trabajar con Marca de Agua
description: "Manipulación de marcas de agua de documentos usando C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /es/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

En este tema se analiza cómo trabajar mediante programación con watermark usando Aspose.Words. Una marca de agua es una imagen de fondo que se muestra detrás del texto de un documento. Una marca de agua puede contener un texto o una imagen representada por la clase [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Pruébalo en línea**

Puede probar esta funcionalidad con nuestro [Marca de agua gratuita para documentos en línea](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Agregar una marca de agua a un Documento

En Microsoft Word, se puede insertar fácilmente una marca de agua en un documento mediante el comando Insertar marca de agua. Aspose.Words proporciona la clase [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) para agregar o eliminar marcas de agua en documentos. Aspose.Words proporciona la enumeración [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)que define tres tipos posibles de marcas de agua (Texto, Imagen y Ninguna) con las que trabajar.

### Agregar Marca de Agua de Texto

El siguiente ejemplo de código demuestra cómo insertar una marca de agua de texto en un documento definiendo [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) con el método [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Agregar Marca de Agua de Imagen

El siguiente ejemplo de código demuestra cómo insertar una marca de agua de imagen en un documento definiendo [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) con el método [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

La marca de agua de la imagen se puede insertar como imagen, cadena o secuencia.

La marca de agua también se puede insertar usando la clase shape. Es muy fácil insertar cualquier forma o imagen en un encabezado o pie de página y así crear una marca de agua de cualquier tipo imaginable.

El siguiente ejemplo de código inserta una marca de agua en un documento Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Puede descargar el archivo de muestra de este ejemplo desde [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Eliminar marca de agua de un Documento

La clase [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) proporciona el método remove para eliminar la marca de agua de un documento.

El siguiente ejemplo de código muestra cómo eliminar una marca de agua de los documentos:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Si las marcas de agua se agregan usando el objeto de clase [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/), para eliminar la marca de agua de un documento, debe establecer solo el nombre de la forma de la marca de agua durante la inserción y luego eliminar la forma de la marca de agua con un nombre asignado.

El siguiente ejemplo de código le muestra cómo establecer el nombre de la forma de la marca de agua y eliminarla del documento:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Agregar una Marca de Agua a una Celda de la tabla

A veces necesita insertar una marca de agua/imagen en la celda de una tabla y mostrarla fuera de la tabla, puede usar la propiedad [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). Esta propiedad obtiene o establece un indicador que indica si la forma se muestra dentro de una tabla o fuera de ella. Tenga en cuenta que esta propiedad solo funciona cuando optimiza el documento para Microsoft Word 2010 utilizando el método [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

El siguiente ejemplo de código muestra cómo usar esta propiedad:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
