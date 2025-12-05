---
title: Resumir un Documento
second_title: Aspose.Words por Python via .NET
articleTitle: Resumir un Documento
linktitle: Resumir un Documento
type: docs
weight: 20
description: "Resumir un documento. Aspose.Words por Python simplifica el resumen de documentos utilizando los modelos OpenAI y Google AI al permitirle especificar la longitud del resumen."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /es/python-net/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Resumir documentos es una herramienta valiosa para revisar contenido, obtener información rápida o preparar resúmenes. Aspose.Words admite el resumen de documentos mediante modelos impulsados por AI, lo que facilita el procesamiento de texto largo. Esta función, disponible en el módulo [aspose.words.ai](https://reference.aspose.com/words/python-net/aspose.words.ai/), integra modelos avanzados de lenguaje generativo de *OpenAI* y *Google*, así como *Claude's* modelos antrópicos de lenguaje generativo. La lista de modelos admitidos está disponible en la enumeración [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/).

Puede especificar varias opciones para resumir el contenido del documento. Utilice el método [summarize](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/summarize/) para generar un resumen de su documento. También puede establecer la longitud del resumen utilizando la propiedad [summary_length](https://reference.aspose.com/words/python-net/aspose.words.ai/summarizeoptions/summary_length/).

Con Aspose.Words, implementar el resumen de documentos es sencillo. El siguiente ejemplo de código muestra cómo resumir un documento usando el modelo GPT-4o:

{{< highlight python >}}
first_doc = aw.Document(MyDir + "Big document.docx")
second_doc = aw.Document(MyDir + "Document.docx")
api_key = os.getenv("API_KEY")
# Use OpenAI or Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GPT_4O_MINI).with_api_key(api_key).as_open_ai_model()
options = aw.ai.SummarizeOptions()
options.summary_length = aw.ai.SummaryLength.SHORT
one_document_summary = model.summarize(first_doc, options)
oneDocumentSummary.save(ArtifactsDir + "AI.AiSummarize.One.docx")
options.summary_length = aw.ai.SummaryLength.LONG
multi_document_summary = model.summarize([first_doc, second_doc], options)
multiDocumentSummary.save(ArtifactsDir + "AI.AiSummarize.Multi.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Resumir documentos con Aspose.Words ahorra tiempo y le ayuda a concentrarse en la información esencial. Para obtener más información, consulte la documentación de [aspose.words.ai](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}