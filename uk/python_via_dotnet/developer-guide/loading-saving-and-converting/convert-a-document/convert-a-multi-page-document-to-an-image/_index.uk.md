---
title: Перетворіть багатосторінковий документ на зображення для Python
second_title: Aspose.Words для Python
articleTitle: Перетворення багатосторінкового документа в зображення
linktitle: Перетворення багатосторінкового документа в зображення
type: docs
description: "Експортуйте багатосторінкові документи в растрові зображення (JPG, PNG, GIF, BMP, TIFF, WebP) Використовуючи Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /uk/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words для Python via .NET дозволяє користувачам експортувати багатосторінкові документи в растрові зображення. Це може бути корисно для створення попередніх переглядів, архівів або візуальних подань документів для використання без редагування.

## Які формати підтримують багатосторінковий експорт?

Aspose.Words підтримує багатосторінковий експорт у наступні формати растрових зображень:

* Формат Jpeg
* Gif
* Png-файл
* Bmp (англ .)
* Незлагода
* WebP

## Як експортувати багатосторінковий документ у зображення

Функція експорту багатосторінкового документа в зображення реалізована за допомогою класу [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) - ви можете вказати, як сторінки повинні бути організовані при збереженні в зображення:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) – зберегти тільки першу із зазначених сторінок
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) – розташуйте сторінки у вигляді сітки зліва направо і зверху вниз, вказавши кількість стовпців
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) – розташуйте сторінки горизонтально, поруч, зліва направо, як єдиний вихід
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) – розташуйте сторінки вертикально, одну під іншою, в єдиному виводі
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) – оформити кожну сторінку у вигляді окремого кадру в многокадровом зображенні TIFF, застосовно тільки до форматів зображень TIFF

Наступний приклад коду показує, як зберегти багатосторінковий DOCX документ як JPEG зображення з горизонтальним розташуванням:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Ви також можете налаштувати зовнішній вигляд сторінки вихідного файлу – вкажіть [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) та [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

Наступний приклад коду показує, як зберегти багатосторінковий DOCX документ як PNG зображення з розміткою сітки:

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