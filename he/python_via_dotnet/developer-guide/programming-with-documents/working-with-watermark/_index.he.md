---
title: עבודה עם סימן מים ב Python
second_title: Aspose.Words עבור Python via .NET
articleTitle: עבודה עם סימן מים
linktitle: עבודה עם סימן מים
description: "צור ונהל סימני מים במסמך באמצעות Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

נושא זה דן כיצד לעבוד באופן פרוגרמטי עם סימן מים באמצעות Aspose.Words. סימן מים הוא תמונת רקע המוצגת מאחורי הטקסט במסמך. סימן מים יכול להכיל טקסט או תמונה המיוצגת על ידי הכיתה [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**נסה באינטרנט**

אתה יכול לנסות את הפונקציונליות הזו עם שלנו [סימן מים למסמכים מקוונים בחינם](https://products.aspose.app/words/watermark).

{{% /alert %}}

## כיצד להוסיף סימן מים למסמך

ב Microsoft Word, ניתן להכניס בקלות סימן מים למסמך באמצעות הפקודה הוסף סימן מים. Aspose.Words מספק את הכיתה [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) כדי להוסיף או להסיר סימן מים במסמכים. Aspose.Words מספק את הספירה [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) המגדירה שלושה סוגים אפשריים של סימני מים ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) ו [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) לעבוד איתם.

### הוסף סימן מים טקסט

דוגמת הקוד הבאה מראה כיצד להוסיף סימן מים טקסט במסמך על ידי הגדרת [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) באמצעות שיטת [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### הוסף סימן מים לתמונה

דוגמת הקוד הבאה מראה כיצד להוסיף סימן מים לתמונה במסמך על ידי הגדרת [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) באמצעות שיטת [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

ניתן להוסיף סימן מים לתמונה כתמונה, מחרוזת או זרם.

ניתן להכניס את סימן המים גם באמצעות מחלקת צורה. קל מאוד להכניס כל צורה או תמונה לכותרת עליונה או תחתונה וכך ליצור סימן מים מכל סוג שניתן להעלות על הדעת.

הדוגמה הבאה של הקוד מכניסה סימן מים למסמך Word:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

ניתן להוריד את קובץ התבנית של דוגמה זו מ [כאן](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## הסר סימן מים ממסמך

המחלקה [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) מספקת את שיטת ההסרה להסרת סימן המים ממסמך.

דוגמת הקוד הבאה מראה כיצד להסיר סימן מים ממסמכים:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

אם סימני המים מתווספים באמצעות אובייקט הכיתה [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/), כדי להסיר את סימן המים ממסמך, עליך להגדיר רק את שם צורת סימן המים במהלך ההכנסה ולאחר מכן להסיר את צורת סימן המים בשם שהוקצה.

דוגמת הקוד הבאה מראה לך כיצד להגדיר את שם צורת סימן המים ולהסיר אותה מהמסמך:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## הוסף סימן מים בתא הטבלה

לפעמים אתה צריך להכניס סימן מים/תמונה לתא של טבלה ולהציג אותה מחוץ לטבלה, אתה יכול להשתמש במאפיין [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/). מאפיין זה מקבל או קובע דגל המציין אם הצורה מוצגת בתוך שולחן או מחוצה לו. שים לב שמאפיין זה פועל רק כאשר אתה מבצע אופטימיזציה של המסמך עבור Microsoft Word 2010 בשיטת [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

דוגמת הקוד הבאה מראה כיצד להשתמש במאפיין זה:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
