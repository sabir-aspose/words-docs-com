---
title: تحويل ورد الى بي دي اف في C#
second_title: Aspose.Words لـ .NET
articleTitle: تحويل مستند الى بي دي اف
linktitle: تحويل مستند الى بي دي اف
description: "تحويل ورد الى بي دي اف في C#. أمثلة كود بسيطة لتحويل DOCX الى PDF. يدعم جميع صيغ ورد والصور."
type: docs
weight: 10
url: /ar/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

إن القدرة على تحويل المستندات بسهولة وموثوقية من صيغة إلى أخرى هي ميزة رئيسية في Aspose.Words. يُعتبر بي دي اف أحد أشهر صيغ التحويل – وهو صيغة ذات تخطيط ثابت تحافظ على المظهر الأصلي للمستند عند عرضه على منصات مختلفة. يُستخدم مصطلح "العرض" في Aspose.Words لوصف عملية تحويل مستند إلى صيغة ملف مقسمة إلى صفحات أو لها مفهوم الصفحات.

## تحويل مستند ورد الى بي دي اف

تحويل ورد الى بي دي اف عملية معقدة إلى حد ما تتطلب عدة مراحل من الحسابات. يحاكي محرك التخطيط في Aspose.Words طريقة عمل محرك تخطيط الصفحات في Microsoft Word، مما يجعل مستندات بي دي اف الناتجة تبدو قريبة قدر الإمكان مما يمكنك رؤيته في Microsoft Word.

باستخدام Aspose.Words يمكنك برمجياً تحويل مستند من صيغ ورد، مثل DOC أو DOCX، إلى بي دي اف دون استخدام Microsoft Office. تشرح هذه المقالة كيفية تنفيذ هذا التحويل.

{{% alert color="primary" %}}

لاحظ أن عدد الصفحات في المستند يؤثر على وقت التحويل.

{{% /alert %}}

### تحويل DOCX أو DOC الى بي دي اف

تحويل مستندات DOC أو DOCX إلى صيغة بي دي اف في Aspose.Words سهل جداً ويمكن تحقيقه بسطرين فقط من الكود:

1. قم بتحميل مستندك إلى كائن [Document](https://reference.aspose.com/words/net/aspose.words/document/) باستخدام أحد منشئيه مع تحديد اسم المستند مع امتداد الصيغة.
1. استدعِ إحدى طرق [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) على كائن **Document** وحدد الصيغة المطلوبة كـ بي دي اف عن طريق إدخال اسم ملف بامتداد ".PDF".

يوضح المثال التالي كيفية تحويل مستند من DOCX إلى بي دي اف باستخدام طريقة [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

يمكنك تحميل ملف القالب لهذا المثال من [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

أحياناً يكون من الضروري تحديد خيارات إضافية يمكن أن تؤثر على نتيجة حفظ مستند كـ بي دي اف. يمكن تحديد هذه الخيارات باستخدام فئة [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) التي تحتوي على خصائص تحدد كيفية عرض مخرجات بي دي اف.

لاحظ أنه بنفس التقنية يمكنك تحويل أي مستند ذو تخطيط متدفق إلى صيغة بي دي اف.

{{% /alert %}}

### تحويل الى معايير بي دي اف مختلفة

يوفر Aspose.Words تعداد [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) لدعم تحويل DOC أو DOCX إلى معايير صيغة بي دي اف مختلفة (مثل PDF 1.7، PDF 1.5، إلخ).

يوضح المثال التالي كيفية تحويل مستند إلى PDF 1.7 باستخدام [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) مع الامتثال لـ PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## تحويل الصور الى بي دي اف

التحويل إلى بي دي اف لا يقتصر على صيغ مستندات Microsoft Word. أي صيغة مدعومة بواسطة Aspose.Words، بما في ذلك المنشأة برمجياً، يمكن أيضاً تحويلها إلى بي دي اف. على سبيل المثال، يمكننا تحويل الصور أحادية الصفحة، مثل جيه بي جي وبي إن جي وبي إم بي وإي إم إف أو دبليو إم إف، وكذلك الصور متعددة الصفحات، مثل تيف وجيف، إلى بي دي اف.

يوضح المثال التالي كيفية تحويل صور جيه بي جي وتيف إلى بي دي اف:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

لجعل هذا الكود يعمل، تحتاج إلى إضافة مراجع لـ Aspose.Words و `System.Drawing` إلى مشروعك.

## تقليل حجم مخرجات بي دي اف

عند الحفظ إلى بي دي اف، يمكنك تحديد ما إذا كنت تريد تحسين المخرجات. للقيام بذلك، تحتاج إلى تعيين علامة [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) إلى true، وبعد ذلك ستتم إزالة اللوحات المتداخلة الزائدة والفارغة، وسيتم دمج الرموز المجاورة بنفس التنسيق.

يوضح المثال التالي كيفية تحسين المخرجات:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

استخدام خاصية **OptimizeOutput** قد يؤثر على دقة عرض المحتوى.

{{% /alert %}}

## انظر أيضاً

- المقالة [العرض](/words/ar/net/rendering/) لمزيد من المعلومات حول صيغ الصفحة الثابتة والتخطيط المتدفق
- المقالة [التحويل إلى صيغة الصفحة الثابتة](/words/ar/net/converting-to-fixed-page-format/#what-is-a-page-layout) لمزيد من المعلومات حول تخطيط الصفحة
- المقالة [تحديد خيارات العرض عند التحويل إلى بي دي اف](/words/ar/net/specify-rendering-options-when-converting-to-pdf/) لمزيد من المعلومات حول استخدام فئة `PdfSaveOptions`
- المقالة [تعلم ميزات التحويل إلى PDF/A و PDF/UA](/words/ar/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) التي تصف معيار بي دي اف المدعوم ومعايير ISO ذات الصلة لمعايير بي دي اف التي يدعمها Aspose.Words
- المقالة [أي معيار بي دي اف الأفضل للاختيار](/words/ar/net/which-pdf-standard-is-better-to-choose/) لتحديد معايير بي دي اف التي تناسب الحالات المختلفة

- المقالة [العمل مع PDF/A أو PDF/UA](/words/ar/net/working-with-pdfa-or-pdfua/) تصف متطلبات محتوى المستند في صيغتي PDF/A و PDF/UA – بشكل أساسي متطلبات البنية والخطوط

- المقالة [تحذيرات مشاكل إمكانية الوصول عند الحفظ إلى PDF/A و PDF/UA](/words/ar/net/warnings-when-saving-to-pdfa-and-pdfua/) تصف متطلبات إمكانية الوصول للمحتوى التي تفرضها صيغتا PDF/A و PDF/UA
