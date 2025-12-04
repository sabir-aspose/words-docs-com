---
title: AI Проверка грамматики
second_title: Aspose.Words для Java
articleTitle: Проверка грамматики
linktitle: Проверка грамматики
type: docs
weight: 40
description: "Проверьте грамматику документа. Aspose.Words для Java позволяет пользователям проверять грамматику и обнаруживать ошибки в документах, используя модели OpenAI, Google и Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ru/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Проверка грамматики в документах важна для обеспечения ясности, профессионализма и точности. Грамотно составленные документы оставляют положительное впечатление и позволяют избежать недоразумений. Проверка грамматики помогает быстро выявлять и исправлять ошибки, экономя время и повышая качество.

Aspose.Words позволяет пользователям проверять грамматику и обнаруживать ошибки в документах, используя семейства моделей OpenAI, Google и Claude, перечисленные в списке [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). Используйте метод [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) для анализа текста в документе и выявления грамматических проблем.

В следующем примере кода показано, как использовать модель GPT-4o mini в Aspose.Words для проверки грамматики:

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

Проверка грамматики с помощью Aspose.Words повышает качество вашей работы и упрощает внедрение корректуры в ваши проекты. Для получения дополнительной информации ознакомьтесь с [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}