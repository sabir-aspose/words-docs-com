---
title: תרגם מסמך
second_title: Aspose.Words עבור NET
articleTitle: תרגם מסמך
linktitle: תרגם מסמך
type: docs
weight: 30
description: "תרגם מסמך. Aspose.Words עבור .NET מפשט את תרגום המסמכים באמצעות מודלים של AI של Google, ומאפשר לך לציין את שפת היעד."
url: /he/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

תרגום מסמכים הוא אופציה נחוצה לעתים קרובות בעידן הדיגיטליזציה הגבוהה. Aspose.Words תומכת בתרגום מסמכים באמצעות מודלים של *Google* של שפה, המאפשרת למפתחים לתרגם תוכן טקסט ליותר מ-300 שפות.

השתמש בשיטת [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) כדי לתרגם את המסמכים שלך לכל שפה המיוצגת ב-[Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) ספירה. שימו לב שאם מסמך המקור מכיל מספר שפות, המודל המבוסס על בינה מלאכותית של גוגל יוכל לתרגם את כל השפות הנתמכות. אם המודל לא יכול לזהות את השפה בחלק מקטעי טקסט, יוחזר לך מסמך עם קטעים לא מתורגמים אלה ועם שאר הטקסט מתורגם.

דוגמא הקוד הבאה מראה כיצד להשתמש במודל *Gemini 1.5 Flash* ב-Aspose.Words כדי לתרגם מסמך לערבית:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Words חוסך זמן ומקל על שילוב פונקציונליות התרגום בפרויקטים שלך. למידע נוסף, עיין בתיעוד ה-API של [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

{{% /alert %}}