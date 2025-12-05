---
title: العمل مع العلامة المائية في Python
second_title: Aspose.Words ل Python via .NET
articleTitle: العمل مع العلامة المائية
linktitle: العمل مع العلامة المائية
description: "إنشاء وإدارة العلامات المائية في مستند باستخدام Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ar/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

يناقش هذا الموضوع كيفية العمل برمجيا باستخدام العلامة المائية Aspose.Words. العلامة المائية هي صورة خلفية تعرض خلف النص في المستند. يمكن أن تحتوي العلامة المائية على نص أو صورة ممثلة بفئة [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**جرب عبر الإنترنت**

يمكنك تجربة هذه الوظيفة من خلال [علامة مائية مجانية للمستندات عبر الإنترنت](https://products.aspose.app/words/watermark).

{{% /alert %}}

## كيفية إضافة علامة مائية إلى مستند

في Microsoft Word، يمكن بسهولة إدراج علامة مائية في مستند باستخدام أمر إدراج علامة مائية. Aspose.Words يوفر فئة [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) لإضافة أو إزالة العلامة المائية في المستندات. Aspose.Words يوفر [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) التعداد الذي يحدد ثلاثة أنواع ممكنة من العلامات المائية ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text) و [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) و [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) للعمل معها.

### إضافة نص العلامة المائية

يوضح مثال التعليمات البرمجية التالية كيفية إدراج علامة مائية نصية في مستند بتعريف [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) باستخدام طريقة [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### إضافة صورة مائية

يوضح مثال الكود التالي كيفية إدراج علامة مائية للصورة في مستند عن طريق تحديد [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) باستخدام طريقة [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

يمكن إدراج العلامة المائية للصورة كصورة أو سلسلة أو دفق.

يمكن أيضا إدراج العلامة المائية باستخدام فئة الشكل أيضا. من السهل جدا إدراج أي شكل أو صورة في رأس أو تذييل وبالتالي إنشاء علامة مائية من أي نوع يمكن تخيله.

يقوم مثال الكود التالي بإدراج علامة مائية في مستند Word:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

يمكنك تنزيل ملف القالب لهذا المثال من [هنا](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## إزالة العلامة المائية من مستند

توفر فئة [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) طريقة الإزالة لإزالة العلامة المائية من مستند.

يوضح مثال الكود التالي كيفية إزالة علامة مائية من المستندات:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

إذا تمت إضافة العلامات المائية باستخدام كائن فئة [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/)، ثم لإزالة العلامة المائية من مستند، يجب عليك تعيين اسم شكل العلامة المائية فقط أثناء الإدراج ثم إزالة شكل العلامة المائية باسم معين.

يوضح لك مثال التعليمات البرمجية التالي كيفية تعيين اسم شكل العلامة المائية وإزالته من المستند:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## إضافة علامة مائية في خلية الجدول

في بعض الأحيان تحتاج إلى إدراج علامة مائية/صورة في خلية الجدول وعرضها خارج الجدول، يمكنك استخدام خاصية [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/). تحصل هذه الخاصية أو تحدد علامة تشير إلى ما إذا كان الشكل معروضا داخل جدول أو خارجه. لاحظ أن هذه الخاصية تعمل فقط عند تحسين المستند لـ Microsoft Word 2010 باستخدام طريقة [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

يوضح مثال التعليمات البرمجية التالية كيفية استخدام هذه الخاصية:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
