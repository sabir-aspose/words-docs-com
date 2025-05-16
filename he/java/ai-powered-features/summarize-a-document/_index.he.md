---
title: לסכם מסמך
second_title: Aspose.Words עבור Java
articleTitle: לסכם מסמך
linktitle: לסכם מסמך
type: docs
weight: 20
description: "סכם מסמך. Aspose.Words עבור Java מפשט את סיכום המסמכים באמצעות מודלים OpenAI וגוגל AI בכך שהוא מאפשר לך לציין את אורך הסיכום."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /he/java/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

סיכום מסמכים הוא כלי רב ערך לבדיקת תוכן, תובנות מהירות או הכנת תקצירים. Aspose.Words תומך בסיכום מסמכים באמצעות מודלים המופעלים על AI, מה שמקל על עיבוד טקסט ארוך. תכונה זו, הזמינה בפונקציונליות AI מבוססת Aspose.Words, משלבת מודלים מתקדמים של שפה גנראטיבית מ *OpenAI* ו *Google*, כמו גם *Claude's* מודלים של שפה גנראטיבית אנתרופית. רשימת הדגמים הנתמכים זמינה בספירה [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/).

ניתן לציין אפשרויות שונות לסיכום תוכן המסמך. השתמש בשיטת [Summarize](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#summarize-com.aspose.words.Document-com.aspose.words.SummarizeOptions) כדי ליצור סיכום של המסמך שלך. ניתן גם להגדיר אורך סיכום באמצעות המאפיין [SummaryLength](https://reference.aspose.com/words/java/com.aspose.words/summarizeoptions/#getSummaryLength).

עם Aspose.Words, יישום סיכום מסמכים הוא פשוט. דוגמת הקוד הבאה מראה כיצד לסכם מסמך באמצעות מודל GPT-4o:

{{< highlight java >}}
Document firstDoc = new Document(getMyDir() + "Big document.docx");
 Document secondDoc = new Document(getMyDir() + "Document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI or Google generative language models.
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 Document oneDocumentSummary = model.summarize(firstDoc, new SummarizeOptions(); { oneDocumentSummary.setSummaryLength(SummaryLength.SHORT); });
 oneDocumentSummary.save(getArtifactsDir() + "AI.AiSummarize.One.docx");

 Document multiDocumentSummary = model.summarize(new Document[] { firstDoc, secondDoc }, new SummarizeOptions(); { multiDocumentSummary.setSummaryLength(SummaryLength.LONG); });
 multiDocumentSummary.save(getArtifactsDir() + "AI.AiSummarize.Multi.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

סיכום מסמכים עם Aspose.Words חוסך זמן ועוזר לך להתמקד במידע חיוני. למידע נוסף, בדוק את [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}