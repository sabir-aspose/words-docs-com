---
title: להמיר Word ל-PDF ב-C#
second_title: Aspose.Words עבור .NET
articleTitle: לתרגם מסמך ל-PDF
linktitle: לתרגם מסמך ל-PDF
description: "להמיר Word ל-PDF ב-C#. דוגמאות קוד פשוטות להמרת DOCX ל-PDF. תומך בכל פורמטי Word ותמונות."
type: docs
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

היכולת להמיר מסמכים בקלות ובאמינות מפורמט אחד לאחר היא תכונה מרכזית של Aspose.Words. PDF הוא אחד הפורמטים הפופולריים ביותר להמרה – זהו פורמט עם פריסה קבועה שמשמר את המראה המקורי של המסמך בעת עיבוד על פלטפורמות שונות. המונח "עיבוד" משמש ב-Aspose.Words לתיאור התהליך של המרת מסמך לפורמט קובץ המחולק לעמודים או בעל מושג של עמודים.

## להמיר מסמך Word ל-PDF

ההמרה מ-Word ל-PDF היא תהליך מורכב למדי הדורש כמה שלבי חישוב. מנוע הפריסה של Aspose.Words מחקה את אופן הפעולה של מנוע פריסת העמודים של Microsoft Word, מה שהופך את מסמכי ה-PDF הפלט להיראות קרובים ככל האפשר למה שאתה יכול לראות ב-Microsoft Word.

עם Aspose.Words אתה יכול לתרגם מסמך באופן פרוגרמטי מפורמטי Word, כמו DOC או DOCX, ל-PDF מבלי להשתמש ב-Microsoft Office. מאמר זה מסביר כיצד לבצע המרה זו.

{{% alert color="primary" %}}

שים לב שמספר העמודים במסמך משפיע על זמן ההמרה.

{{% /alert %}}

### להמיר DOCX או DOC ל-PDF

לחדש מסמכים מפורמט DOC או DOCX לפורמט PDF ב-Aspose.Words קל מאוד וניתן להשגה באמצעות שני שורות קוד בלבד:

1. טען את המסמך שלך לאובייקט [Document](https://reference.aspose.com/words/net/aspose.words/document/) באמצעות אחד מהבנאים שלו על ידי ציון שם המסמך עם סיומת הפורמט שלו.
1. הפעל אחת מהמתודות [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) על אובייקט **Document** וציין את פורמט הפלט הרצוי כ-PDF על ידי הזנת שם קובץ עם הסיומת ".PDF".

דוגמת הקוד הבאה מראה כיצד להמיר מסמך מ-DOCX ל-PDF באמצעות מתודת [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

אתה יכול להוריד את קובץ התבנית של דוגמה זו מ-[Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

לפעמים יש צורך לציין אפשרויות נוספות שיכולות להשפיע על התוצאה של שמירת מסמך כ-PDF. אפשרויות אלו יכולות להיות מצוינות באמצעות המחלקה [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), המכילה מאפיינים שקובעים כיצד יוצג הפלט של ה-PDF.

שים לב שבאותה טכניקה אתה יכול לחדש כל מסמך בפורמט פריסה זורמת לפורמט PDF.

{{% /alert %}}

### לתרגם לסטנדרטי PDF שונים

Aspose.Words מספק את האנומרציה [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) לתמיכה בהמרת DOC או DOCX לסטנדרטי פורמט PDF שונים (כמו PDF 1.7, PDF 1.5, וכו').

דוגמת הקוד הבאה מדגימה כיצד לחדש מסמך ל-PDF 1.7 באמצעות [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) עם התאמה ל-PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## להמיר תמונות ל-PDF

ההמרה ל-PDF אינה מוגבלת לפורמטי מסמכי Microsoft Word. כל פורמט הנתמך על ידי Aspose.Words, כולל אלו שנוצרו באופן פרוגרמטי, יכול גם להיות מתורגם ל-PDF. לדוגמה, אנו יכולים לתרגם תמונות בעלות עמוד יחיד, כמו JPEG, PNG, BMP, EMF, או WMF, כמו גם תמונות רב-עמודיות, כמו TIFF ו-GIF, ל-PDF.

דוגמת הקוד הבאה מראה כיצד לחדש תמונות JPEG ו-TIFF ל-PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

כדי שקוד זה יעבוד, אתה צריך להוסיף הפניות ל-Aspose.Words ול-`System.Drawing` לפרויקט שלך.

## להקטין את גודל הפלט PDF

בעת שמירה ל-PDF, אתה יכול לציין אם ברצונך לייעל את הפלט. לשם כך, עליך להגדיר את הדגל [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) ל-true, ואז קנבסים מקוננים מיותרים ורקים יוסרו, גליפים סמוכים עם אותו עיצוב ישורשרו.

דוגמת הקוד הבאה מראה כיצד לייעל את הפלט:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

השימוש במאפיין **OptimizeOutput** עשוי להשפיע על דיוק הצגת התוכן.

{{% /alert %}}

## ראה גם

- המאמר [עיבוד](/words/he/net/rendering/) למידע נוסף על פורמטי עמוד קבוע ופריסה זורמת
- המאמר [המרה לפורמט עמוד קבוע](/words/he/net/converting-to-fixed-page-format/#what-is-a-page-layout) למידע נוסף על פריסת עמוד
- המאמר [ציון אפשרויות עיבוד בעת תרגום ל-PDF](/words/he/net/specify-rendering-options-when-converting-to-pdf/) למידע נוסף על השימוש במחלקת `PdfSaveOptions`
- המאמר [למד על תכונות ההמרה ל-PDF/A ו-PDF/UA](/words/he/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) המתאר איזה סטנדרט PDF וה-ISO הרלוונטיים לסטנדרטי PDF נתמכים על ידי Aspose.Words
- המאמר [איזה סטנדרט PDF עדיף לבחור](/words/he/net/which-pdf-standard-is-better-to-choose/) לקביעת אילו סטנדרטי PDF מתאימים לאילו מקרים

- המאמר [עבודה עם PDF/A או PDF/UA](/words/he/net/working-with-pdfa-or-pdfua/) מתאר את הדרישות לתוכן המסמך בפורמטי PDF/A ו-PDF/UA – בעיקר הדרישות למבנה ולפונטים

- המאמר [אזהרות בעיות נגישות בעת שמירה ל-PDF/A ו-PDF/UA](/words/he/net/warnings-when-saving-to-pdfa-and-pdfua/) מתאר אילו דרישות נגישות תוכן מטילים PDF/A ו-PDF/UA
