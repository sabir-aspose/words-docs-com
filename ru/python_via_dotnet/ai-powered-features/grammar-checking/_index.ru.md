---
title: AI Проверка грамматики
second_title: Aspose.Words для Python via .NET
articleTitle: Проверка грамматики
linktitle: Проверка грамматики
type: docs
weight: 40
description: "Проверьте грамматику документа. Aspose.Words для Python позволяет пользователям проверять грамматику и обнаруживать ошибки в документах, используя модели OpenAI, Google и Claude."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ru/python-net/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Проверка грамматики в документах важна для обеспечения ясности, профессионализма и точности. Грамотно составленные документы оставляют положительное впечатление и позволяют избежать недоразумений. Проверка грамматики помогает быстро выявлять и исправлять ошибки, экономя время и повышая качество.

Aspose.Words позволяет пользователям проверять грамматику и обнаруживать ошибки в документах, используя семейства моделей OpenAI, Google и Claude, перечисленные в списке [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). Используйте метод [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), доступный в пространстве имен [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** анализирует текст в документе и выявляет грамматические проблемы.

В следующем примере кода показано, как использовать модель GPT-4o mini в Aspose.Words для проверки грамматики:

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

Проверка грамматики с помощью Aspose.Words повышает качество вашей работы и упрощает внедрение корректуры в ваши проекты. Для получения дополнительной информации ознакомьтесь с документацией [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}