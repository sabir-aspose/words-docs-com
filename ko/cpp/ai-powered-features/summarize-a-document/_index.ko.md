---
title: 문서 요약
second_title: Aspose.WordsC++
articleTitle: 문서 요약
linktitle: 문서 요약
type: docs
weight: 20
description: "문서를 요약합니다. Aspose.Words의 경우C++는 요약 길이를 지정할 수 있도록 하여OpenAI및 구글AI모델을 사용하여 문서 요약을 단순화합니다."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ko/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

문서 요약은 콘텐츠 검토,빠른 통찰력 또는 초록을 준비하는 데 유용한 도구입니다. Aspose.Words는AI전원 모델을 사용하여 문서 요약을 지원하므로 긴 텍스트를 더 쉽게 처리 할 수 있습니다. [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)네임스페이스에서 사용할 수 있는 이 기능은*OpenAI*및*Google*의 고급 생성 언어 모델과*Claude's*인성 생성 언어 모델을 통합합니다. 지원되는 모델 목록은[AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/)열거형에서 사용할 수 있습니다.

문서 내용을 요약하기 위한 다양한 옵션을 지정할 수 있습니다. [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/)메서드를 사용하여 문서 요약을 생성합니다. [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/)속성을 사용하여 요약 길이를 설정할 수도 있습니다.

Aspose.Words을 사용하면 문서 요약을 구현하는 것이 간단합니다. 다음 코드 예제에서는GPT-4o모델을 사용하여 문서를 요약하는 방법을 보여 줍니다:

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

Aspose.Words로 문서를 요약하면 시간을 절약하고 필수 정보에 집중할 수 있습니다. 자세한 내용은[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)API문서를 확인하십시오.

{{% /alert %}}
