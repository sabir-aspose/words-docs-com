---
title: AI בדיקת דקדוק
second_title: Aspose.Words עבור Python via .NET
articleTitle: בדיקת דקדוק
linktitle: בדיקת דקדוק
type: docs
weight: 40
description: "בדוק דקדוק מסמך. Aspose.Words עבור Python מאפשר למשתמשים לבדוק דקדוק ולזהות שגיאות במסמכים באמצעות מודלים OpenAI."
url: /he/python-net/grammar-checking/
timestamp: 2025-01-15-16-40-05
---

בדיקת דקדוק במסמכים חשובה כדי להבטיח בהירות, מקצועיות ודיוק. מסמכים כתובים היטב משאירים רושם חיובי ומונעים אי הבנות. בדיקות דקדוק עוזרות לזהות ולתקן שגיאות במהירות, חוסכות זמן ומשפרות את האיכות.

Aspose.Words מאפשר למשתמשים לבדוק דקדוק ולזהות שגיאות במסמכים באמצעות **OpenAI** מודלים גנראטיביים. השתמש בשיטת [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), הזמינה במרחב השמות [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** מנתח את הטקסט במסמך ומדגיש בעיות דקדוקיות.

דוגמת הקוד הבאה מראה כיצד להשתמש במודל GPT-4o mini ב Aspose.Words כדי לבדוק דקדוק:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + 'Big document.docx')

api_key = system_helper.environment.Environment.get_environment_variable('API_KEY')
# Use OpenAI generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GPT_4O_MINI).with_api_key(api_key).as_open_ai_model()

grammar_options = aw.ai.CheckGrammarOptions()
grammar_options.improve_stylistics = True

proofed_doc = model.check_grammar(doc, grammar_options)
proofed_doc.save(file_name='AI.AiGrammar.docx')
{{< /highlight >}}

{{% alert color="primary" %}}

בדיקת דקדוק עם Aspose.Words משפרת את איכות העבודה שלך ומקלה על שילוב הגהה בפרויקטים שלך. למידע נוסף, עיין בתיעוד [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}