---
title: AI문법 검사
second_title: Aspose.WordsC++
articleTitle: 문법 검사
linktitle: 문법 검사
type: docs
weight: 40
description: "문서 문법을 확인하십시오. C++에 대한Aspose.Words은 사용자가 문법을 확인하고OpenAI,구글,Claude모델을 사용하여 문서의 오류를 감지 할 수 있습니다."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ko/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

문서에서 문법을 확인하는 것은 명확성,전문성 및 정확성을 보장하는 데 중요합니다. 잘 작성된 문서는 긍정적 인 인상을 남기고 오해를 피합니다. 문법 검사는 오류를 신속하게 식별하고 수정하여 시간을 절약하고 품질을 향상시키는 데 도움이됩니다.

Aspose.Words사용자가 문법을 확인하고[AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/)열거에 나열된OpenAI,구글 및Claude모델의 패밀리를 사용하여 문서의 오류를 감지 할 수 있습니다. [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)네임스페이스에서 사용할 수 있는[CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/)메서드를 사용합니다. **CheckGrammar**문서의 텍스트를 분석하고 문법 문제를 강조 표시합니다.

다음 코드 예제에서는Aspose.Words에서GPT-4o mini모델을 사용하여 문법을 확인하는 방법을 보여 줍니다:

{{< highlight cpp >}}
void AiGrammar()
{
    auto doc = MakeObject<Document>(MyDir + u"Big document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto grammarOptions = MakeObject<CheckGrammarOptions>();
    grammarOptions->set_ImproveStylistics(true);

    auto proofedDoc = model->CheckGrammar(doc, grammarOptions);
    proofedDoc->Save(ArtifactsDir + u"AI.AiGrammar.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Words으로 문법을 확인하면 작업의 질이 향상되고 교정을 프로젝트에 쉽게 통합 할 수 있습니다. 자세한 내용은[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)API문서를 확인하십시오.

{{% /alert %}}