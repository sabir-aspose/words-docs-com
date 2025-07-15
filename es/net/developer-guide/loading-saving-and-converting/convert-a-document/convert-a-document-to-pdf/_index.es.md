---
title: Convertir Word a PDF en C#
second_title: Aspose.Words para .NET
articleTitle: Transformar documento a PDF
linktitle: Transformar documento a PDF
description: "Convertir Word a PDF en C#. Ejemplos de código simples para conversión DOCX a PDF. Compatible con todos los formatos Word e imágenes."
type: docs
weight: 10
url: /es/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

La capacidad de convertir documentos fácil y confiablemente de un formato a otro es una característica clave de Aspose.Words. PDF es uno de los formatos más populares para la conversión – es un formato de diseño fijo que preserva la apariencia original de un documento durante su renderizado en varias plataformas. El término "renderizado" se usa en Aspose.Words para describir el proceso de transformar un documento a un formato de archivo que está paginado o tiene el concepto de páginas.

## Convertir documento Word a PDF

La conversión de Word a PDF es un proceso bastante complejo que requiere varias etapas de cálculo. El motor de diseño de Aspose.Words imita la forma en que funciona el motor de diseño de páginas de Microsoft Word, haciendo que los documentos PDF de salida se vean lo más cerca posible a lo que puedes ver en Microsoft Word.

Con Aspose.Words puedes convertir programáticamente un documento desde formatos Word, como DOC o DOCX, a PDF sin usar Microsoft Office. Este artículo explica cómo realizar esta conversión.

{{% alert color="primary" %}}

Ten en cuenta que el número de páginas en un documento afecta el tiempo de conversión.

{{% /alert %}}

### Convertir DOCX o DOC a PDF

Transformar documentos DOC o DOCX al formato PDF en Aspose.Words es muy fácil y se puede lograr con solo dos líneas de código que:

1. Carga tu documento en un objeto [Document](https://reference.aspose.com/words/net/aspose.words/document/) usando uno de sus constructores especificando el nombre del documento con su extensión de formato.
1. Invoca uno de los métodos [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) en el objeto **Document** y especifica el formato de salida deseado como PDF ingresando un nombre de archivo con la extensión ".PDF".

El siguiente ejemplo de código muestra cómo convertir un documento de DOCX a PDF usando el método [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Puedes descargar el archivo de plantilla de este ejemplo desde [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

A veces es necesario especificar opciones adicionales que pueden afectar el resultado de guardar un documento como PDF. Estas opciones se pueden especificar usando la clase [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), que contiene propiedades que determinan cómo se mostrará la salida PDF.

Nota que con la misma técnica puedes transformar cualquier documento de formato de flujo a formato PDF.

{{% /alert %}}

### Convertir a diferentes estándares PDF

Aspose.Words proporciona la enumeración [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) para soportar la conversión de DOC o DOCX a varios estándares de formato PDF (como PDF 1.7, PDF 1.5, etc.).

El siguiente ejemplo de código demuestra cómo cambiar un documento a PDF 1.7 usando [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) con cumplimiento de PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Convertir imágenes a PDF

La conversión a PDF no está restringida a formatos de documento Microsoft Word. Cualquier formato soportado por Aspose.Words, incluyendo los creados programáticamente, también puede transformarse a PDF. Por ejemplo, podemos convertir imágenes de página única, como JPEG, PNG, BMP, EMF, o WMF, así como imágenes multipágina, como TIFF y GIF, a PDF.

El siguiente ejemplo de código muestra cómo cambiar imágenes JPEG y TIFF a PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Para que este código funcione, necesitas agregar referencias a Aspose.Words y `System.Drawing` a tu proyecto.

## Reducir el tamaño de salida PDF

Al guardar en PDF, puedes especificar si deseas optimizar la salida. Para hacer esto, necesitas establecer el flag [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) en true, y entonces se eliminarán los lienzos anidados redundantes y vacíos, se concatenarán los glifos vecinos con el mismo formato.

El siguiente ejemplo de código muestra cómo optimizar la salida:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Usar la propiedad **OptimizeOutput** puede afectar la precisión de la visualización del contenido.

{{% /alert %}}

## Ver también

- El artículo [Renderizado](/words/es/net/rendering/) para más información sobre los formatos de página fija y diseño de flujo
- El artículo [Conversión a formato de página fija](/words/net/converting-to-fixed-page-format/#what-is-a-page-layout) para más información sobre el diseño de página
- El artículo [Especificar opciones de renderizado al transformar a PDF](/words/es/net/specify-rendering-options-when-converting-to-pdf/) para más información sobre el uso de la clase `PdfSaveOptions`
- El artículo [Aprende las características de conversión a PDF/A y PDF/UA](/words/es/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) que describe qué estándar PDF y los ISO relevantes para estándares PDF soporta Aspose.Words
- El artículo [Qué estándar PDF es mejor elegir](/words/es/net/which-pdf-standard-is-better-to-choose/) para determinar qué estándares PDF tienen sentido para qué casos

- El artículo [Trabajar con PDF/A o PDF/UA](/words/es/net/working-with-pdfa-or-pdfua/) describe los requisitos para el contenido del documento en formatos PDF/A y PDF/UA – principalmente los requisitos para la estructura y fuentes

- El artículo [Advertencias de problemas de accesibilidad al guardar en PDF/A y PDF/UA](/words/es/net/warnings-when-saving-to-pdfa-and-pdfua/) describe qué requisitos de accesibilidad del contenido imponen PDF/A y PDF/UA
