---
title: לנקות לפני או במהלך Mail Merge פעולה
second_title: Aspose.Words עבור Java
articleTitle: לנקות לפני או במהלך Mail Merge פעולה
linktitle: לנקות לפני או במהלך Mail Merge פעולה
type: docs
description: "החל אפשרויות ניקוי והסרה שונות כגון מחיקת שדות מיזוג לפני ביצוע פעולת Mail Merge או הסרת אזורים שאינם בשימוש במהלך פעולת Mail Merge באמצעות Java."
keywords: "cleanup options Mail Merge c#"
weight: 10
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/java/clean-up-before-or-during-mail-merge/
timestamp: 2024-01-27-14-07-04
---

Aspose.Words מאפשר לך להחיל אפשרויות ניקוי והסרה שונות כגון מחיקת שדות מיזוג לפני ביצוע פעולת Mail Merge או הסרת אזורים שאינם בשימוש במהלך פעולת Mail Merge. סעיף זה יסביר כיצד למחוק שדות ממוזגים וכיצד להגדיר אפשרות הסרה.

## מחק שדות ממוזגים

כאשר אתה משתמש בתבנית ארוכה כלשהי שנוצרה על ידי מישהו אחר, ייתכן שתרצה למחוק את כל שדות המיזוג שכבר קיימים בתבנית זו לפני ביצוע פעולת Mail Merge. ניתן להשתמש בשיטת [DeleteFields](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#deleteFields) אם ברצונך למחוק את כל שדות המיזוג ממסמך מבלי לבצע פעולה Mail Merge. שיטה זו אינה מושפעת מאפשרויות הסרה של המאפיין [CleanupOptions](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#getCleanupOptions) וביצועה מסיר רק שדות ממוזגים, לא שדות המכילים או פסקאות ריקות.

דוגמת הקוד הבאה מראה כיצד למחוק את כל שדות המיזוג מהתבנית מבלי לבצע פעולת Mail Merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-fields-GetFieldNames-DeleteFields.java" >}}

## הגדר אפשרות `Removing`

Aspose.Words מאפשר לך להסיר שדות, אזורים ופסקאות לא ממוזגים מתבנית במהלך פעולת Mail Merge באמצעות אפשרויות הסרה.

השתמש במאפיין **CleanupOptions** יחד עם הספירה [MailMergeCleanupOptions](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/) כדי להגדיר את אפשרות ההסרה. ציין אילו פריטים ברצונך להסיר על ידי בחירת האפשרויות הבאות (ניתן לשלב יותר מאחד):

* הסר פסקאות ריקות
* הסר אזורים שאינם בשימוש
* הסר שדות שאינם בשימוש
* הסר שדות המכילים
* הסר שדות סטטיים
* הסר שורות טבלה ריקות

אתה יכול לשקול שדה מיזוג כבלתי ממוזג באחד מהתנאים הבאים:

1. אם לשדה המיזוג במקור הנתונים אין עמודה או שדה מיפוי.
2. אם שדה המיזוג במקור הנתונים מכיל שדה מיפוי אך הנתונים בטלים.

{{% alert color="primary" %}}

אם אתה ממזג נתונים באמצעות מקורות נתונים נפרדים, אפשרויות ההסרה הללו יופעלו רק בשיחה האחרונה של שיטת הביצוע Mail Merge.

{{% /alert %}}

### הסר פסקאות ריקות

פסקה הכוללת רק שדות מיזוג תהיה ריקה כאשר תהליך Mail Merge מסיר את כל שדות המיזוג שלו כבלתי ממוזגים. פסקאות ריקות אלה יכולות להוסיף שטח לא רצוי ולשנות את מראה הדוח שנוצר. ייתכן שתתמודד עם שני מצבים עם פסקאות במהלך פעולת Mail Merge:

1. השדה Mail Merge ימוזג עם נתונים ריקים.
2. שדה המיזוג אינו בשימוש ויוסר.

בשני המצבים האפשרות **RemoveEmptyParagraphs** תסיר אוטומטית פסקאות ריקות מהמסמך. כמו כן, הוא יסיר את שדות המיזוג `TableStart` ו - TableEnd אם שאר הפסקה ריקה.

דוגמת הקוד הבאה מראה כיצד להסיר את הפסקאות הריקות:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeCleanUp-RemoveEmptyParagraphs.java" >}}

{{% alert color="primary" %}}

ניתן להוריד את קובץ המדגם של דוגמה זו מ [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Table%20with%20fields.docx).

{{% /alert %}}

### הסר אזורים שאינם בשימוש

בגרסאות קודמות של Aspose.Words, אזורים ריקים Mail Merge הוסרו מהמסמך באופן אוטומטי במהלך פעולת Mail Merge. עם הגרסה האחרונה של Aspose.wordים, אזורים ריקים Mail Merge נשארים לאחר פעולת Mail Merge כברירת מחדל. עם זאת, באפשרותך להשתמש באפשרות **RemoveUnusedRegions** כדי להסיר את האזורים שאינם בשימוש Mail Merge במהלך הפעולה Mail Merge. לדוגמה, ניתן למזג מסמך עם מקור נתונים ריק שאינו מכיל טבלאות נתונים המובילות לאזורים שאינם בשימוש במסמך.

דוגמת הקוד הבאה מראה כיצד להסיר את אזורי המיזוג שאינם בשימוש:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeCleanUp-RemoveUnmergedRegions.java" >}}

{{% alert color="primary" %}}

ניתן להוריד את קובץ המדגם של דוגמה זו מ [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20destination%20-%20Northwind%20suppliers.docx).

{{% /alert %}}

**הערה**

### הסר שדות שאינם בשימוש

Aspose.Words מאפשר לך להסיר שדות Mail Merge שאינם בשימוש על ידי הקצאת הדגל **RemoveUnusedFields** ל **CleanupOptions**. אפשרות זו תסיר שדות מיזוג שאין להם את הנתונים המתאימים במקור הנתונים.

דוגמת הקוד הבאה מראה כיצד להסיר שדות מיזוג שאינם בשימוש ממסמך באופן אוטומטי במהלך פעולת Mail Merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeCleanUp-RemoveUnusedFields.java" >}}

### הסרת שדות המכילים

שדה מיזוג יכול להיות כלול בתוך שדה אחר כגון שדה **IF** או שדה נוסחה. הסר שדה חיצוני זה כאשר שדה המיזוג ממוזג או מוסר מהמסמך.

דוגמת הקוד הבאה מראה כיצד להסיר שדות המכילים שדות מיזוג ממסמך:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeCleanUp-RemoveContainingFields.java" >}}

**הערה**

### הסר שורות טבלה ריקות

Aspose.Words מאפשר לך להסיר שורות טבלה ריקות על ידי הקצאת הדגל **RemoveEmptyTableRows** ל **CleanupOptions**. אפשרות זו תסיר שורות טבלה המכילות שדות מיזוג ריקים.

דוגמת הקוד הבאה מראה כיצד להסיר שורות טבלה ריקות המכילות Mail Merge אזורים ממסמך:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeCleanUp-RemoveEmptyTableRows.java" >}}
