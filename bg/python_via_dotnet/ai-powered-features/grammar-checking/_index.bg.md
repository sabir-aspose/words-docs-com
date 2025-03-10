---
title: AI Проверка На Граматиката
second_title: Aspose.Words за Python via .NET
articleTitle: Проверка На Граматиката
linktitle: Проверка На Граматиката
type: docs
weight: 40
description: "Проверете граматиката на документа. Aspose.Words за Python позволява на потребителите да проверяват граматиката и да откриват грешки в документите, използвайки OpenAI модели."
url: /bg/python-net/grammar-checking/
timestamp: 2025-01-15-16-40-05
---

Проверката на граматиката в документите е важна, за да се гарантира яснота, професионализъм и точност. Добре написаните документи оставят положително впечатление и избягват недоразумения. Проверките на граматиката помагат бързо да се идентифицират и коригират грешките, спестявайки време и подобрявайки качеството.

Aspose.Words позволява на потребителите да проверяват граматиката и да откриват грешки в документите, използвайки **OpenAI** генеративни модели. Използвайте метода [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), Наличен в пространство от имена [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** анализира текста в документ и подчертава граматическите проблеми.

Следващият пример за код показва как да използвате модела GPT-4o mini в Aspose.Words, за да проверите граматиката:

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

Проверката на граматиката с Aspose.Words подобрява качеството на работата ви и улеснява интегрирането на корекцията във вашите проекти. За повече информация вижте документацията [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}