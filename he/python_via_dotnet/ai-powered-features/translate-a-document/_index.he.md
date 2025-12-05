---
title: תרגום מסמך
second_title: Aspose.Words עבור Python via .NET
articleTitle: תרגום מסמך
linktitle: תרגום מסמך
type: docs
weight: 30
description: "תרגם מסמך. Aspose.Words עבור Python מפשט תרגום מסמכים באמצעות מודלים של גוגל AI, ומאפשר לך לציין את שפת היעד."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

תרגום מסמכים הוא אפשרות נחוצה לעתים קרובות בעידן הדיגיטליזציה הגבוהה. Aspose.Words תומך תרגום מסמכים באמצעות *Google* מודלים שפה גנראטיבית, המאפשר למפתחים לתרגם תוכן טקסטים ליותר מ -300 שפות.

השתמש בשיטת [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) כדי לתרגם את המסמכים שלך לכל שפה המיוצגת בספירה [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). שים לב שאם מסמך המקור מכיל מספר שפות, המודל המבוסס על גוגל AI יוכל לתרגם את כל השפות הנתמכות. אם המודל אינו יכול לזהות את השפה בחלק מקטעי הטקסט, יוחזר לך מסמך עם השברים הלא מתורגמים הללו ועם שאר הטקסט המתורגם.

דוגמת הקוד הבאה מראה כיצד להשתמש במודל *Gemini 1.5 Flash* ב Aspose.Words כדי לתרגם מסמך לערבית:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

תרגום מסמכים עם Aspose.Words חוסך זמן ומקל על שילוב פונקציונליות התרגום בפרויקטים שלך. למידע נוסף, עיין בתיעוד [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}