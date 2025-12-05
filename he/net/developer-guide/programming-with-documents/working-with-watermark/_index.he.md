---
title: עבודה עם סימן מים ב C#
second_title: Aspose.Words עבור .NET
articleTitle: עבודה עם סימן מים
linktitle: עבודה עם סימן מים
description: "מסמך מניפולציה סימן מים באמצעות C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

נושא זה דן כיצד לעבוד באופן פרוגרמטי עם סימן מים באמצעות Aspose.Words. סימן מים הוא תמונת רקע המוצגת מאחורי הטקסט במסמך. סימן מים יכול להכיל טקסט או תמונה המיוצגת על ידי הכיתה [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**נסה באינטרנט**

אתה יכול לנסות את הפונקציונליות הזו עם שלנו [סימן מים למסמכים מקוונים בחינם](https://products.aspose.app/words/watermark).

{{% /alert %}}

## הוסף סימן מים למסמך

ב Microsoft Word, ניתן להכניס בקלות סימן מים למסמך באמצעות הפקודה הוסף סימן מים. Aspose.Words מספק את הכיתה [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) כדי להוסיף או להסיר סימן מים במסמכים. Aspose.Words מספק את הספירה [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)המגדירה שלושה סוגים אפשריים של סימני מים (טקסט, תמונה ואף אחד) לעבוד איתם.

### הוסף סימן מים טקסט

דוגמת הקוד הבאה מראה כיצד להוסיף סימן מים טקסט במסמך על ידי הגדרת [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) באמצעות שיטת [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### הוסף סימן מים לתמונה

דוגמת הקוד הבאה מראה כיצד להוסיף סימן מים לתמונה במסמך על ידי הגדרת [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) באמצעות שיטת [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

ניתן להוסיף סימן מים לתמונה כתמונה, מחרוזת או זרם.

ניתן להכניס את סימן המים גם באמצעות מחלקת צורה. קל מאוד להכניס כל צורה או תמונה לכותרת עליונה או תחתונה וכך ליצור סימן מים מכל סוג שניתן להעלות על הדעת.

הדוגמה הבאה של הקוד מכניסה סימן מים למסמך Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

ניתן להוריד את קובץ המדגם של דוגמה זו מ [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## הסר סימן מים ממסמך

המחלקה [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) מספקת את שיטת ההסרה להסרת סימן המים ממסמך.

דוגמת הקוד הבאה מראה כיצד להסיר סימן מים ממסמכים:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

אם סימני המים מתווספים באמצעות אובייקט הכיתה [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/), כדי להסיר את סימן המים ממסמך, עליך להגדיר רק את שם צורת סימן המים במהלך ההכנסה ולאחר מכן להסיר את צורת סימן המים בשם שהוקצה.

דוגמת הקוד הבאה מראה לך כיצד להגדיר את שם צורת סימן המים ולהסיר אותה מהמסמך:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## הוסף סימן מים לתא טבלה

לפעמים אתה צריך להכניס סימן מים/תמונה לתא של טבלה ולהציג אותה מחוץ לטבלה, אתה יכול להשתמש במאפיין [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). מאפיין זה מקבל או קובע דגל המציין אם הצורה מוצגת בתוך שולחן או מחוצה לו. שים לב שמאפיין זה פועל רק כאשר אתה מבצע אופטימיזציה של המסמך עבור Microsoft Word 2010 בשיטת [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

דוגמת הקוד הבאה מראה כיצד להשתמש במאפיין זה:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
