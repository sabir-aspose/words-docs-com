---
title: תרגום מסמך
second_title: Aspose.Words עבור .NET
articleTitle: תרגום מסמך
linktitle: תרגום מסמך
type: docs
weight: 30
description: "תרגם מסמך. Aspose.Words עבור .NET מפשט תרגום מסמכים באמצעות מודלים של גוגל AI, ומאפשר לך לציין את שפת היעד."
url: /he/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

תרגום מסמכים הוא אפשרות נחוצה לעתים קרובות בעידן הדיגיטליזציה הגבוהה. Aspose.Words תומך תרגום מסמכים באמצעות *Google* מודלים שפה גנראטיבית, המאפשר למפתחים לתרגם תוכן טקסטים ליותר מ -300 שפות.

השתמש בשיטת [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) כדי לתרגם את המסמכים שלך לכל שפה המיוצגת בספירה [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). שים לב שאם מסמך המקור מכיל מספר שפות, המודל המבוסס על גוגל AI יוכל לתרגם את כל השפות הנתמכות. אם המודל אינו יכול לזהות את השפה בחלק מקטעי הטקסט, יוחזר לך מסמך עם השברים הלא מתורגמים הללו ועם שאר הטקסט המתורגם.

דוגמת הקוד הבאה מראה כיצד להשתמש במודל *Gemini 1.5 Flash* ב Aspose.Words כדי לתרגם מסמך לערבית:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

תרגום מסמכים עם Aspose.Words חוסך זמן ומקל על שילוב פונקציונליות התרגום בפרויקטים שלך. למידע נוסף, עיין בתיעוד [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}