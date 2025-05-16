---
title: תרגום מסמך
second_title: Aspose.Words עבור Java
articleTitle: תרגום מסמך
linktitle: תרגום מסמך
type: docs
weight: 30
description: "תרגם מסמך. Aspose.Words עבור Java מפשט תרגום מסמכים באמצעות מודלים של גוגל AI, ומאפשר לך לציין את שפת היעד."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /he/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

תרגום מסמכים הוא אפשרות נחוצה לעתים קרובות בעידן הדיגיטליזציה הגבוהה. Aspose.Words תומך תרגום מסמכים באמצעות *Google* מודלים שפה גנראטיבית, המאפשר למפתחים לתרגם תוכן טקסטים ליותר מ -300 שפות.

השתמש בשיטת [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) כדי לתרגם את המסמכים שלך לכל שפה המיוצגת בספירה [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). שים לב שאם מסמך המקור מכיל מספר שפות, המודל המבוסס על גוגל AI יוכל לתרגם את כל השפות הנתמכות. אם המודל אינו יכול לזהות את השפה בחלק מקטעי הטקסט, יוחזר לך מסמך עם השברים הלא מתורגמים הללו ועם שאר הטקסט המתורגם.

דוגמת הקוד הבאה מראה כיצד להשתמש במודל *Gemini 1.5 Flash* ב Aspose.Words כדי לתרגם מסמך לערבית:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

תרגום מסמכים עם Aspose.Words חוסך זמן ומקל על שילוב פונקציונליות התרגום בפרויקטים שלך. למידע נוסף, בדוק את [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}