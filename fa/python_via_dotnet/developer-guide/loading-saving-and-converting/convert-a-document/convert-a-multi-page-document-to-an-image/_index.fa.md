---
title: تبدیل یک سند چند صفحه ای به یک تصویر در Python
second_title: Aspose.Words برای Python
articleTitle: تبدیل یک سند چند صفحه ای به یک تصویر
linktitle: تبدیل یک سند چند صفحه ای به یک تصویر
type: docs
description: "صادرات اسناد چند صفحه ای به تصاویر رستر(JPG, PNG, GIF, BMP, TIFF, WebP) با استفاده از Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fa/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words برای Python via .NET به کاربران اجازه می دهد تا اسناد چند صفحه ای را به تصاویر رستر صادر کنند. این می تواند برای تولید پیش نمایش ، آرشیو یا نمایش بصری اسناد برای استفاده غیر قابل ویرایش مفید باشد.

## چه فرمت هایی از صادرات چند صفحه ای پشتیبانی می کنند ؟ 

Aspose.Words از صادرات چند صفحه ای به فرمت های تصویر رستر زیر پشتیبانی می کند:

* Jpeg
* Gif
* Png
* بی ام پی
* Tiff
* WebP

## چگونه یک سند چند صفحه ای را به یک تصویر صادر کنیم

ویژگی صادرات یک سند چند صفحه ای به یک تصویر با استفاده از کلاس [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) اجرا می شود-شما می توانید مشخص کنید که چگونه صفحات باید هنگام ذخیره به یک تصویر سازماندهی شوند:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) – فقط اولین صفحه مشخص شده را ذخیره کنید
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) – صفحات را در یک شبکه ، از چپ به راست و از بالا به پایین مرتب کنید ، در حالی که تعداد ستون ها را مشخص می کنید
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) – صفحات را به صورت افقی در کنار هم ، از چپ به راست ، در یک خروجی واحد مرتب کنید
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) – صفحات را به صورت عمودی یکی زیر دیگری در یک خروجی واحد مرتب کنید
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) – هر صفحه را به عنوان یک فریم جداگانه در یک تصویر چند فریم TIFF مرتب کنید ، فقط برای فرمت های تصویر TIFF اعمال می شود

مثال کد زیر نشان می دهد که چگونه یک سند چند صفحه ای DOCX را به عنوان JPEG تصویر با طرح افقی ذخیره کنیم:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

همچنین می توانید ظاهر صفحه فایل خروجی را سفارشی کنید – [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/) ، [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) و [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/) را مشخص کنید.

مثال کد زیر نشان می دهد که چگونه یک سند چند صفحه ای DOCX را به عنوان PNG تصویر با طرح شبکه ذخیره کنیم:

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