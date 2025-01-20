---
title: Перевести документ
second_title: Aspose.Words для Python via .NET
articleTitle: Перевести документ
linktitle: Перевести документ
type: docs
weight: 30
description: "Переведите документ. Aspose.Words для Python упрощает перевод документов с помощью моделей Google AI, позволяя указать язык перевода."
url: /ru/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Перевод документов - это часто необходимая опция в эпоху высокой цифровизации. Aspose.Words поддерживает перевод документов с использованием *Google* моделей генерирующего языка, что позволяет разработчикам переводить текстовое содержимое более чем на 300 языков.

Используйте метод [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) для перевода ваших документов на любой язык, представленный в списке [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). Обратите внимание, что если исходный документ содержит несколько языков, модель, основанная на Google AI, сможет переводить все поддерживаемые языки. Если модель не сможет распознать язык в некоторых фрагментах текста, вам будет возвращен документ с этими непереведенными фрагментами и переведенным остальным текстом.

В следующем примере кода показано, как использовать модель *Gemini 1.5 Flash* в Aspose.Words для перевода документа на арабский язык:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Перевод документов с помощью Aspose.Words экономит время и упрощает интеграцию функций перевода в ваши проекты. Для получения дополнительной информации ознакомьтесь с документацией [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}