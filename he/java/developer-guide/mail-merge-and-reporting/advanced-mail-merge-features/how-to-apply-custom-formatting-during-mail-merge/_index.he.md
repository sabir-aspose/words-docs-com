---
title: כיצד להחיל עיצוב מותאם אישית במהלך Mail Merge
second_title: Aspose.Words עבור Java
articleTitle: כיצד להחיל עיצוב מותאם אישית במהלך Mail Merge
linktitle: כיצד להחיל עיצוב מותאם אישית במהלך Mail Merge
type: docs
description: "החל עיצוב מותאם אישית במהלך פעולת Mail Merge באמצעות Java."
weight: 60
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/java/how-to-apply-custom-formatting-during-mail-merge/
timestamp: 2024-01-27-14-07-04
---

הכיתה [MailMerge](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/) מספקת שני אירועים שיכולים להיות שימושיים מאוד בהרחבת יכולות Mail Merge. המאפיין [setFieldMergingCallback(IFieldMergingCallback)](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#FieldMergingCallback) מקבל כיתה שמיישמת את השיטות [fieldMerging(FieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#fieldMerging-com.aspose.words.FieldMergingArgs) ו [imageFieldMerging(ImageFieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#imageFieldMerging-com.aspose.words.ImageFieldMergingArgs). ניתן להשתמש בהם כדי ליישם שליטה מותאמת אישית על תהליך Mail Merge.

האירוע **fieldMerging(FieldMergingArgs)** מתרחש במהלך Mail Merge כאשר שדה Mail Merge פשוט נתקל במסמך. זה נותן שליטה נוספת על Mail Merge ואתה יכול לבצע כל פעולה כאשר האירוע מתרחש. שיטה זו עטופה בכיתה שמיישמת את ממשק [IFieldMergingCallBack](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/) ומקבלת אובייקט [FieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/fieldmergingargs/) המספק נתונים לאירוע המתאים.

דוגמת הקוד המופיעה להלן מדגימה כיצד ליישם לוגיקה מותאמת אישית באירוע `MergeField` כדי להחיל עיצוב תאים.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomFormattingDuringMailMerge-ApplyCustomFormattingDuringMailMerge.java" >}}
