---
title: AI문법 검사
second_title: Aspose.WordsJava
articleTitle: 문법 검사
linktitle: 문법 검사
type: docs
weight: 40
description: "문서 문법을 확인하십시오. Java에 대한Aspose.Words은 사용자가 문법을 확인하고OpenAI,구글,Claude모델을 사용하여 문서의 오류를 감지 할 수 있습니다."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ko/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

문서에서 문법을 확인하는 것은 명확성,전문성 및 정확성을 보장하는 데 중요합니다. 잘 작성된 문서는 긍정적 인 인상을 남기고 오해를 피합니다. 문법 검사는 오류를 신속하게 식별하고 수정하여 시간을 절약하고 품질을 향상시키는 데 도움이됩니다.

Aspose.Words는 사용자가[AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/)열거에 나열된OpenAI,구글,Claude모델의 패밀리를 사용하여 문법을 확인하고 문서의 오류를 감지할 수 있도록 합니다. [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions)방법을 사용하여 문서의 텍스트를 분석하고 문법 문제를 강조 표시합니다.

다음 코드 예제에서는Aspose.Words에서GPT-4o mini모델을 사용하여 문법을 확인하는 방법을 보여 줍니다:

{{< highlight java >}}
 Document doc = new Document("Big document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI generative language models.
 IAiModelText model = (OpenAiModel)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
 grammarOptions.setImproveStylistics(true);

 Document proofedDoc = model.checkGrammar(doc, grammarOptions);
 proofedDoc.save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Words으로 문법을 확인하면 작업의 질이 향상되고 교정을 프로젝트에 쉽게 통합 할 수 있습니다. 자세한 내용은[Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/)을 확인하십시오.

{{% /alert %}}