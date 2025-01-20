---
title: 문서 번역
second_title: Aspose.Words.NET
articleTitle: 문서 번역
linktitle: 문서 번역
type: docs
weight: 30
description: "문서를 번역합니다. Aspose.Words에 대한.NET대상 언어를 지정할 수 있도록 구글AI모델을 사용하여 문서 번역을 단순화합니다."
url: /ko/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

문서 번역은 높은 디지털화 시대에 자주 필요한 옵션입니다. Aspose.Words*Google*생성 언어 모델을 사용하여 문서 번역을 지원하므로 개발자는 텍스트 콘텐츠를 300 개 이상의 언어로 번역할 수 있습니다.

[Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/)메서드를 사용하여[Language](https://reference.aspose.com/words/net/aspose.words.ai/language/)열거형에 표시된 모든 언어로 문서를 번역합니다. 소스 문서에 여러 언어가 포함되어 있으면 구글AI기반 모델이 지원되는 모든 언어를 번역할 수 있습니다. 모델이 일부 텍스트 조각의 언어를 인식할 수 없는 경우 이러한 번역되지 않은 조각과 나머지 텍스트가 번역된 문서가 반환됩니다.

다음 코드 예제에서는Aspose.Words에서*Gemini 1.5 Flash*모델을 사용하여 문서를 아랍어로 번역하는 방법을 보여 줍니다:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Words로 문서를 번역하면 시간을 절약하고 번역 기능을 프로젝트에 쉽게 통합 할 수 있습니다. 자세한 내용은[Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)API문서를 확인하십시오.

{{% /alert %}}