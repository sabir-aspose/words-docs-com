---
title: تحويل مستند متعدد الصفحات إلى صورة في Java
second_title: Aspose.Words ل Java
articleTitle: تحويل مستند متعدد الصفحات إلى صورة
linktitle: تحويل مستند متعدد الصفحات إلى صورة
type: docs
description: "تصدير المستندات متعددة الصفحات إلى الصور النقطية(JPG, PNG, GIF, BMP, TIFF, WebP) باستخدام Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ar/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words إلى عن على Java يسمح للمستخدمين بتصدير مستندات متعددة الصفحات إلى صور نقطية. يمكن أن يكون هذا مفيدا لإنشاء معاينات أو أرشيفات أو تمثيلات مرئية للمستندات للاستخدام غير القابل للتحرير.

## ما هي صيغ دعم تصدير متعدد الصفحات?

Aspose.Words يدعم التصدير متعدد الصفحات إلى تنسيقات الصور النقطية التالية:

* الحياة السياسية في فرنسا
* اف
* بابوا نيو غينيا
* بمب
* تيف
* WebP

## كيفية تصدير مستند متعدد الصفحات إلى صورة

يتم تنفيذ ميزة تصدير مستند متعدد الصفحات إلى صورة باستخدام فئة [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) - يمكنك تحديد كيفية تنظيم الصفحات عند الحفظ في صورة:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - احفظ أول الصفحات المحددة فقط
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - ترتيب الصفحات في شبكة ، من اليسار إلى اليمين ومن أعلى إلى أسفل ، مع تحديد عدد الأعمدة
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - ترتيب الصفحات أفقيا جنبا إلى جنب ، من اليسار إلى اليمين ، في إخراج واحد
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - ترتيب الصفحات عموديا واحدة تحت الأخرى في إخراج واحد
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - ترتيب كل صفحة كإطار منفصل في إطار متعدد TIFF صورة ، ينطبق فقط على TIFF تنسيقات الصور

يوضح مثال الكود التالي كيفية حفظ مستند متعدد الصفحات DOCX كصورة JPEG مع تخطيط أفقي:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

يمكنك أيضا تخصيص مظهر صفحة ملف الإخراج-حدد [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor) و [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) و [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

يوضح مثال الكود التالي كيفية حفظ مستند متعدد الصفحات DOCX كصورة PNG مع تخطيط الشبكة:

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