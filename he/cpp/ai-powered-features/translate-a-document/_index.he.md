---
title: תרגום מסמך
second_title: Aspose.Words עבור C++
articleTitle: תרגום מסמך
linktitle: תרגום מסמך
type: docs
weight: 30
description: "תרגם מסמך. Aspose.Words עבור C++ מפשט תרגום מסמכים באמצעות מודלים של גוגל AI, ומאפשר לך לציין את שפת היעד."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

תרגום מסמכים הוא אפשרות נחוצה לעתים קרובות בעידן הדיגיטליזציה הגבוהה. Aspose.Words תומך תרגום מסמכים באמצעות *Google* מודלים שפה גנראטיבית, המאפשר למפתחים לתרגם תוכן טקסטים ליותר מ -300 שפות.

השתמש בשיטת [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) כדי לתרגם את המסמכים שלך לכל שפה המיוצגת בספירה [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/). שים לב שאם מסמך המקור מכיל מספר שפות, המודל המבוסס על גוגל AI יוכל לתרגם את כל השפות הנתמכות. אם המודל אינו יכול לזהות את השפה בחלק מקטעי הטקסט, יוחזר לך מסמך עם השברים הלא מתורגמים הללו ועם שאר הטקסט המתורגם.

דוגמת הקוד הבאה מראה כיצד להשתמש במודל *Gemini 1.5 Flash* ב Aspose.Words כדי לתרגם מסמך לערבית:

{{< highlight cpp >}}
void AiTranslate()
{
    auto doc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<GoogleAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto translatedDoc = model->Translate(doc, Language::Arabic);
    translatedDoc->Save(ArtifactsDir + u"AI.AiTranslate.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

תרגום מסמכים עם Aspose.Words חוסך זמן ומקל על שילוב פונקציונליות התרגום בפרויקטים שלך. למידע נוסף, עיין בתיעוד [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}