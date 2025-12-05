---
title: کار با واترمارک در Python
second_title: Aspose.Words برای Python via .NET
articleTitle: کار با واترمارک
linktitle: کار با واترمارک
description: "ایجاد و مدیریت علامت های آبی در یک سند با استفاده از Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fa/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

این موضوع در مورد چگونگی کار برنامه نویسی با watermark با استفاده از Aspose.Words بحث می کند. علامت آبی یک تصویر پس زمینه است که در پشت متن در یک سند نمایش داده می شود. یک علامت آبی می تواند حاوی یک متن یا یک تصویر باشد که توسط کلاس [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) نشان داده شده است.

{{% alert color="primary" %}}

**سعی کنید آنلاین**

شما می توانید این قابلیت را با ما امتحان کنید [علامت آبی سند آنلاین رایگان](https://products.aspose.app/words/watermark).

{{% /alert %}}

## چگونه یک علامت آبی به یک سند اضافه کنیم

در Microsoft Word، یک علامت آبی را می توان به راحتی در یک سند با استفاده از دستور Insert Watermark وارد کرد. Aspose.Words کلاس [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) را برای اضافه کردن یا حذف علامت آبی در اسناد فراهم می کند. Aspose.Words شمارش [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) را فراهم می کند که سه نوع ممکن از علامت های آبی ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text)، [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) و [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) را برای کار با آن تعریف می کند.

### اضافه کردن علامت آبی متن

مثال کد زیر نشان می دهد که چگونه یک علامت آبی متن را در یک سند با تعریف [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) با استفاده از روش [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/) وارد کنید:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### علامت آب تصویر را اضافه کنید

مثال کد زیر نشان می دهد که چگونه یک علامت آبی تصویر را در یک سند با تعریف [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) با استفاده از روش [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/) وارد کنید:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

علامت آبی تصویر را می توان به عنوان تصویر، رشته یا جریان وارد کرد.

علامت آبی را می توان با استفاده از کلاس شکل نیز وارد کرد. بسیار آسان است که هر شکل یا تصویر را در یک سر یا پای صفحه قرار دهید و بنابراین یک علامت آبی از هر نوع قابل تصور ایجاد کنید.

مثال کد زیر یک علامت آبی را در یک سند Word قرار می دهد:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

شما می توانید فایل قالب این مثال را از [اینجا](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## علامت آب را از یک سند حذف کنید

کلاس [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) روش حذف را برای حذف علامت آبی از یک سند فراهم می کند.

مثال کد زیر نشان می دهد که چگونه یک علامت آبی را از اسناد حذف کنیم:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

اگر علامت های آبی با استفاده از شیء کلاس [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/) اضافه شوند، برای حذف علامت آبی از یک سند باید فقط نام شکل علامت آبی را در هنگام قرار دادن تنظیم کنید و سپس شکل علامت آبی را با یک نام اختصاص داده شده حذف کنید.

مثال کد زیر به شما نشان می دهد که چگونه نام شکل علامت آبی را تنظیم کنید و آن را از سند حذف کنید:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## یک علامت آبی در سلول جدول اضافه کنید

گاهی اوقات شما باید یک علامت/تصویر را در سلول جدول قرار دهید و آن را در خارج از جدول نمایش دهید، می توانید از ویژگی [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/) استفاده کنید. این ویژگی یک پرچم را دریافت یا تنظیم می کند که نشان می دهد آیا شکل در داخل یک جدول یا خارج از آن نمایش داده می شود. توجه داشته باشید که این ویژگی تنها زمانی کار می کند که شما سند را برای Microsoft Word 2010 با استفاده از روش [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/) بهینه سازی کنید.

مثال کد زیر نشان می دهد که چگونه از این ویژگی استفاده کنید:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
