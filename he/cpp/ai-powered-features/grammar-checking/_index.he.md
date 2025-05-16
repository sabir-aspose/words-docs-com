---
title: AI בדיקת דקדוק
second_title: Aspose.Words עבור C++
articleTitle: בדיקת דקדוק
linktitle: בדיקת דקדוק
type: docs
weight: 40
description: "בדוק דקדוק מסמך. Aspose.Words עבור C++ מאפשר למשתמשים לבדוק דקדוק ולזהות שגיאות במסמכים באמצעות מודלים OpenAI, גוגל ו Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /he/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

בדיקת דקדוק במסמכים חשובה כדי להבטיח בהירות, מקצועיות ודיוק. מסמכים כתובים היטב משאירים רושם חיובי ומונעים אי הבנות. בדיקות דקדוק עוזרות לזהות ולתקן שגיאות במהירות, חוסכות זמן ומשפרות את האיכות.

Aspose.Words מאפשר למשתמשים לבדוק דקדוק ולזהות שגיאות במסמכים באמצעות משפחות הדגמים OpenAI, גוגל ו Claude המפורטות בספירה [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). השתמש בשיטת [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), הזמינה במרחב השמות [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** מנתח את הטקסט במסמך ומדגיש בעיות דקדוקיות.

דוגמת הקוד הבאה מראה כיצד להשתמש במודל GPT-4o mini ב Aspose.Words כדי לבדוק דקדוק:

{{< highlight cpp >}}
void AiGrammar()
{
    auto doc = MakeObject<Document>(MyDir + u"Big document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto grammarOptions = MakeObject<CheckGrammarOptions>();
    grammarOptions->set_ImproveStylistics(true);

    auto proofedDoc = model->CheckGrammar(doc, grammarOptions);
    proofedDoc->Save(ArtifactsDir + u"AI.AiGrammar.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

בדיקת דקדוק עם Aspose.Words משפרת את איכות העבודה שלך ומקלה על שילוב הגהה בפרויקטים שלך. למידע נוסף, עיין בתיעוד [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}