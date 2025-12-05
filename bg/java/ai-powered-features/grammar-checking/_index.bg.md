---
title: AI Проверка На Граматиката
second_title: Aspose.Words за Java
articleTitle: Проверка На Граматиката
linktitle: Проверка На Граматиката
type: docs
weight: 40
description: "Проверете граматиката на документа. Aspose.Words за Java позволява на потребителите да проверяват граматиката и да откриват грешки в документи, използвайки модели OpenAI, Гугъл и Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Проверката на граматиката в документите е важна, за да се гарантира яснота, професионализъм и точност. Добре написаните документи оставят положително впечатление и избягват недоразумения. Проверките на граматиката помагат бързо да се идентифицират и коригират грешките, спестявайки време и подобрявайки качеството.

Aspose.Words позволява на потребителите да проверяват граматиката и да откриват грешки в документите, като използват семействата на моделите OpenAI, Гугъл и Claude, изброени в [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). Използвайте метода [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions), за да анализирате текста в документ и да подчертаете граматичните проблеми.

Следващият пример за код показва как да използвате модела GPT-4o mini в Aspose.Words, за да проверите граматиката:

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

Проверката на граматиката с Aspose.Words подобрява качеството на работата ви и улеснява интегрирането на корекцията във вашите проекти. За повече информация вижте [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}