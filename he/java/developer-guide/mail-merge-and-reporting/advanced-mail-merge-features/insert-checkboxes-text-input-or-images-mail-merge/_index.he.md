---
title: הכנס Checkbox, קלט טקסט או תמונות במהלך Mail Merge
second_title: Aspose.Words עבור Java
articleTitle: הכנס Checkbox, קלט טקסט או תמונות
linktitle: הכנס Checkbox, קלט טקסט או תמונות
description: "הכנס checkboxאו שדות קלט טקסט במהלך Mail Merge באמצעות Java. הכנס גם תמונות ממסד נתונים במהלך Mail Merge ב Java."
type: docs
weight: 20
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/java/insert-checkboxes-text-input-or-images-mail-merge/
timestamp: 2024-01-27-14-07-04
---

מנוע המיזוג לוקח מסמך כקלט, מחפש בו שדות `MERGEFIELD` ומחליף אותם בנתונים המתקבלים ממקור הנתונים. בדרך כלל, טקסט רגיל ו HTML מוכנסים, אך Aspose.Words משתמשים יכולים גם ליצור מסמך המטפל בתרחישים יוצאי דופן יותר עבור שדות Mail Merge.

פונקציונליות Aspose.Words עוצמתית מאפשרת לך להרחיב את התהליך Mail Merge:

- הכנס checkboxשדות טופס קלט טקסט למסמך במהלך mail merge
- הוסף תמונות מכל אחסון מותאם אישית (קבצים, BLOB שדות, וכו').)

## הכנס Checkboxקלט טקסט במהלך Mail Merge

לפעמים יש צורך לבצע פעולת Mail Merge כך שלא יוחלף טקסט בשדה המיזוג, אלא שדה checkbox או קלט טקסט. למרות שזה לא התרחיש הנפוץ ביותר, זה מאוד שימושי למשימות מסוימות.

צילום המסך הבא של מסמך Word מציג תבנית עם שדות מיזוג:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-1](insert-checkboxes-html-or-images-during-mail-merge_1.jpeg)

צילום מסך זה של המסמך Word למטה מציג את המסמך שכבר נוצר:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-2](insert-checkboxes-html-or-images-during-mail-merge-2.png)

{{% alert color="primary" %}}

שימו לב שחלק מהשדות הוחלפו בטקסט רגיל, חלק מהשדות הוחלפו בשדות טופס checkbox, והשדה `Subject` הוחלף בשדה קלט טקסט.

{{% /alert %}}

דוגמת הקוד הבאה מראה כיצד להוסיף checkboxשדות טקסט ושדות טקסט למסמך במהלך mail merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-MailMergeFormFields.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-HandleMergeField.java" >}}

## הכנס תמונות במהלך Mail Merge

בעת ביצוע פעולת Mail Merge, ניתן להוסיף תמונות ממסד הנתונים למסמך באמצעות שדות מיוחדים Mail Merge. שדה התמונה Mail Merge הוא שדה מיזוג בשם תמונה: MyFieldName.

### הכנס תמונות ממסד נתונים

במהלך mail merge, כאשר שדה תמונה Mail Merge נתקל במסמך, האירוע [FieldMergingCallback](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#getFieldMergingCallback) יורה. אתה יכול להגיב לאירוע זה כדי להחזיר שם קובץ, זרם או אובייקט תמונה למנוע Mail Merge כך שניתן יהיה להכניס אותו למסמך.

דוגמת הקוד הבאה מראה כיצד להוסיף תמונות המאוחסנות בשדה מסד נתונים BLOB לדוח:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageFromBlob.java" >}}

### הגדר מאפייני תמונה במהלך Mail Merge

בעת מיזוג שדה מיזוג תמונות, ייתכן שתצטרך לפעמים לשלוט במאפייני תמונה שונים, כגון [WrapType](https://reference.aspose.com/words/java/com.aspose.words/wraptype/).

נכון לעכשיו, באמצעות [ImageFieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/) ניתן להגדיר רק מאפייני רוחב תמונה או גובה, בהתאמה. כדי להתגבר על בעיה זו, Aspose.Words מספק את המאפיין [Shape](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/#getShape), המאפשר לקבל שליטה מלאה על התמונה שהוכנסה או על כל צורה אחרת.

דוגמת הקוד הבאה מראה כיצד להגדיר מאפייני תמונה שונים:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-MailMergeImageField.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-FieldMergingHandler.java" >}}

