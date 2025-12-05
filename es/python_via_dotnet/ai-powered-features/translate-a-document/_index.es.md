---
title: Traducir un Documento
second_title: Aspose.Words por Python via .NET
articleTitle: Traducir un Documento
linktitle: Traducir un Documento
type: docs
weight: 30
description: "Traducir un documento. Aspose.Words por Python simplifica la traducción de documentos mediante los modelos de Google AI, lo que le permite especificar el idioma de destino."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /es/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

La traducción de documentos es una opción que se necesita con frecuencia en la era de la alta digitalización. Aspose.Words admite la traducción de documentos mediante modelos de lenguaje generativos *Google*, lo que permite a los desarrolladores traducir contenido de textos a más de 300 idiomas.

Utilice el método [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) para traducir sus documentos a cualquier idioma representado en la enumeración [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). Tenga en cuenta que si el documento de origen contiene varios idiomas, el modelo basado en Google AI podrá traducir todos los idiomas admitidos. Si el modelo no puede reconocer el idioma en algunos fragmentos de texto, se le devolverá un documento con estos fragmentos sin traducir y con el resto del texto traducido.

El siguiente ejemplo de código muestra cómo usar el modelo *Gemini 1.5 Flash* en Aspose.Words para traducir un documento al árabe:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Traducir documentos con Aspose.Words ahorra tiempo y facilita la integración de la funcionalidad de traducción en sus proyectos. Para obtener más información, consulte la documentación de [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}