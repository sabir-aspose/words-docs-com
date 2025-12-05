---
title: המרת מסמך מרובה עמודים לתמונה ב C#
second_title: Aspose.Words עבור .NET
articleTitle: המרת מסמך מרובה עמודים לתמונה
linktitle: המרת מסמך מרובה עמודים לתמונה
type: docs
description: "ייצוא מסמכים מרובי עמודים לתמונות סריקה(JPG, PNG, GIF, BMP, TIFF, WebP) באמצעות C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /he/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words עבור .NET מאפשר למשתמשים לייצא מסמכים מרובי עמודים לתמונות סריקה. זה יכול להיות שימושי ליצירת תצוגות מקדימות, ארכיונים או ייצוגים חזותיים של מסמכים לשימוש שאינו ניתן לעריכה.

## אילו פורמטים תומכים בייצוא מרובה עמודים?

Aspose.Words תומך ביצוא מרובה עמודים לפורמטים הבאים של תמונות רסטר:

* ג 'יי-פי-ג' י
* גיף
* פנגוויה
* ב. מ. פ
* טיף
* WebP

## כיצד לייצא מסמך מרובה עמודים לתמונה

התכונה של ייצוא מסמך מרובה עמודים לתמונה מיושמת באמצעות הכיתה [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) – ניתן לציין כיצד יש לארגן את הדפים בעת שמירה בתמונה:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - שמור רק את הראשון מבין הדפים שצוינו
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - סדר את הדפים ברשת, משמאל לימין ומלמעלה למטה, תוך ציון מספר העמודות
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - סדר את הדפים בצורה אופקית זה לצד זה, משמאל לימין, בפלט יחיד
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - סדר את הדפים אנכית אחד מתחת לשני בפלט יחיד
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - סדר כל עמוד כמסגרת נפרדת בתמונה מרובת מסגרות TIFF, חל רק על TIFF פורמטים של תמונות

דוגמת הקוד הבאה מראה כיצד לשמור מסמך מרובה עמודים DOCX כתמונה JPEG עם פריסה אופקית:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

ניתן גם להתאים אישית את מראה דף קובץ הפלט-ציין [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) ו [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

דוגמת הקוד הבאה מראה כיצד לשמור מסמך מרובה עמודים DOCX כתמונה PNG עם פריסת רשת:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Png);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.PageLayout = MultiPageLayout.Grid(3, 10, 10);

// Customize the background and border.
options.PageLayout.BackColor = Color.LightGray;
options.PageLayout.BorderColor = Color.Blue;
options.PageLayout.BorderWidth = 2;

doc.Save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}