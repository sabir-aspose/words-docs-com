---
title: AI בדיקת דקדוק
second_title: Aspose.Words עבור .NET
articleTitle: בדיקת דקדוק
linktitle: בדיקת דקדוק
type: docs
weight: 40
description: "בדוק דקדוק מסמך. Aspose.Words עבור .NET מאפשר למשתמשים לבדוק דקדוק ולזהות שגיאות במסמכים באמצעות מודלים OpenAI."
url: /he/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

בדיקת דקדוק במסמכים חשובה כדי להבטיח בהירות, מקצועיות ודיוק. מסמכים כתובים היטב משאירים רושם חיובי ומונעים אי הבנות. בדיקות דקדוק עוזרות לזהות ולתקן שגיאות במהירות, חוסכות זמן ומשפרות את האיכות.

Aspose.Words מאפשר למשתמשים לבדוק דקדוק ולזהות שגיאות במסמכים באמצעות **OpenAI** מודלים גנראטיביים. השתמש בשיטת [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), הזמינה במרחב השמות [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/). **CheckGrammar** מנתח את הטקסט במסמך ומדגיש בעיות דקדוקיות.

דוגמת הקוד הבאה מראה כיצד להשתמש במודל GPT-4o mini ב Aspose.Words כדי לבדוק דקדוק:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Big document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use OpenAI generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gpt4OMini).WithApiKey(apiKey);

CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
grammarOptions.ImproveStylistics = true;

Document proofedDoc = model.CheckGrammar(doc, grammarOptions);
proofedDoc.Save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

בדיקת דקדוק עם Aspose.Words משפרת את איכות העבודה שלך ומקלה על שילוב הגהה בפרויקטים שלך. למידע נוסף, עיין בתיעוד [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}