---
title: Bir Belgeyi Özetleme
second_title: Aspose.Words için C++
articleTitle: Bir Belgeyi Özetleme
linktitle: Bir Belgeyi Özetleme
type: docs
weight: 20
description: "Bir belgeyi özetleyin. Aspose.Words için C++ özet uzunluğunu belirtmenize izin vererek OpenAI ve Google AI modellerini kullanarak belge özetlemeyi basitleştirir."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /tr/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Belgeleri özetlemek, içerik incelemesi, hızlı içgörüler veya özetler hazırlamak için değerli bir araçtır. Aspose.Words, AI destekli modelleri kullanarak belge özetlemeyi destekler ve uzun metnin işlenmesini kolaylaştırır. [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) ad alanında bulunan bu özellik, *OpenAI* ve *Google* 'ten gelişmiş üretici dil modellerinin yanı sıra *Claude's* antropik üretici dil modellerini entegre eder. Desteklenen modellerin listesi [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/) numaralandırmasında mevcuttur.

Belge içeriğini özetlemek için çeşitli seçenekler belirleyebilirsiniz. Belgenizin bir özetini oluşturmak için [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) yöntemini kullanın. [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/) özelliğini kullanarak özet uzunluğunu da ayarlayabilirsiniz.

Aspose.Words ile belge özetlemenin uygulanması basittir. Aşağıdaki kod örneği, GPT-4o modelini kullanarak bir belgenin nasıl özetleneceğini gösterir:

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

Belgeleri Aspose.Words ile özetlemek zaman kazandırır ve temel bilgilere odaklanmanıza yardımcı olur. Daha fazla bilgi için [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API belgelerine bakın.

{{% /alert %}}
