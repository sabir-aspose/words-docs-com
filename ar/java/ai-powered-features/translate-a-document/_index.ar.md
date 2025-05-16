---
title: ترجمة وثيقة
second_title: Aspose.Words ل Java
articleTitle: ترجمة وثيقة
linktitle: ترجمة وثيقة
type: docs
weight: 30
description: "ترجمة وثيقة. Aspose.Words ل Java يبسط ترجمة المستندات باستخدام نماذج جوجل AI، مما يسمح لك بتحديد اللغة الهدف."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ar/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

تعد ترجمة المستندات خيارا مطلوبا بشكل متكرر في عصر الرقمنة العالية. Aspose.Words يدعم ترجمة المستندات باستخدام *Google* نماذج اللغة التوليدية، والتي تسمح للمطورين بترجمة محتوى النصوص إلى أكثر من 300 لغة.

استخدم طريقة [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) لترجمة مستنداتك إلى أي لغة ممثلة في تعداد [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). لاحظ أنه إذا كان المستند المصدر يحتوي على عدة لغات، فسيكون النموذج المستند إلى جوجل AI قادرا على ترجمة جميع اللغات المدعومة. إذا لم يتمكن النموذج من التعرف على اللغة في بعض أجزاء النص، فسيتم إرجاع مستند به هذه الأجزاء غير المترجمة ومع ترجمة بقية النص.

يوضح مثال الكود التالي كيفية استخدام نموذج *Gemini 1.5 Flash* في Aspose.Words لترجمة مستند إلى اللغة العربية:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

توفر ترجمة المستندات باستخدام Aspose.Words الوقت وتجعل من السهل دمج وظائف الترجمة في مشاريعك. لمزيد من المعلومات، تحقق من [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}