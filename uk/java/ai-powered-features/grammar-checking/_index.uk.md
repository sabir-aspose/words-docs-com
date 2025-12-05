---
title: AI перевірка граматики
second_title: Aspose.Words для Java
articleTitle: Перевірка граматики
linktitle: Перевірка граматики
type: docs
weight: 40
description: "Перевірте граматику документа. Aspose.Words для Java дозволяє користувачам перевіряти граматику та виявляти помилки в документах за допомогою моделей OpenAI, Google та Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Перевірка граматики в документах важлива для забезпечення ясності, професіоналізму та точності. Грамотно складені документи залишають позитивне враження і дозволяють уникнути непорозумінь. Перевірка граматики допомагає швидко виявляти та виправляти помилки, заощаджуючи час та покращуючи якість.

Aspose.Words дозволяє користувачам перевіряти граматику та виявляти помилки в документах, використовуючи сімейства моделей OpenAI, Google та Claude, перелічені у списку [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). Використовуйте метод [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) для аналізу тексту в документі та виявлення граматичних проблем.

Наступний приклад коду показує, як використовувати модель GPT-4o mini в Aspose.Words для перевірки граматики:

{{< highlight java >}}
 Document doc = new Document("Big document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI generative language models.
 IAiModelText model = (OpenAiModel)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
 grammarOptions.setImproveStylistics(true);

 Document proofedDoc = model.checkGrammar(doc, grammarOptions);
 proofedDoc.save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Перевірка граматики за допомогою Aspose.Words покращує якість вашої роботи та полегшує впровадження коректури у ваші проекти. Для отримання додаткової інформації ознайомтеся з [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}