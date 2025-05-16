---
title: کار با واترمارک در C#
second_title: Aspose.Words برای .NET
articleTitle: کار با واترمارک
linktitle: کار با واترمارک
description: "دستکاری علامت آبی سند با استفاده از C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /fa/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

این موضوع در مورد چگونگی کار برنامه نویسی با watermark با استفاده از Aspose.Words بحث می کند. علامت آبی یک تصویر پس زمینه است که در پشت متن در یک سند نمایش داده می شود. یک علامت آبی می تواند حاوی یک متن یا یک تصویر باشد که توسط کلاس [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) نشان داده شده است.

{{% alert color="primary" %}}

**سعی کنید آنلاین**

شما می توانید این قابلیت را با ما امتحان کنید [علامت آبی سند آنلاین رایگان](https://products.aspose.app/words/watermark).

{{% /alert %}}

## یک علامت آبی به یک سند اضافه کنید

در Microsoft Word، یک علامت آبی را می توان به راحتی در یک سند با استفاده از دستور Insert Watermark وارد کرد. Aspose.Words کلاس [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) را برای اضافه کردن یا حذف علامت آبی در اسناد فراهم می کند. Aspose.Words شمارش [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)را فراهم می کند که سه نوع ممکن از علامت های آبی (متن، تصویر و هیچ) را برای کار با آن تعریف می کند.

### اضافه کردن علامت آبی متن

مثال کد زیر نشان می دهد که چگونه یک علامت آبی متن را در یک سند با تعریف [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) با استفاده از روش [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext) وارد کنید:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### علامت آب تصویر را اضافه کنید

مثال کد زیر نشان می دهد که چگونه یک علامت آبی تصویر را در یک سند با تعریف [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) با استفاده از روش [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage) وارد کنید:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

علامت آبی تصویر را می توان به عنوان تصویر، رشته یا جریان وارد کرد.

علامت آبی را می توان با استفاده از کلاس شکل نیز وارد کرد. بسیار آسان است که هر شکل یا تصویر را در یک سر یا پای صفحه قرار دهید و بنابراین یک علامت آبی از هر نوع قابل تصور ایجاد کنید.

مثال کد زیر یک علامت آبی را در یک سند Word قرار می دهد:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

شما می توانید فایل نمونه این مثال را از [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## علامت آب را از یک سند حذف کنید

کلاس [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) روش حذف را برای حذف علامت آبی از یک سند فراهم می کند.

مثال کد زیر نشان می دهد که چگونه یک علامت آبی را از اسناد حذف کنیم:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

اگر علامت های آبی با استفاده از شیء کلاس [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/) اضافه شوند، برای حذف علامت آبی از یک سند باید فقط نام شکل علامت آبی را در هنگام قرار دادن تنظیم کنید و سپس شکل علامت آبی را با یک نام اختصاص داده شده حذف کنید.

مثال کد زیر به شما نشان می دهد که چگونه نام شکل علامت آبی را تنظیم کنید و آن را از سند حذف کنید:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## یک علامت آبی به یک سلول میز اضافه کنید

گاهی اوقات شما باید یک علامت/تصویر را در سلول جدول قرار دهید و آن را در خارج از جدول نمایش دهید، می توانید از ویژگی [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/) استفاده کنید. این ویژگی یک پرچم را دریافت یا تنظیم می کند که نشان می دهد آیا شکل در داخل یک جدول یا خارج از آن نمایش داده می شود. توجه داشته باشید که این ویژگی تنها زمانی کار می کند که شما سند را برای Microsoft Word 2010 با استفاده از روش [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/) بهینه سازی کنید.

مثال کد زیر نشان می دهد که چگونه از این ویژگی استفاده کنید:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
