---
title: סוגי Mail Merge פעולה ב Java
second_title: Aspose.Words עבור Java
articleTitle: סוגי Mail Merge פעולה
linktitle: סוגי Mail Merge פעולה
type: docs
description: "בצע שני סוגים שונים של פעולות Mail Merge: פשוט Mail Merge ו Mail Merge עם אזורים. פשוט Mail Merge חוזר על המסמך כולו לכל רשומה של מקור נתונים, בעוד Mail Merge עם אזורים חוזר רק על אזורים מוגדרים לכל רשומה באמצעות Java."
keywords: "how to execute Mail Merge java, Mail Merge Java, Simple Mail Merge"
weight: 20
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/java/types-of-mail-merge-operations/
timestamp: 2024-01-27-14-07-04
---

הרעיון המרכזי של Mail Merge הוא ליצור באופן אוטומטי מסמך או מספר מסמכים המבוססים על התבנית והנתונים שנלקחו ממקור הנתונים שלך. Aspose.Words מאפשר לך לבצע שני סוגים שונים של פעולות Mail Merge: פשוט Mail Merge ו Mail Merge עם אזורים.

הדוגמה הנפוצה ביותר לשימוש פשוט Mail Merge היא כאשר ברצונך לשלוח מסמך ללקוחות שונים על ידי הכללת שמותיהם בתחילת המסמך. לשם כך, עליך ליצור שדות מיזוג כגון *First Name* ו *Last Name* בתבנית שלך, ולאחר מכן למלא אותם בנתונים ממקור הנתונים שלך. ואילו הדוגמה הנפוצה ביותר לשימוש Mail Merge עם אזורים היא כאשר ברצונך לשלוח מסמך הכולל הזמנות ספציפיות עם רשימת כל הפריטים בכל הזמנה. לשם כך, יהיה עליך ליצור מיזוג אזורים בתוך אזור התבנית שלך עבור כל הזמנה, על מנת למלא אותו עם כל הנתונים הנדרשים עבור הפריטים.

ההבדל העיקרי בין שתי פעולות המיזוג הוא שפשוט Mail Merge (ללא אזורים) חוזר על המסמך כולו לכל רשומת מקור נתונים, ואילו Mail Merge עם אזורים חוזר רק על אזורים ייעודיים לכל רשומה. אתה יכול לחשוב על פעולה פשוטה Mail Merge כמקרה מסוים של מיזוג עם אזורים שבהם האזור היחיד הוא המסמך כולו.

{{% alert color="primary" %}}

הכיתה [MailMerge](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/) מייצגת פונקציונליות Mail Merge. עם המאפיינים שלה, אתה יכול להתאים אישית את ההתנהגות הנדרשת לפני ביצוע פעולה Mail Merge.

{{% /alert %}}

## פשוט Mail Merge פעולה {#simple-mail-merge-operation}

Mail Merge פשוט משמש למילוי השדות Mail Merge בתוך התבנית שלך בנתונים הנדרשים ממקור הנתונים שלך (ייצוג טבלה אחת). אז זה דומה לקלאסיקה Mail Merge ב Microsoft Word.

אתה יכול להוסיף שדה מיזוג אחד או יותר בתבנית שלך ואז לבצע את הפעולה הפשוטה Mail Merge. מומלץ להשתמש בו אם התבנית שלך אינה מכילה אזורי מיזוג.

המגבלה העיקרית בשימוש בסוג זה היא שכל תוכן המסמך יחזור על עצמו עבור כל רשומה במקור הנתונים.

### כיצד לבצע פעולה פשוטה Mail Merge {#how-to-execute-a-simple-mail-merge-operation}

לאחר שהתבנית שלך מוכנה, תוכל להתחיל לבצע את הפעולה הפשוטה Mail Merge. Aspose.Words מאפשר לך לבצע פשוט Mail Merge פעולה באמצעות שונה [Execute methods](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#execute-com.aspose.words.IMailMergeDataSource) שמקבלים אובייקטי נתונים שונים כמקור הנתונים.

דוגמת הקוד הבאה מראה כיצד לבצע פעולה פשוטה Mail Merge באמצעות אחת מהשיטות [Execute](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#execute-java.lang.String---java.lang.Object):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e"  "Examples-src-main-java-com-aspose-words-examples-mail_merge-TypesofMailMergeOperations-ExecuteSimpleMailMerge.java" >}}

אתה יכול להבחין בהבדל בין המסמך לפני ביצוע פשוט mail merge:

<img src="execute-simple-mail-merge-1.png" alt="simple_mail_merge_template_aspose_words_java" style="width:300px"/>

ואחרי ביצוע פשוט mail merge:

<img src="execute-simple-mail-merge-2.png" alt="execute_simple_mail_merge_aspose_words_java" style="width:300px"/>

### כיצד ליצור מסמכים ממוזגים מרובים

ב Aspose.Words, הפעולה הסטנדרטית Mail Merge ממלאת רק מסמך אחד בתוכן ממקור הנתונים שלך. לכן, יהיה עליך לבצע את פעולת Mail Merge מספר פעמים כדי ליצור מסמכים ממוזגים מרובים כפלט.

דוגמת הקוד הבאה מראה כיצד ליצור מסמכים מרובים הממוזגים במהלך פעולת Mail Merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e"  "Examples-src-main-java-com-aspose-words-examples-mail_merge-ProduceMultipleDocumentsDuringMailMerge-ProduceMultipleDocumentsDuringMailMerge.java" >}}

{{% alert color="primary" %}}

ניתן להוריד את קובץ המדגם של דוגמה זו מ [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/tree/master/Examples/src/main/resources/MailMerge).

{{% /alert %}}

## Mail Merge עם אזורים

אתה יכול ליצור אזורים שונים בתבנית שלך כדי שיהיו לך אזורים מיוחדים שאתה יכול פשוט למלא בנתונים שלך. השתמש ב Mail Merge עם אזורים אם ברצונך להוסיף טבלאות, שורות עם נתונים חוזרים כדי לגרום למסמכים שלך לצמוח באופן דינמי על ידי ציון אזורים אלה בתבנית שלך.

ניתן ליצור אזורים מקוננים (ילד) וכן למזג אזורים. היתרון העיקרי של שימוש בסוג זה הוא להגדיל באופן דינמי חלקים בתוך מסמך. ראה פרטים נוספים במאמר הבא"מקונן Mail Merge עם אזורים".

{{% alert color="primary" %}}

מידע על אזור Mail Merge ניתן להשיג באמצעות הכיתה [MailMergeRegionInfo](https://reference.aspose.com/words/java/com.aspose.words/mailmergeregioninfo/).

{{% /alert %}}

### כיצד לבצע Mail Merge עם אזורים

אזור Mail Merge הוא חלק ספציפי בתוך מסמך שיש לו נקודת התחלה ונקודת סיום. שתי הנקודות מיוצגות כשדות Mail Merge שיש להם שמות ספציפיים *"TableStart:XXX"* ו *"TableEnd:XXX"*. כל התוכן הכלול באזור Mail Merge יחזור על עצמו באופן אוטומטי עבור כל רשומה במקור הנתונים.

Aspose.Words מאפשר לך לבצע Mail Merge עם אזורים המשתמשים ב [Execute methods](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/executewithregions/#executewithregions/) שונים המקבלים אובייקטי נתונים שונים כמקור הנתונים.

כצעד ראשון, עלינו ליצור את `DataSet` כדי להעביר אותו מאוחר יותר כפרמטר קלט לשיטת `ExecuteWithRegions`:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e"  "Examples-src-main-java-com-aspose-words-examples-mail_merge-TypesofMailMergeOperations-CreateDataSet.java" >}}

דוגמת הקוד הבאה מראה כיצד לבצע Mail Merge עם אזורים באמצעות שיטת [ExecuteWithRegions(DataSet)](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#executeWithRegions-com.aspose.words.net.System.Data.DataSet):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e"  "Examples-src-main-java-com-aspose-words-examples-mail_merge-TypesofMailMergeOperations-MailMergeWithRegions.java" >}}

אתה יכול להבחין בהבדל בין המסמך לפני ביצוע Mail Merge עם אזורים:

<img src="execute-mail-merge-with-regions-1.png" alt="mail_merge_with_regions_template_aspose_words_java" style="width:850px"/>

ואחרי ביצוע Mail Merge עם אזורים:

<img src="execute-mail-merge-with-regions-2.png" alt="mail_merge_with_regions_execute_aspose_words_java" style="width:850px"/>

### מגבלות של Mail Merge עם אזורים

יש כמה נקודות חשובות שעליך לקחת בחשבון בעת ביצוע Mail Merge עם אזורים:

* נקודת ההתחלה *TableStart:Orders* ונקודת הסיום *TableEnd:Orders* שניהם צריכים להיות באותה שורה או תא. לדוגמה, אם אתה מפעיל אזור מיזוג בתא בטבלה, עליך לסיים את אזור המיזוג באותה שורה כמו התא הראשון.
* שם שדה המיזוג חייב להתאים לשם העמודה שלך DataTable. אלא אם כן ציינת שדות ממופים, Mail Merge עם אזורים לא יצליח עבור כל שדה מיזוג שיש לו שם שונה משם העמודה.

אם אחד הכללים האלה נשבר, תקבל תוצאות בלתי צפויות או חריג עשוי להיות נזרק.

{{% alert color="primary" %}}

אם אינך משתמש ב Mail Merge אזורים, אז זה יהיה דומה ל Microsoft Word mail merge, וכל תוכן המסמך יחזור על עצמו עבור כל רשומה במקור הנתונים.

{{% /alert %}}

