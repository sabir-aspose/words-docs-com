---
title: המרת מסמך מרובה עמודים לתמונה ב Java
second_title: Aspose.Words עבור Java
articleTitle: המרת מסמך מרובה עמודים לתמונה
linktitle: המרת מסמך מרובה עמודים לתמונה
type: docs
description: "ייצוא מסמכים מרובי עמודים לתמונות סריקה(JPG, PNG, GIF, BMP, TIFF, WebP) באמצעות Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words עבור Java מאפשר למשתמשים לייצא מסמכים מרובי עמודים לתמונות סריקה. זה יכול להיות שימושי ליצירת תצוגות מקדימות, ארכיונים או ייצוגים חזותיים של מסמכים לשימוש שאינו ניתן לעריכה.

## אילו פורמטים תומכים בייצוא מרובה עמודים?

Aspose.Words תומך ביצוא מרובה עמודים לפורמטים הבאים של תמונות רסטר:

* ג 'יי-פי-ג' י
* גיף
* פנגוויה
* ב. מ. פ
* טיף
* WebP

## כיצד לייצא מסמך מרובה עמודים לתמונה

התכונה של ייצוא מסמך מרובה עמודים לתמונה מיושמת באמצעות הכיתה [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) – ניתן לציין כיצד יש לארגן את הדפים בעת שמירה בתמונה:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - שמור רק את הראשון מבין הדפים שצוינו
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - סדר את הדפים ברשת, משמאל לימין ומלמעלה למטה, תוך ציון מספר העמודות
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - סדר את הדפים בצורה אופקית זה לצד זה, משמאל לימין, בפלט יחיד
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - סדר את הדפים אנכית אחד מתחת לשני בפלט יחיד
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - סדר כל עמוד כמסגרת נפרדת בתמונה מרובת מסגרות TIFF, חל רק על TIFF פורמטים של תמונות

דוגמת הקוד הבאה מראה כיצד לשמור מסמך מרובה עמודים DOCX כתמונה JPEG עם פריסה אופקית:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

ניתן גם להתאים אישית את מראה דף קובץ הפלט-ציין [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) ו [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

דוגמת הקוד הבאה מראה כיצד לשמור מסמך מרובה עמודים DOCX כתמונה PNG עם פריסת רשת:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.PNG);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.setPageLayout(MultiPageLayout.grid(3, 10f, 10f));

// Customize the background and border.
options.getPageLayout().setBackColor(Color.lightGray);
options.getPageLayout().setBorderColor(Color.BLUE);
options.getPageLayout().setBorderWidth(2f);

doc.save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}