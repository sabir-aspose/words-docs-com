---
title: לסכם מסמך
second_title: Aspose.Words עבור C++
articleTitle: לסכם מסמך
linktitle: לסכם מסמך
type: docs
weight: 20
description: "סכם מסמך. Aspose.Words עבור C++ מפשט את סיכום המסמכים באמצעות מודלים OpenAI וגוגל AI בכך שהוא מאפשר לך לציין את אורך הסיכום."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /he/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

סיכום מסמכים הוא כלי רב ערך לבדיקת תוכן, תובנות מהירות או הכנת תקצירים. Aspose.Words תומך בסיכום מסמכים באמצעות מודלים המופעלים על AI, מה שמקל על עיבוד טקסט ארוך. תכונה זו, הזמינה במרחב השמות [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/), משלבת מודלים מתקדמים של שפות גנראטיביות מ *OpenAI* ו *Google*, כמו גם *Claude's* מודלים של שפות גנראטיביות אנתרופיות. רשימת הדגמים הנתמכים זמינה בספירה [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/).

ניתן לציין אפשרויות שונות לסיכום תוכן המסמך. השתמש בשיטה [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) כדי ליצור סיכום של המסמך שלך. ניתן גם להגדיר אורך סיכום באמצעות המאפיין [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

עם Aspose.Words, יישום סיכום מסמכים הוא פשוט. דוגמת הקוד הבאה מראה כיצד לסכם מסמך באמצעות מודל GPT-4o:

{{< highlight cpp >}}
void AiSummarize()
{
    auto firstDoc = MakeObject<Document>(MyDir + u"Big document.docx");
    auto secondDoc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"))->WithOrganization(u"Organization")->WithProject(u"Project");

    auto options = MakeObject<SummarizeOptions>();

    options->set_SummaryLength(SummaryLength::Short);
    auto firstDocumentSummary = model->Summarize(firstDoc, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.One.docx");

    System::ArrayPtr<System::SharedPtr<Document>> documents = System::MakeArray<System::SharedPtr<Document>>(2);
    documents[0] = firstDoc;
    documents[1] = secondDoc;

    options->set_SummaryLength(SummaryLength::Long);
    auto multiDocumentSummary = model->Summarize(documents, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.Multi.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

סיכום מסמכים עם Aspose.Words חוסך זמן ועוזר לך להתמקד במידע חיוני. למידע נוסף, עיין בתיעוד [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
