---
title: تحويل مستند متعدد الصفحات إلى صورة في C#
second_title: Aspose.Words ل .NET
articleTitle: تحويل مستند متعدد الصفحات إلى صورة
linktitle: تحويل مستند متعدد الصفحات إلى صورة
type: docs
description: "تصدير المستندات متعددة الصفحات إلى الصور النقطية(JPG, PNG, GIF, BMP, TIFF, WebP) باستخدام C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ar/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words إلى عن على .NET يسمح للمستخدمين بتصدير مستندات متعددة الصفحات إلى صور نقطية. يمكن أن يكون هذا مفيدا لإنشاء معاينات أو أرشيفات أو تمثيلات مرئية للمستندات للاستخدام غير القابل للتحرير.

## ما هي صيغ دعم تصدير متعدد الصفحات?

Aspose.Words يدعم التصدير متعدد الصفحات إلى تنسيقات الصور النقطية التالية:

* الحياة السياسية في فرنسا
* اف
* بابوا نيو غينيا
* بمب
* تيف
* WebP

## كيفية تصدير مستند متعدد الصفحات إلى صورة

يتم تنفيذ ميزة تصدير مستند متعدد الصفحات إلى صورة باستخدام فئة [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) - يمكنك تحديد كيفية تنظيم الصفحات عند الحفظ في صورة:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - احفظ أول الصفحات المحددة فقط
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - ترتيب الصفحات في شبكة ، من اليسار إلى اليمين ومن أعلى إلى أسفل ، مع تحديد عدد الأعمدة
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - ترتيب الصفحات أفقيا جنبا إلى جنب ، من اليسار إلى اليمين ، في إخراج واحد
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - ترتيب الصفحات عموديا واحدة تحت الأخرى في إخراج واحد
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - ترتيب كل صفحة كإطار منفصل في إطار متعدد TIFF صورة ، ينطبق فقط على TIFF تنسيقات الصور

يوضح مثال الكود التالي كيفية حفظ مستند متعدد الصفحات DOCX كصورة JPEG مع تخطيط أفقي:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

يمكنك أيضا تخصيص مظهر صفحة ملف الإخراج-حدد [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/) و [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) و [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

يوضح مثال الكود التالي كيفية حفظ مستند متعدد الصفحات DOCX كصورة PNG مع تخطيط الشبكة:

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