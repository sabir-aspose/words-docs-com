---
title: Low Code
second_title: Aspose.Words por .NET
articleTitle: Trabajar con Documentos Usando LowCode API
linktitle: Low Code
type: docs
description: "Simplifique las tareas de procesamiento de documentos como comparar, convertir, dividir, fusionar, buscar y reemplazar, y otras usando Low Code API. Aspose.Words LowCode API con una sintaxis limpia, resultados rápidos y un esfuerzo de codificación mínimo."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /es/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words por .NET proporciona el espacio de nombres [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/), que simplifica las tareas comunes de procesamiento de documentos. Este API está diseñado para desarrolladores que desean realizar operaciones de alto nivel, como comparación de documentos, extracción de contenido, conversión de imágenes y reemplazo de texto, con un mínimo esfuerzo.

El LowCode API es ideal para escenarios en los que la implementación rápida es más importante que un control detallado. Echemos un vistazo más de cerca a las LowCode capacidades de Aspose.Words por .NET.

{{% alert color="primary" %}}

Es importante tener en cuenta que LowCode API no le permite cambiar la estructura del documento.

{{% /alert %}}

## Funciones disponibles en LowCode API

El espacio de nombres `Aspose.Words.LowCode` actualmente admite:

* **Converting** documentos de un formato a otro
* **Comparing** documentos
* **Mail merging**
* **Reporting** basado en la sintaxis LINQ
* **Merging** documentos
* **Search and replace**
* **Digital signing** de documentos
* **Splitting** un documento en partes usando diferentes criterios
* Añadiendo un **watermark**

{{% alert color="primary" %}}

Tenga en cuenta que puede encontrar una descripción detallada de cada función fuera de Low Code en la sección Guía del desarrollador.

{{% /alert %}}

## Fluido y No fluido API

Aspose.Words por .NET admite tanto fluidez como fluidez APIs, lo que permite a los desarrolladores elegir el estilo que mejor se adapte a sus preferencias de codificación y necesidades del proyecto. Veamos algunos ejemplos para ver cómo difieren estos dos tipos de API.

{{% alert color="primary" %}}

En Fluent API, las operaciones se pueden configurar y ejecutar a través de un contexto (como ComparerContext o ReplacerContext). Este contexto contiene opciones comunes. Garantiza que todos los métodos relacionados funcionen con una configuración coherente, lo que hace que API sea potente y fácil de administrar en escenarios complejos.

{{% /alert %}}

### Comparar Documentos

Utilice `LowCode` para comparar dos documentos Word y guardar el resultado.

**ejemplo de API no fluida:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**ejemplo de API fluida:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

También puede pasar `CompareOptions` para una comparación ajustada.

**ejemplo de API no fluida:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

CompareOptions options = new CompareOptions
{
    IgnoreFormatting = true,
    IgnoreCaseChanges = true
};

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc, options);
{{< /highlight >}}

**ejemplo de API fluida:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

ComparerContext comparerContext = new ComparerContext();
comparerContext.CompareOptions.IgnoreCaseChanges = true;

Comparer.Create(comparerContext)
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.3.docx")
   .Execute();
{{< /highlight >}}

### Convertir Documento a Imágenes

Utilice `LowCode` para convertir Word documento en PDF.

**ejemplo de API no fluida:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**ejemplo de API fluida:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Buscar y Reemplazar texto

Utilice `LowCode` para reemplazar texto rápidamente en todo el documento.

**ejemplo de API no fluida:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**ejemplo de API fluida:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";

ReplacerContext replacerContext = new ReplacerContext();
replacerContext.SetReplacement("ReplaceMe", "Replacement");

Replacer.Create(replacerContext)
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

## Por qué usar Aspose.Words Low Code

El espacio de nombres **Aspose.Words.LowCode** le ayuda a implementar tareas de procesamiento de documentos de alto nivel rápidamente con una sintaxis limpia y legible. Es especialmente útil para desarrolladores que necesitan velocidad, simplicidad y código mantenible cuando trabajan con documentos Word.

Para explorar opciones más avanzadas, siempre puede combinar LowCode APIs con el modelo de objetos Aspose.Words completo. Vea más Low Code ejemplos en [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).