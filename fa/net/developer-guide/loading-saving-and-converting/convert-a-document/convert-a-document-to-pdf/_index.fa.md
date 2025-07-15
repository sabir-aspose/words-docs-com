---
title: تبدیل ورد به پی دی اف در C#
second_title: Aspose.Words برای .NET
articleTitle: تغییر سند به PDF
linktitle: تغییر سند به PDF
description: "تبدیل ورد به پی دی اف در C#. نمونه کدهای ساده برای تبدیل DOCX به PDF. پشتیبانی از تمام فرمت‌های ورد و تصاویر."
type: docs
weight: 10
url: /fa/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

قابلیت تبدیل آسان و قابل اعتماد اسناد از یک فرمت به فرمت دیگر یکی از ویژگی‌های کلیدی Aspose.Words است. PDF یکی از محبوب‌ترین فرمت‌ها برای تغییر است – این فرمتی با چیدمان ثابت است که ظاهر اصلی سند را هنگام رندر کردن در پلتفرم‌های مختلف حفظ می‌کند. اصطلاح "رندرینگ" در Aspose.Words برای توصیف فرآیند تبدیل یک سند به فرمت فایلی که صفحه‌بندی شده یا مفهوم صفحات را دارد، استفاده می‌شود.

## تبدیل سند ورد به PDF

تبدیل از ورد به PDF فرآیند نسبتاً پیچیده‌ای است که به چندین مرحله محاسبه نیاز دارد. موتور چیدمان Aspose.Words نحوه کار موتور چیدمان صفحه Microsoft Word را تقلید می‌کند و باعث می‌شود اسناد PDF خروجی تا حد امکان شبیه به آنچه در Microsoft Word می‌بینید باشند.

با Aspose.Words می‌توانید به صورت برنامه‌ای سندی را از فرمت‌های ورد مانند DOC یا DOCX به PDF تغییر دهید بدون استفاده از Microsoft Office. این مقاله نحوه انجام این تحویل را توضیح می‌دهد.

{{% alert color="primary" %}}

توجه داشته باشید که تعداد صفحات در سند بر زمان تبدیل تأثیر می‌گذارد.

{{% /alert %}}

### تبدیل DOCX یا DOC به PDF

تغییر از فرمت سند DOC یا DOCX به فرمت PDF در Aspose.Words بسیار آسان است و تنها با دو خط کد قابل دستیابی است:

1. سند خود را در یک شیء [Document](https://reference.aspose.com/words/net/aspose.words/document/) با استفاده از یکی از سازنده‌هایش با مشخص کردن نام سند به همراه پسوند فرمتش بارگذاری کنید.
1. یکی از متدهای [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) را روی شیء **Document** فراخوانی کنید و فرمت خروجی مورد نظر را به عنوان PDF با وارد کردن نام فایل با پسوند ".PDF" مشخص کنید.

نمونه کد زیر نحوه تبدیل سند از DOCX به PDF با استفاده از متد [Save](https://reference.aspose.com/words/net/aspose.words/document/save/) را نشان می‌دهد:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

می‌توانید فایل الگوی این مثال را از [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx) دانلود کنید.

{{% alert color="primary" %}}

گاهی اوقات لازم است گزینه‌های اضافی مشخص کنید که می‌تواند بر نتیجه ذخیره سند به عنوان PDF تأثیر بگذارد. این گزینه‌ها می‌توانند با استفاده از کلاس [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) که حاوی ویژگی‌هایی است که تعیین می‌کند خروجی PDF چگونه نمایش داده شود، مشخص شوند.

توجه داشته باشید که با همین تکنیک می‌توانید هر سند با فرمت جریان-چیدمان را به فرمت PDF تحویل دهید.

{{% /alert %}}

### تبدیل به استانداردهای مختلف PDF

Aspose.Words شمارش [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) را برای پشتیبانی از تغییر DOC یا DOCX به استانداردهای مختلف فرمت PDF (مانند PDF 1.7، PDF 1.5 و غیره) ارائه می‌دهد.

نمونه کد زیر نحوه تبدیل سند به PDF 1.7 با استفاده از [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) با انطباق با PDF17 را نشان می‌دهد:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## تبدیل تصاویر به PDF

تبدیل به PDF محدود به فرمت‌های سند Microsoft Word نیست. هر فرمتی که توسط Aspose.Words پشتیبانی می‌شود، از جمله موارد ایجاد شده به صورت برنامه‌ای، همچنین می‌تواند به PDF تحویل شود. به عنوان مثال، می‌توانیم تصاویر تک صفحه‌ای مانند JPEG، PNG، BMP، EMF یا WMF و همچنین عکس‌های چند صفحه‌ای مانند TIFF و GIF را به PDF تبدیل کنیم.

نمونه کد زیر نحوه تغییر تصاویر JPEG و TIFF به PDF را نشان می‌دهد:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

برای کارکرد این کد، نیاز دارید مراجع به Aspose.Words و `System.Drawing` را به پروژه‌تان اضافه کنید.

## کاهش اندازه خروجی PDF

هنگام ذخیره به PDF، می‌توانید مشخص کنید که آیا می‌خواهید خروجی را بهینه کنید یا نه. برای انجام این کار، باید پرچم [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) را روی true تنظیم کنید، و سپس بوم‌های تودرتو اضافی و خالی حذف می‌شوند، گلیف‌های مجاور با همان قالب‌بندی به هم متصل می‌شوند.

نمونه کد زیر نحوه بهینه‌سازی خروجی را نشان می‌دهد:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

استفاده از ویژگی **OptimizeOutput** ممکن است بر دقت نمایش محتوا تأثیر بگذارد.

{{% /alert %}}

## همچنین ببینید

- مقاله [رندرینگ](/words/fa/net/rendering/) برای اطلاعات بیشتر در مورد فرمت‌های صفحه ثابت و جریان-چیدمان
- مقاله [تبدیل به فرمت صفحه ثابت](/words/net/converting-to-fixed-page-format/#what-is-a-page-layout) برای اطلاعات بیشتر در مورد چیدمان صفحه
- مقاله [مشخص کردن گزینه‌های رندرینگ هنگام تغییر به PDF](/words/fa/net/specify-rendering-options-when-converting-to-pdf/) برای اطلاعات بیشتر در مورد استفاده از کلاس `PdfSaveOptions`
- مقاله [آشنایی با ویژگی‌های تبدیل به PDF/A و PDF/UA](/words/fa/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) که توضیح می‌دهد کدام استاندارد PDF و ISO های مربوط به استانداردهای PDF توسط Aspose.Words پشتیبانی می‌شود
- مقاله [کدام استاندارد PDF بهتر است انتخاب کنید](/words/fa/net/which-pdf-standard-is-better-to-choose/) برای تعیین اینکه کدام استانداردهای PDF برای کدام موارد مناسب هستند

- مقاله [کار با PDF/A یا PDF/UA](/words/fa/net/working-with-pdfa-or-pdfua/) الزامات محتوای سند در فرمت‌های PDF/A و PDF/UA را توصیف می‌کند – عمدتاً الزامات ساختار و فونت‌ها

- مقاله [هشدارهای مسائل دسترسی هنگام ذخیره در PDF/A و PDF/UA](/words/fa/net/warnings-when-saving-to-pdfa-and-pdfua/) توضیح می‌دهد که PDF/A و PDF/UA چه الزاماتی برای دسترسی محتوا وضع می‌کنند
