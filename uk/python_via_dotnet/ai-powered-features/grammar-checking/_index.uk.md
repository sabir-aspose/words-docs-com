---
title: AI перевірка граматики
second_title: Aspose.Words для Python via .NET
articleTitle: Перевірка граматики
linktitle: Перевірка граматики
type: docs
weight: 40
description: "Перевірте граматику документа. Aspose.Words для Python дозволяє користувачам перевіряти граматику та виявляти помилки в документах за допомогою моделей OpenAI, Google та Claude."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/python-net/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Перевірка граматики в документах важлива для забезпечення ясності, професіоналізму та точності. Грамотно складені документи залишають позитивне враження і дозволяють уникнути непорозумінь. Перевірка граматики допомагає швидко виявляти та виправляти помилки, заощаджуючи час та покращуючи якість.

Aspose.Words дозволяє користувачам перевіряти граматику та виявляти помилки в документах, використовуючи сімейства моделей OpenAI, Google та Claude, перелічені у списку [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). Використовуйте метод [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), доступний у просторі імен [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** аналізує текст у документі та виявляє граматичні проблеми.

Наступний приклад коду показує, як використовувати модель GPT-4o mini в Aspose.Words для перевірки граматики:

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

Перевірка граматики за допомогою Aspose.Words покращує якість вашої роботи та полегшує впровадження коректури у ваші проекти. Для отримання додаткової інформації перегляньте документацію [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}