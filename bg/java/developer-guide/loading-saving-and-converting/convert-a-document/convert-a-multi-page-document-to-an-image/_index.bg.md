---
title: Конвертиране на документ от няколко страници в изображение в Java
second_title: Aspose.Words за Java
articleTitle: Конвертиране на документ от няколко страници в изображение
linktitle: Конвертиране на документ от няколко страници в изображение
type: docs
description: "Експортиране на документи от няколко страници към растерни изображения (JPG, PNG, GIF, BMP, TIFF, WebP) употреба Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words за Java позволява на потребителите да експортират документи от няколко страници в растерни изображения. Това може да бъде полезно за генериране на визуализации, архиви или визуални представяния на документи, които не могат да се редактират.

## Какви формати поддържат Експорт на няколко страници?

Aspose.Words поддържа експорт на няколко страници в следните растерни формати на изображения:

* Джпег
* Гиф
* ПНГ
* БМП
* Тиф
* WebP

## Как да експортирате документ от няколко страници към изображение

Функцията за експортиране на документ от няколко страници към изображение се реализира с помощта на класа [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) - можете да зададете как да се организират страниците, когато записвате в изображение:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - запазете само първата от посочените страници
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - подредете страниците в мрежа, отляво надясно и отгоре надолу, като посочите броя на колоните
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - подредете страниците хоризонтално една до друга, отляво надясно, в един изход
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - подредете страниците вертикално една под друга в един изход
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - подредете всяка страница като отделен кадър в мулти-кадър TIFF изображение, важи само за TIFF формати на изображения

Следващият пример за код показва как да запишете документ с няколко страници DOCX като JPEG изображение с хоризонтално оформление:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Можете също да персонализирате външния вид на страницата на изходния файл – посочете [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) и [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

Следващият пример за код показва как да запишете документ с няколко страници DOCX като PNG изображение с оформление на мрежата:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.PNG);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.setPageLayout(MultiPageLayout.grid(3, 10f, 10f));

// Customize the background and border.
options.getPageLayout().setBackColor(Color.lightGray);
options.getPageLayout().setBorderColor(Color.BLUE);
options.getPageLayout().setBorderWidth(2f);

doc.save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}