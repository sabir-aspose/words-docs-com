---
title: Конвертиране на документ от няколко страници в изображение в Python
second_title: Aspose.Words за Python
articleTitle: Конвертиране на документ от няколко страници в изображение
linktitle: Конвертиране на документ от няколко страници в изображение
type: docs
description: "Експортиране на документи от няколко страници към растерни изображения (JPG, PNG, GIF, BMP, TIFF, WebP) Използване на Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words за Python via .NET позволява на потребителите да експортират документи от няколко страници в растерни изображения. Това може да бъде полезно за генериране на визуализации, архиви или визуални представяния на документи, които не могат да се редактират.

## Какви формати поддържат Експорт на няколко страници?

Aspose.Words поддържа експорт на няколко страници в следните растерни формати на изображения:

* Джпег
* Гиф
* ПНГ
* БМП
* Тиф
* WebP

## Как да експортирате документ от няколко страници към изображение

Функцията за експортиране на документ от няколко страници към изображение се реализира с помощта на класа [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) - можете да зададете как да се организират страниците, когато записвате в изображение:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - запазете само първата от посочените страници
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - подредете страниците в мрежа, отляво надясно и отгоре надолу, като посочите броя на колоните
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - подредете страниците хоризонтално една до друга, отляво надясно, в един изход
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - подредете страниците вертикално една под друга в един изход
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - подредете всяка страница като отделен кадър в мулти-кадър TIFF изображение, важи само за TIFF формати на изображения

Следващият пример за код показва как да запишете документ с няколко страници DOCX като JPEG изображение с хоризонтално оформление:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Можете също да персонализирате външния вид на страницата на изходния файл – посочете [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) и [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

Следващият пример за код показва как да запишете документ с няколко страници DOCX като PNG изображение с оформление на мрежата:

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