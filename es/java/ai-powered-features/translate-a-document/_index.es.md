---
title: Traducir un Documento
second_title: Aspose.Words por Java
articleTitle: Traducir un Documento
linktitle: Traducir un Documento
type: docs
weight: 30
description: "Traducir un documento. Aspose.Words por Java simplifica la traducción de documentos mediante los modelos de Google AI, lo que le permite especificar el idioma de destino."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /es/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

La traducción de documentos es una opción que se necesita con frecuencia en la era de la alta digitalización. Aspose.Words admite la traducción de documentos mediante modelos de lenguaje generativos *Google*, lo que permite a los desarrolladores traducir contenido de textos a más de 300 idiomas.

Utilice el método [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) para traducir sus documentos a cualquier idioma representado en la enumeración [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). Tenga en cuenta que si el documento de origen contiene varios idiomas, el modelo basado en Google AI podrá traducir todos los idiomas admitidos. Si el modelo no puede reconocer el idioma en algunos fragmentos de texto, se le devolverá un documento con estos fragmentos sin traducir y con el resto del texto traducido.

El siguiente ejemplo de código muestra cómo usar el modelo *Gemini 1.5 Flash* en Aspose.Words para traducir un documento al árabe:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Traducir documentos con Aspose.Words ahorra tiempo y facilita la integración de la funcionalidad de traducción en sus proyectos. Para obtener más información, marque [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}