---
title: Resumir un Documento
second_title: Aspose.Words por C++
articleTitle: Resumir un Documento
linktitle: Resumir un Documento
type: docs
weight: 20
description: "Resumir un documento. Aspose.Words por C++ simplifica el resumen de documentos utilizando los modelos OpenAI y Google AI al permitirle especificar la longitud del resumen."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /es/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Resumir documentos es una herramienta valiosa para revisar contenido, obtener información rápida o preparar resúmenes. Aspose.Words admite el resumen de documentos mediante modelos impulsados por AI, lo que facilita el procesamiento de texto largo. Esta función, disponible en el espacio de nombres [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), integra modelos avanzados de lenguaje generativo de *OpenAI* y *Google*, así como *Claude's* modelos antrópicos de lenguaje generativo. La lista de modelos admitidos está disponible en la enumeración [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

Puede especificar varias opciones para resumir el contenido del documento. Utilice el método [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) para generar un resumen de su documento. También puede establecer la longitud del resumen utilizando la propiedad [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

Con Aspose.Words, implementar el resumen de documentos es sencillo. El siguiente ejemplo de código muestra cómo resumir un documento usando el modelo GPT-4o:

{{< highlight cpp >}}
void AiSummarize()
{
    auto firstDoc = MakeObject<Document>(MyDir + u"Big document.docx");
    auto secondDoc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"))->WithOrganization(u"Organization")->WithProject(u"Project");

    auto options = MakeObject<SummarizeOptions>();

    options->set_SummaryLength(SummaryLength::Short);
    auto firstDocumentSummary = model->Summarize(firstDoc, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.One.docx");

    System::ArrayPtr<System::SharedPtr<Document>> documents = System::MakeArray<System::SharedPtr<Document>>(2);
    documents[0] = firstDoc;
    documents[1] = secondDoc;

    options->set_SummaryLength(SummaryLength::Long);
    auto multiDocumentSummary = model->Summarize(documents, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.Multi.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Resumir documentos con Aspose.Words ahorra tiempo y le ayuda a concentrarse en la información esencial. Para obtener más información, consulte la documentación de [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
