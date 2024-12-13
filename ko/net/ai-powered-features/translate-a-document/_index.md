---
title: 문서 번역
second_title: .NET용 Aspose.Words
articleTitle: 문서 번역
linktitle: 문서 번역
type: docs
weight: 30
description: "문서를 번역하세요. .NET용 Aspose.Words는 Google AI 모델을 사용하여 문서 번역을 간소화하여 대상 언어를 지정할 수 있습니다."
url: /ko/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

문서 번역은 고도 디지털화 시대에 자주 필요한 옵션입니다. Aspose.Words는 *Google* 생성 언어 모델을 사용하여 문서 번역을 지원하여 개발자가 텍스트 콘텐츠를 300개 이상의 언어로 번역할 수 있습니다.

[Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) 메서드를 사용하여 문서를 [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) 열거형에 표현된 모든 언어로 번역합니다. 소스 문서에 여러 언어가 포함된 경우 Google AI 기반 모델은 지원되는 모든 언어를 번역할 수 있습니다. 모델이 일부 텍스트 조각에서 언어를 인식할 수 없는 경우 이러한 번역되지 않은 조각과 나머지 텍스트가 번역된 문서가 반환됩니다.

다음 코드 예제는 Aspose.Words에서 *Gemini 1.5 Flash* 모델을 사용하여 문서를 아랍어로 번역하는 방법을 보여줍니다.

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Words로 문서를 번역하면 시간이 절약되고 프로젝트에 번역 기능을 쉽게 통합할 수 있습니다. 자세한 내용은 [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API 문서를 확인하세요.

{{% /alert %}}