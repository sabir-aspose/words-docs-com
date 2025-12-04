---
title: Преобразуйте многостраничный документ в изображение за Python
second_title: Aspose.Words для Python
articleTitle: Преобразование многостраничного документа в изображение
linktitle: Преобразование многостраничного документа в изображение
type: docs
description: "Экспортируйте многостраничные документы в растровые изображения (JPG, PNG, GIF, BMP, TIFF, WebP) используя Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ru/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words для Python via .NET позволяет пользователям экспортировать многостраничные документы в растровые изображения. Это может быть полезно для создания предварительных просмотров, архивов или визуальных представлений документов для использования без редактирования.

## Какие форматы поддерживают многостраничный экспорт?

Aspose.Words поддерживает многостраничный экспорт в следующие форматы растровых изображений:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Как экспортировать многостраничный документ в изображение

Функция экспорта многостраничного документа в изображение реализована с помощью класса [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) - вы можете указать, как должны быть организованы страницы при сохранении в изображение:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) – сохранить только первую из указанных страниц
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) – расположите страницы в виде сетки слева направо и сверху вниз, указав количество столбцов
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) – расположите страницы горизонтально, бок о бок, слева направо, в виде единого вывода
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) – расположите страницы вертикально, одну под другой, в едином выводе
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) – оформить каждую страницу в виде отдельного кадра в многокадровом изображении TIFF, применимо только к форматам изображений TIFF

В следующем примере кода показано, как сохранить многостраничный DOCX документ в виде JPEG изображения с горизонтальным расположением:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Вы также можете настроить внешний вид страницы выходного файла – укажите [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) и [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

В следующем примере кода показано, как сохранить многостраничный DOCX документ в виде PNG изображения с разметкой сетки:

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