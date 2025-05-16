---
title: Trabajar con marca de agua en Python
second_title: Aspose.Words por Python via .NET
articleTitle: Trabajar con Marca de Agua
linktitle: Trabajar con Marca de Agua
description: "Cree y administre marcas de agua en un documento usando Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /es/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

En este tema se analiza cómo trabajar mediante programación con watermark usando Aspose.Words. Una marca de agua es una imagen de fondo que se muestra detrás del texto de un documento. Una marca de agua puede contener un texto o una imagen representada por la clase [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Pruébalo en línea**

Puede probar esta funcionalidad con nuestro [Marca de agua gratuita para documentos en línea](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Cómo Agregar una marca de Agua a un Documento

En Microsoft Word, se puede insertar fácilmente una marca de agua en un documento mediante el comando Insertar marca de agua. Aspose.Words proporciona la clase [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) para agregar o eliminar marcas de agua en documentos. Aspose.Words proporciona la enumeración [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) que define tres tipos posibles de marcas de agua ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) y [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) con las que trabajar.

### Agregar Marca de Agua de Texto

El siguiente ejemplo de código demuestra cómo insertar una marca de agua de texto en un documento definiendo [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) con el método [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### Agregar Marca de Agua de Imagen

El siguiente ejemplo de código demuestra cómo insertar una marca de agua de imagen en un documento definiendo [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) con el método [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

La marca de agua de la imagen se puede insertar como imagen, cadena o secuencia.

La marca de agua también se puede insertar usando la clase shape. Es muy fácil insertar cualquier forma o imagen en un encabezado o pie de página y así crear una marca de agua de cualquier tipo imaginable.

El siguiente ejemplo de código inserta una marca de agua en un documento Word:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

Puede descargar el archivo de plantilla de este ejemplo desde [aquí](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Eliminar marca de agua de un Documento

La clase [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) proporciona el método remove para eliminar la marca de agua de un documento.

El siguiente ejemplo de código muestra cómo eliminar una marca de agua de los documentos:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

Si las marcas de agua se agregan usando el objeto de clase [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/), para eliminar la marca de agua de un documento, debe establecer solo el nombre de la forma de la marca de agua durante la inserción y luego eliminar la forma de la marca de agua con un nombre asignado.

El siguiente ejemplo de código le muestra cómo establecer el nombre de la forma de la marca de agua y eliminarla del documento:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## Agregar una Marca de Agua en la Celda de la Tabla

A veces necesita insertar una marca de agua/imagen en la celda de una tabla y mostrarla fuera de la tabla, puede usar la propiedad [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/). Esta propiedad obtiene o establece un indicador que indica si la forma se muestra dentro de una tabla o fuera de ella. Tenga en cuenta que esta propiedad solo funciona cuando optimiza el documento para Microsoft Word 2010 utilizando el método [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

El siguiente ejemplo de código muestra cómo usar esta propiedad:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
