---
title: AI التدقيق النحوي
second_title: Aspose.Words ل Java
articleTitle: التدقيق النحوي
linktitle: التدقيق النحوي
type: docs
weight: 40
description: "تحقق من قواعد المستند. Aspose.Words ل Java يسمح للمستخدمين بالتحقق من القواعد واكتشاف الأخطاء في المستندات باستخدام نماذج OpenAI وجوجل و Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ar/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

يعد التحقق من القواعد في المستندات أمرا مهما لضمان الوضوح والاحتراف والدقة. تترك المستندات المكتوبة جيدا انطباعا إيجابيا وتتجنب سوء الفهم. تساعد عمليات التدقيق النحوي في تحديد الأخطاء وتصحيحها بسرعة، مما يوفر الوقت ويحسن الجودة.

Aspose.Words يسمح للمستخدمين بالتحقق من القواعد واكتشاف الأخطاء في المستندات باستخدام عائلات النماذج OpenAI وجوجل و Claude المدرجة في تعداد [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). استخدم طريقة [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) لتحليل النص في مستند وإبراز المشكلات النحوية.

يوضح مثال الكود التالي كيفية استخدام نموذج GPT-4o mini في Aspose.Words للتحقق من القواعد:

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

يؤدي التحقق من القواعد باستخدام Aspose.Words إلى تحسين جودة عملك ويجعل من السهل دمج التدقيق اللغوي في مشاريعك. لمزيد من المعلومات، تحقق من [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}