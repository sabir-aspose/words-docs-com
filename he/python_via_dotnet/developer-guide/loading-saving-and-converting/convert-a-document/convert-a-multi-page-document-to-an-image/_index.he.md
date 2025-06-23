---
title: המרת מסמך מרובה עמודים לתמונה ב Python
second_title: Aspose.Words עבור Python
articleTitle: המרת מסמך מרובה עמודים לתמונה
linktitle: המרת מסמך מרובה עמודים לתמונה
type: docs
description: "ייצוא מסמכים מרובי עמודים לתמונות סריקה(JPG, PNG, GIF, BMP, TIFF, WebP) באמצעות Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /he/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words עבור Python via .NET מאפשר למשתמשים לייצא מסמכים מרובי עמודים לתמונות סריקה. זה יכול להיות שימושי ליצירת תצוגות מקדימות, ארכיונים או ייצוגים חזותיים של מסמכים לשימוש שאינו ניתן לעריכה.

## אילו פורמטים תומכים בייצוא מרובה עמודים?

Aspose.Words תומך ביצוא מרובה עמודים לפורמטים הבאים של תמונות רסטר:

* ג 'יי-פי-ג' י
* גיף
* פנגוויה
* ב. מ. פ
* טיף
* WebP

## כיצד לייצא מסמך מרובה עמודים לתמונה

התכונה של ייצוא מסמך מרובה עמודים לתמונה מיושמת באמצעות הכיתה [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) – ניתן לציין כיצד יש לארגן את הדפים בעת שמירה בתמונה:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - שמור רק את הראשון מבין הדפים שצוינו
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - סדר את הדפים ברשת, משמאל לימין ומלמעלה למטה, תוך ציון מספר העמודות
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - סדר את הדפים בצורה אופקית זה לצד זה, משמאל לימין, בפלט יחיד
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - סדר את הדפים אנכית אחד מתחת לשני בפלט יחיד
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - סדר כל עמוד כמסגרת נפרדת בתמונה מרובת מסגרות TIFF, חל רק על TIFF פורמטים של תמונות

דוגמת הקוד הבאה מראה כיצד לשמור מסמך מרובה עמודים DOCX כתמונה JPEG עם פריסה אופקית:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

ניתן גם להתאים אישית את מראה דף קובץ הפלט-ציין [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) ו [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

דוגמת הקוד הבאה מראה כיצד לשמור מסמך מרובה עמודים DOCX כתמונה PNG עם פריסת רשת:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.PNG)
# Set up a grid layout with:
# - 3 columns per row.
# - 10pts spacing between pages (horizontal and vertical).
options.page_layout = aw.saving.MultiPageLayout.grid(3, 10, 10)

# Customize the background and border.
options.page_layout.back_color = aspose.pydrawing.Color.light_gray
options.page_layout.border_color = aspose.pydrawing.Color.blue
options.page_layout.border_width = 2

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}