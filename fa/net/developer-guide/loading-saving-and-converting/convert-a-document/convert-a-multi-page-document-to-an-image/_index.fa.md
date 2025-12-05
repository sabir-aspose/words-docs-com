---
title: تبدیل یک سند چند صفحه ای به یک تصویر در C#
second_title: Aspose.Words برای .NET
articleTitle: تبدیل یک سند چند صفحه ای به یک تصویر
linktitle: تبدیل یک سند چند صفحه ای به یک تصویر
type: docs
description: "صادرات اسناد چند صفحه ای به تصاویر رستر(JPG, PNG, GIF, BMP, TIFF, WebP) با استفاده از C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fa/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words برای .NET به کاربران اجازه می دهد تا اسناد چند صفحه ای را به تصاویر رستر صادر کنند. این می تواند برای تولید پیش نمایش ، آرشیو یا نمایش بصری اسناد برای استفاده غیر قابل ویرایش مفید باشد.

## چه فرمت هایی از صادرات چند صفحه ای پشتیبانی می کنند ؟ 

Aspose.Words از صادرات چند صفحه ای به فرمت های تصویر رستر زیر پشتیبانی می کند:

* Jpeg
* Gif
* Png
* بی ام پی
* Tiff
* WebP

## چگونه یک سند چند صفحه ای را به یک تصویر صادر کنیم

ویژگی صادرات یک سند چند صفحه ای به یک تصویر با استفاده از کلاس [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) اجرا می شود-شما می توانید مشخص کنید که چگونه صفحات باید هنگام ذخیره به یک تصویر سازماندهی شوند:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) – فقط اولین صفحه مشخص شده را ذخیره کنید
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) – صفحات را در یک شبکه ، از چپ به راست و از بالا به پایین مرتب کنید ، در حالی که تعداد ستون ها را مشخص می کنید
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) – صفحات را به صورت افقی در کنار هم ، از چپ به راست ، در یک خروجی واحد مرتب کنید
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) – صفحات را به صورت عمودی یکی زیر دیگری در یک خروجی واحد مرتب کنید
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) – هر صفحه را به عنوان یک فریم جداگانه در یک تصویر چند فریم TIFF مرتب کنید ، فقط برای فرمت های تصویر TIFF اعمال می شود

مثال کد زیر نشان می دهد که چگونه یک سند چند صفحه ای DOCX را به عنوان JPEG تصویر با طرح افقی ذخیره کنیم:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

همچنین می توانید ظاهر صفحه فایل خروجی را سفارشی کنید – [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/) ، [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) و [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/) را مشخص کنید.

مثال کد زیر نشان می دهد که چگونه یک سند چند صفحه ای DOCX را به عنوان PNG تصویر با طرح شبکه ذخیره کنیم:

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