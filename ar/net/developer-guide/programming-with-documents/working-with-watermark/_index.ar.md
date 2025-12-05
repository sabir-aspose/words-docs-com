---
title: العمل مع العلامة المائية في C#
second_title: Aspose.Words ل .NET
articleTitle: العمل مع العلامة المائية
linktitle: العمل مع العلامة المائية
description: "وثيقة التلاعب العلامة المائية باستخدام C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ar/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

يناقش هذا الموضوع كيفية العمل برمجيا باستخدام العلامة المائية Aspose.Words. العلامة المائية هي صورة خلفية تعرض خلف النص في المستند. يمكن أن تحتوي العلامة المائية على نص أو صورة ممثلة بفئة [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**جرب عبر الإنترنت**

يمكنك تجربة هذه الوظيفة من خلال [علامة مائية مجانية للمستندات عبر الإنترنت](https://products.aspose.app/words/watermark).

{{% /alert %}}

## أضف علامة مائية إلى مستند

في Microsoft Word، يمكن بسهولة إدراج علامة مائية في مستند باستخدام أمر إدراج علامة مائية. Aspose.Words يوفر فئة [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) لإضافة أو إزالة العلامة المائية في المستندات. Aspose.Words يوفر [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)التعداد الذي يحدد ثلاثة أنواع ممكنة من العلامات المائية (نص وصورة ولا شيء) للعمل معها.

### إضافة نص العلامة المائية

يوضح مثال التعليمات البرمجية التالية كيفية إدراج علامة مائية نصية في مستند بتعريف [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) باستخدام طريقة [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### إضافة صورة مائية

يوضح مثال الكود التالي كيفية إدراج علامة مائية للصورة في مستند عن طريق تحديد [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) باستخدام طريقة [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

يمكن إدراج العلامة المائية للصورة كصورة أو سلسلة أو دفق.

يمكن أيضا إدراج العلامة المائية باستخدام فئة الشكل أيضا. من السهل جدا إدراج أي شكل أو صورة في رأس أو تذييل وبالتالي إنشاء علامة مائية من أي نوع يمكن تخيله.

يقوم مثال الكود التالي بإدراج علامة مائية في مستند Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

يمكنك تنزيل نموذج ملف هذا المثال من [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## إزالة العلامة المائية من مستند

توفر فئة [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) طريقة الإزالة لإزالة العلامة المائية من مستند.

يوضح مثال الكود التالي كيفية إزالة علامة مائية من المستندات:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

إذا تمت إضافة العلامات المائية باستخدام كائن فئة [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/)، ثم لإزالة العلامة المائية من مستند، يجب عليك تعيين اسم شكل العلامة المائية فقط أثناء الإدراج ثم إزالة شكل العلامة المائية باسم معين.

يوضح لك مثال التعليمات البرمجية التالي كيفية تعيين اسم شكل العلامة المائية وإزالته من المستند:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## أضف علامة مائية إلى خلية جدول

في بعض الأحيان تحتاج إلى إدراج علامة مائية/صورة في خلية الجدول وعرضها خارج الجدول، يمكنك استخدام خاصية [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). تحصل هذه الخاصية أو تحدد علامة تشير إلى ما إذا كان الشكل معروضا داخل جدول أو خارجه. لاحظ أن هذه الخاصية تعمل فقط عند تحسين المستند لـ Microsoft Word 2010 باستخدام طريقة [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

يوضح مثال التعليمات البرمجية التالية كيفية استخدام هذه الخاصية:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
