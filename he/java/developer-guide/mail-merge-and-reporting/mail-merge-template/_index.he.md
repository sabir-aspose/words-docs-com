---
title: Mail Merge תבנית ב Java
second_title: Aspose.Words עבור Java
articleTitle: Mail Merge תבנית
linktitle: Mail Merge תבנית
type: docs
description: "צור תבנית Mail Merge להגדרת תוכן קבוע במסמכי פלט, ולאחר מכן צור מסמכי מיזוג באמצעות שדות המיזוג ב Java."
keywords: "create Mail Merge template Java, Mail Merge Java"
weight: 10
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /he/java/mail-merge-template/
timestamp: 2024-01-31-14-23-37
---

מקובל להשתמש בתבנית מיזוג כמסמך הבסיס לפעולה Mail Merge אם היא פשוטה Mail Merge או Mail Merge עם אזורים. Mail merge עם אזורים הוא חזק יותר פופולרי מאשר פשוט mail merge. Mail Merge פשוט נחשב למקרה מסוים של Mail Merge עם אזורים שבהם האזור הוא המסמך כולו. הכל מוסבר במאמר הבא" סוגי Mail Merge פעולה " בפירוט רב יותר.

התבנית מבטיחה שהטקסט במסמך הממוזג של הפלט מעוצב כהלכה, והפעולה Mail Merge מבטיחה שהטקסט ממקור הנתונים מוזן כהלכה בתבנית המיזוג.

Aspose.Words מספק את היכולת ליצור תבנית Mail Merge להגדרת תוכן קבוע ולאחר מכן ליצור מסמכי מיזוג באמצעות שדות המיזוג. לפיכך, לתבנית המיזוג יהיה הטקסט הדרוש, זהה בכל מסמכי הפלט, ושדות המיזוג למילוי התוכן המשתנה. כתוצאה מכך, מידע ממקור הנתונים שצוין יתווסף לתבנית המיזוג דרך שדות אלה במהלך יצירת המסמך הממוזג.

## מהי תבנית Mail Merge

תבנית Mail Merge היא מסמך מותאם אישית המכיל את הנתונים הקבועים ואת השדות הממוזגים שבהם ברצונך שהטקסט המשתנה יהיה. תבנית מיזוג יכולה להיות בכל פורמט התומך בשדות, למשל, DOC, DOCX, DOT, DOTX, RTF. בנוסף, ניתן גם להשתמש בתבנית mustache המוסברת במאמר "Mustache תחביר תבנית" ביתר פירוט.

אתה יכול ליצור תבנית מיזוג כדי להיות מודל למסמכים חדשים, והיא צריכה לכלול את הטקסט הראשי שצריך להיות זהה עבור כל גרסה של המסמך הממוזג. הוספת שדות מיזוג בתוך התבנית תייצג את נתוני ההתאמה האישית כגון שמות או כתובות שנלקחו ממקור נתונים. פעולה Mail Merge תכניס אוטומטית את נתוני ההתאמה האישית ממקור הנתונים למסמך תבנית המיזוג שלך.

בנוסף, תוכל להוסיף אזור Mail Merge בתבנית שלך על ידי הוספת שני שדות Mail Merge כדי לסמן את ההתחלה ואת הסוף של אזור הדואר. המאמר הבא" סוגי פעולה Mail Merge " מסביר זאת ביתר פירוט.

## צור תבנית Mail Merge

ניתן ליצור תבנית ולהוסיף לה שדות מיזוג ספציפיים, שיוחלפו בערכים ממקור הנתונים באופן ידני, לדוגמה, באמצעות Microsoft Word, או באמצעות תכנות Aspose.Words. במאמר זה, נבחן את הדרך הפרוגרמטית ליצירת תבנית.

השתמש בכיתה [DocumentBuilder](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/) כדי ליצור את תבנית המיזוג הנדרשת באמצעות Aspose.Words. אתה יכול לכלול טקסט, שדה מיזוג ומעבר שורה בתבנית כזו באמצעות [InsertTextInput](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertTextInput(java.lang.String,int,java.lang.String,java.lang.String,int)), [InsertField](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertField(int,boolean)), ו [InsertParagraph](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertParagraph()) שיטות.

דוגמת הקוד הבאה מראה כיצד ליצור תבנית Mail Merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeTemplate-CreateMailMergeTemplate.java" >}}

התמונה שלהלן מציגה את התבנית שנוצרה:

<img src="mail-merge-template-1.png" alt="mail_merge_template_aspose_words_java" style="width:650px"/>

## התאמה אישית של מאפייני תבנית Mail Merge

Aspose.Words מאפשר לך להתאים אישית את התבנית שלך באמצעות מאפיינים רבים. התאמה אישית של תבנית תתואר להלן באמצעות דוגמה להתאמה אישית של מאפיינים מסוימים של תמונות וטקסט.

### התאמה אישית של מאפייני תמונה

ניתן לציין את מאפייני התמונה באמצעות הכיתה [ImageFieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/). שים לב שאתה יכול להוסיף תמונה ממסד נתונים כפי שהיא מתוארת ב [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/c693ec7a8957051c206edc69612094a4169f6def/Examples/DocsExamples/Java/src/main/java/DocsExamples/Mail_Merge_And_Reporting/WorkingWithFields.java#L226).

דוגמת הקוד הבאה מראה כיצד לציין את שם קובץ התמונה וגודל התמונה:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-ImageFieldMerging.java" >}}

### התאמה אישית של מאפייני טקסט

אתה יכול להשתמש בכיתות [Text]https://reference.aspose.com/words/java/com.aspose.words/Fieldmergingargs#Text) property to insert text into the document for the current merge field. Also, you can change the formatting of texts and paragraphs inside your template using [Font](https://reference.aspose.com/words/java/com.aspose.words/font/) ו - [ParagraphFormat](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/). ניתן לטפל בטקסט שיוכנס לפני או אחרי שדה המיזוג באמצעות המאפיינים [TextBefore](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/#TextBefore) ו - [TextAfter](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/#TextAfter) הכלולים בכיתה [FieldMergeField](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/).

דוגמת הקוד הבאה מראה כיצד להוסיף תיבות סימון או HTML במהלך Mail Merge פעולה:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-MailMergeFormFields.java" >}}

{{% alert color="primary" %}}

ניתן להוריד את קובץ המדגם של דוגמה זו מ [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20destinations%20-%20Fax.docx).

אתה יכול גם לבדוק את יישום הכיתה `HandleMergeField` מ [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/DocsExamples/Java/src/main/java/DocsExamples/Mail_Merge_And_Reporting/WorkingWithFields.java).

{{% /alert %}}

## ראה גם

* לפרטים נוספים על אופן יצירת תבניות ב Microsoft Word באופן ידני, אנא בדוק את [צור תבנית](https://support.microsoft.com/en-us/office/save-a-word-document-as-a-template-cb17846d-ecec-49d4-82ea-a6f5e3e8b9ae) מאמר בתיעוד Microsoft
