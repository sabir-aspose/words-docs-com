---
title: Конвертиране на документ от няколко страници в изображение в C#
second_title: Aspose.Words за .NET
articleTitle: Конвертиране на документ от няколко страници в изображение
linktitle: Конвертиране на документ от няколко страници в изображение
type: docs
description: "Експортиране на документи от няколко страници към растерни изображения (JPG, PNG, GIF, BMP, TIFF, WebP) употреба C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words за .NET позволява на потребителите да експортират документи от няколко страници в растерни изображения. Това може да бъде полезно за генериране на визуализации, архиви или визуални представяния на документи, които не могат да се редактират.

## Какви формати поддържат Експорт на няколко страници?

Aspose.Words поддържа експорт на няколко страници в следните растерни формати на изображения:

* Джпег
* Гиф
* ПНГ
* БМП
* Тиф
* WebP

## Как да експортирате документ от няколко страници към изображение

Функцията за експортиране на документ от няколко страници към изображение се реализира с помощта на класа [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) - можете да зададете как да се организират страниците, когато записвате в изображение:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - запазете само първата от посочените страници
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - подредете страниците в мрежа, отляво надясно и отгоре надолу, като посочите броя на колоните
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - подредете страниците хоризонтално една до друга, отляво надясно, в един изход
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - подредете страниците вертикално една под друга в един изход
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - подредете всяка страница като отделен кадър в мулти-кадър TIFF изображение, важи само за TIFF формати на изображения

Следващият пример за код показва как да запишете документ с няколко страници DOCX като JPEG изображение с хоризонтално оформление:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Можете също да персонализирате външния вид на страницата на изходния файл – посочете [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) и [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

Следващият пример за код показва как да запишете документ с няколко страници DOCX като PNG изображение с оформление на мрежата:

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