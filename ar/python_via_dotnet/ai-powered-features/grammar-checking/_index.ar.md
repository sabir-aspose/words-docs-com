---
title: AI التدقيق النحوي
second_title: Aspose.Words ل Python via .NET
articleTitle: التدقيق النحوي
linktitle: التدقيق النحوي
type: docs
weight: 40
description: "تحقق من قواعد المستند. Aspose.Words ل Python يسمح للمستخدمين بالتحقق من القواعد واكتشاف الأخطاء في المستندات باستخدام نماذج OpenAI وجوجل و Claude."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ar/python-net/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

يعد التحقق من القواعد في المستندات أمرا مهما لضمان الوضوح والاحتراف والدقة. تترك المستندات المكتوبة جيدا انطباعا إيجابيا وتتجنب سوء الفهم. تساعد عمليات التدقيق النحوي في تحديد الأخطاء وتصحيحها بسرعة، مما يوفر الوقت ويحسن الجودة.

Aspose.Words يسمح للمستخدمين بالتحقق من القواعد واكتشاف الأخطاء في المستندات باستخدام عائلات النماذج OpenAI وجوجل و Claude المدرجة في تعداد [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). استخدم طريقة [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions)، المتوفرة في مساحة الاسم [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** يحلل النص في وثيقة ويسلط الضوء على المشاكل النحوية.

يوضح مثال الكود التالي كيفية استخدام نموذج GPT-4o mini في Aspose.Words للتحقق من القواعد:

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

يؤدي التحقق من القواعد باستخدام Aspose.Words إلى تحسين جودة عملك ويجعل من السهل دمج التدقيق اللغوي في مشاريعك. لمزيد من المعلومات، راجع وثائق [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}