---
title: Перевести документ
second_title: Aspose.Words для Java
articleTitle: Перевести документ
linktitle: Перевести документ
type: docs
weight: 30
description: "Переведите документ. Aspose.Words для Java упрощает перевод документов с помощью моделей Google AI, позволяя указать язык перевода."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ru/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Перевод документов - это часто необходимая опция в эпоху высокой цифровизации. Aspose.Words поддерживает перевод документов с использованием *Google* моделей генерирующего языка, что позволяет разработчикам переводить текстовое содержимое более чем на 300 языков.

Используйте метод [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) для перевода ваших документов на любой язык, представленный в списке [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). Обратите внимание, что если исходный документ содержит несколько языков, модель, основанная на Google AI, сможет переводить все поддерживаемые языки. Если модель не сможет распознать язык в некоторых фрагментах текста, вам будет возвращен документ с этими непереведенными фрагментами и переведенным остальным текстом.

В следующем примере кода показано, как использовать модель *Gemini 1.5 Flash* в Aspose.Words для перевода документа на арабский язык:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Перевод документов с помощью Aspose.Words экономит время и упрощает интеграцию функций перевода в ваши проекты. Для получения дополнительной информации ознакомьтесь с [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}