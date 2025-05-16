---
title: עבודה עם סימן מים ב Java
second_title: Aspose.Words עבור Java
articleTitle: עבודה עם סימן מים
linktitle: עבודה עם סימן מים
type: docs
description: "מסמך מניפולציה סימן מים באמצעות Java."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /he/java/working-with-watermark/
timestamp: 2025-04-22-08-07-04
---

נושא זה דן כיצד לעבוד באופן פרוגרמטי עם סימן מים באמצעות Aspose.Words. סימן מים הוא תמונת רקע המוצגת מאחורי הטקסט במסמך. סימן מים יכול להכיל טקסט או תמונה המיוצגת על ידי הכיתה [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/).

{{% alert color="primary" %}}

**נסה באינטרנט**

אתה יכול לנסות את הפונקציונליות הזו עם שלנו [סימן מים למסמכים מקוונים בחינם](https://products.aspose.app/words/watermark).

{{% /alert %}}

## הוסף סימן מים למסמך

ב Microsoft Word, ניתן להכניס בקלות סימן מים למסמך באמצעות הפקודה הוסף סימן מים. Aspose.Words מספק את הכיתה [watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) כדי להוסיף או להסיר סימן מים במסמכים. Aspose.Words מספק את הספירה [WatermarkType ](https://reference.aspose.com/words/java/com.aspose.words/watermarktype/)המגדירה שלושה סוגים אפשריים של סימני מים (טקסט, תמונה ואף אחד) לעבוד איתם.

### הוסף סימן מים טקסט

דוגמת הקוד הבאה מראה כיצד להוסיף סימן מים טקסט במסמך על ידי הגדרת [TextWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/textwatermarkoptions/) באמצעות שיטת [SetText](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setText-java.lang.String):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddTextWatermarkWithSpecificOptions.java" >}}

### הוסף סימן מים לתמונה

דוגמת הקוד הבאה מראה כיצד להוסיף סימן מים לתמונה במסמך על ידי הגדרת [ImageWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/imagewatermarkoptions/) באמצעות שיטת [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.awt.image.BufferedImage):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddImageWatermarkWithSpecificOptions.java" >}}

ניתן להוסיף סימן מים לתמונה כתמונה, מחרוזת או זרם.

ניתן להכניס את סימן המים גם באמצעות מחלקת צורה. קל מאוד להכניס כל צורה או תמונה לכותרת עליונה או תחתונה וכך ליצור סימן מים מכל סוג שניתן להעלות על הדעת.

הדוגמה הבאה של הקוד מכניסה סימן מים למסמך Word:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-AddWatermarkToADocument-AddWatermarkToADocument.java" >}}

{{% alert color="primary" %}}

ניתן להוריד את קובץ המדגם של דוגמה זו מ [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Document.doc).

{{% /alert %}}


## הסר סימן מים ממסמך

המחלקה [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) מספקת את השיטה `Remove` להסרת סימן המים ממסמך.

דוגמאות הקוד הבאות מראות כיצד להסיר סימן מים ממסמכים:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-RemoveWatermarkFromDocument.java" >}}

כדי להסיר את סימן המים ממסמך עליך להגדיר רק את שם צורת סימן המים במהלך ההכנסה ואז להסיר את צורת סימן המים בשם שהוקצה.

דוגמת הקוד הבאה מראה לך כיצד להגדיר את שם צורת סימן המים ולהסיר אותה מהמסמך:

{{< highlight csharp >}}

// Set name to be able to remove it afterwards
watermark.Name("WaterMark");
{{< /highlight >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-RemoveWatermark-RemoveWatermark.java" >}}

## הוסף סימן מים לתא טבלה

לפעמים אתה צריך להכניס סימן מים/תמונה לתא של טבלה ולהציג אותו מחוץ לטבלה, אתה יכול להשתמש במאפיין [IsLayoutInCell](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#isLayoutInCell-boolean). מאפיין זה מקבל או קובע דגל המציין אם הצורה מוצגת בתוך שולחן או מחוצה לו. שים לב שמאפיין זה פועל רק כאשר אתה מבצע אופטימיזציה של המסמך עבור Microsoft Word 2010 בשיטת [OptimizeFor](https://reference.aspose.com/words/java/com.aspose.words/compatibilityoptions/#optimizeFor-int).

דוגמת הקוד הבאה מראה כיצד להשתמש במאפיין זה:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-Shapes-WorkingWithShapes-SetShapeLayoutInCell.java" >}}
