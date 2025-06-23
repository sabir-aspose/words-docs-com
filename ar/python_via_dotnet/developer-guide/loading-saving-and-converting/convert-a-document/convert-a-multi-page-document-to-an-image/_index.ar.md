---
title: تحويل مستند متعدد الصفحات إلى صورة في Python
second_title: Aspose.Words ل Python
articleTitle: تحويل مستند متعدد الصفحات إلى صورة
linktitle: تحويل مستند متعدد الصفحات إلى صورة
type: docs
description: "تصدير المستندات متعددة الصفحات إلى الصور النقطية(JPG, PNG, GIF, BMP, TIFF, WebP) باستخدام Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ar/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words إلى عن على Python via .NET يسمح للمستخدمين بتصدير مستندات متعددة الصفحات إلى صور نقطية. يمكن أن يكون هذا مفيدا لإنشاء معاينات أو أرشيفات أو تمثيلات مرئية للمستندات للاستخدام غير القابل للتحرير.

## ما هي صيغ دعم تصدير متعدد الصفحات?

Aspose.Words يدعم التصدير متعدد الصفحات إلى تنسيقات الصور النقطية التالية:

* الحياة السياسية في فرنسا
* اف
* بابوا نيو غينيا
* بمب
* تيف
* WebP

## كيفية تصدير مستند متعدد الصفحات إلى صورة

يتم تنفيذ ميزة تصدير مستند متعدد الصفحات إلى صورة باستخدام فئة [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) - يمكنك تحديد كيفية تنظيم الصفحات عند الحفظ في صورة:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - احفظ أول الصفحات المحددة فقط
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - ترتيب الصفحات في شبكة ، من اليسار إلى اليمين ومن أعلى إلى أسفل ، مع تحديد عدد الأعمدة
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - ترتيب الصفحات أفقيا جنبا إلى جنب ، من اليسار إلى اليمين ، في إخراج واحد
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - ترتيب الصفحات عموديا واحدة تحت الأخرى في إخراج واحد
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - ترتيب كل صفحة كإطار منفصل في إطار متعدد TIFF صورة ، ينطبق فقط على TIFF تنسيقات الصور

يوضح مثال الكود التالي كيفية حفظ مستند متعدد الصفحات DOCX كصورة JPEG مع تخطيط أفقي:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

يمكنك أيضا تخصيص مظهر صفحة ملف الإخراج-حدد [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/) و [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) و [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

يوضح مثال الكود التالي كيفية حفظ مستند متعدد الصفحات DOCX كصورة PNG مع تخطيط الشبكة:

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