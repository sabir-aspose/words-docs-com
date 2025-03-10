---
title: AI문법 검사
second_title: Aspose.Words(으)로 Python via .NET
articleTitle: 문법 검사
linktitle: 문법 검사
type: docs
weight: 40
description: "문서 문법을 확인하십시오. Aspose.WordsPython의 경우 사용자가OpenAI모델을 사용하여 문법을 확인하고 문서의 오류를 감지할 수 있습니다."
url: /ko/python-net/grammar-checking/
timestamp: 2025-01-15-16-40-05
---

문서에서 문법을 확인하는 것은 명확성,전문성 및 정확성을 보장하는 데 중요합니다. 잘 작성된 문서는 긍정적 인 인상을 남기고 오해를 피합니다. 문법 검사는 오류를 신속하게 식별하고 수정하여 시간을 절약하고 품질을 향상시키는 데 도움이됩니다.

Aspose.Words사용자가 문법을 확인하고**OpenAI**생성 모델을 사용하여 문서의 오류를 감지 할 수 있습니다. [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)네임스페이스에서 사용할 수 있는[CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions)메서드를 사용합니다. **CheckGrammar**는 문서의 텍스트를 분석하고 문법적 문제를 강조합니다.

다음 코드 예제에서는Aspose.Words에서GPT-4o mini모델을 사용하여 문법을 확인하는 방법을 보여 줍니다:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + 'Big document.docx')

api_key = system_helper.environment.Environment.get_environment_variable('API_KEY')
# Use OpenAI generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GPT_4O_MINI).with_api_key(api_key).as_open_ai_model()

grammar_options = aw.ai.CheckGrammarOptions()
grammar_options.improve_stylistics = True

proofed_doc = model.check_grammar(doc, grammar_options)
proofed_doc.save(file_name='AI.AiGrammar.docx')
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Words으로 문법을 확인하면 작업의 질이 향상되고 교정을 프로젝트에 쉽게 통합 할 수 있습니다. 자세한 내용은[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)API문서를 확인하십시오.

{{% /alert %}}