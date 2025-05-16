---
title: Resumir um documento
second_title: Aspose.Words Para C++
articleTitle: Resumir um documento
linktitle: Resumir um documento
type: docs
weight: 20
description: "Resuma um documento. Aspose.Words para C++ simplifica a sumarização de documentos utilizando os modelos OpenAI e Google AI, permitindo especificar o comprimento do resumo."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pt/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Resumir documentos é uma ferramenta valiosa para revisão de conteúdo, insights rápidos ou preparação de resumos. Aspose.Words suporta sumarização de documentos usando modelos com AI, facilitando o processamento de texto longo. Este recurso, disponível no namespace [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), integra modelos avançados de linguagem generativa de *OpenAI* e *Google*, bem como *Claude's* modelos antrópicos de linguagem generativa. A lista de modelos suportados está disponível na enumeração [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

Você pode especificar várias opções para resumir o conteúdo do documento. Use o método [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) para gerar um resumo do seu documento. Você também pode definir o comprimento do resumo usando a propriedade [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

Com Aspose.Words, a implementação do resumo do documento é simples. O exemplo de código a seguir mostra como resumir um documento usando o modelo GPT-4o:

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

Resumir documentos com Aspose.Words economiza tempo e ajuda você a se concentrar em informações essenciais. Para obter mais informações, consulte a documentação [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
