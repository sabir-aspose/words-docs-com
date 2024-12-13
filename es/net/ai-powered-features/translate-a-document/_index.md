---
title: Traducir un documento
second_title: Aspose.Words para .NET
articleTitle: Traducir un documento
linktitle: Traducir un documento
type: docs
weight: 30
description: "Traducir un documento. Aspose.Words para .NET simplifica la traducción de documentos mediante los modelos de inteligencia artificial de Google, lo que le permite especificar el idioma de destino."
url: /es/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

La traducción de documentos es una opción que se necesita con frecuencia en la era de la alta digitalización. Aspose.Words admite la traducción de documentos mediante los modelos de lenguaje generativo de *Google*, lo que permite a los desarrolladores traducir el contenido de textos a más de 300 idiomas.

Utilice el método [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) para traducir sus documentos a cualquier idioma representado en la enumeración [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Tenga en cuenta que si el documento de origen contiene varios idiomas, el modelo basado en Google AI podrá traducir todos los idiomas admitidos. Si el modelo no puede reconocer el idioma en algunos fragmentos de texto, se le devolverá un documento con estos fragmentos sin traducir y con el resto del texto traducido.

El siguiente ejemplo de código muestra cómo utilizar el modelo *Gemini 1.5 Flash* en Aspose.Words para traducir un documento al árabe:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Traducir documentos con Aspose.Words ahorra tiempo y facilita la integración de la funcionalidad de traducción en sus proyectos. Para obtener más información, consulte la documentación de la API [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

{{% /alert %}}