---
title: AI בדיקת דקדוק
second_title: Aspose.Words עבור Java
articleTitle: בדיקת דקדוק
linktitle: בדיקת דקדוק
type: docs
weight: 40
description: "בדוק דקדוק מסמך. Aspose.Words עבור Java מאפשר למשתמשים לבדוק דקדוק ולזהות שגיאות במסמכים באמצעות מודלים OpenAI, גוגל ו Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

בדיקת דקדוק במסמכים חשובה כדי להבטיח בהירות, מקצועיות ודיוק. מסמכים כתובים היטב משאירים רושם חיובי ומונעים אי הבנות. בדיקות דקדוק עוזרות לזהות ולתקן שגיאות במהירות, חוסכות זמן ומשפרות את האיכות.

Aspose.Words מאפשר למשתמשים לבדוק דקדוק ולזהות שגיאות במסמכים באמצעות משפחות הדגמים OpenAI, גוגל ו - Claude המפורטות בספירה [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). השתמש בשיטת [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) כדי לנתח את הטקסט במסמך ולהדגיש בעיות דקדוקיות.

דוגמת הקוד הבאה מראה כיצד להשתמש במודל GPT-4o mini ב Aspose.Words כדי לבדוק דקדוק:

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

בדיקת דקדוק עם Aspose.Words משפרת את איכות העבודה שלך ומקלה על שילוב הגהה בפרויקטים שלך. למידע נוסף, בדוק את [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}