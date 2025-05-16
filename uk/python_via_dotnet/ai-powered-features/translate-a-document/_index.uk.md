---
title: Перекласти документ
second_title: Aspose.Words для Python via .NET
articleTitle: Перекласти документ
linktitle: Перекласти документ
type: docs
weight: 30
description: "Перекладіть документ. Aspose.Words для Python спрощує Переклад документів за допомогою моделей Google AI, дозволяючи вказати мову перекладу."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /uk/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Переклад документів-це часто необхідна опція в епоху високої цифровізації. Aspose.Words підтримує Переклад документів за допомогою *Google* моделей генеруючої мови, що дозволяє розробникам перекладати текстовий вміст більш ніж на 300 мов.

Використовуйте метод [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) для перекладу документів будь-якою мовою, представленою у списку [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). Зверніть увагу, що якщо оригінальний документ містить кілька мов, модель, заснована на Google AI, зможе перекласти всі підтримувані мови. Якщо модель не зможе розпізнати мову в деяких фрагментах тексту, Вам буде повернуто документ із цими неперекладеними фрагментами та перекладеним рештою тексту.

Наступний приклад коду показує, як використовувати модель *Gemini 1.5 Flash* в Aspose.Words для перекладу документа на арабську мову:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Переклад документів за допомогою Aspose.Words економить час та полегшує інтеграцію функцій перекладу у ваші проекти. Для отримання додаткової інформації перегляньте документацію [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}