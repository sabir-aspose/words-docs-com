---
title: Перетворіть багатосторінковий документ на зображення для C#
second_title: Aspose.Words для .NET
articleTitle: Перетворення багатосторінкового документа в зображення
linktitle: Перетворення багатосторінкового документа в зображення
type: docs
description: "Експортуйте багатосторінкові документи в растрові зображення (JPG, PNG, GIF, BMP, TIFF, WebP) використовуючи C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words для .NET дозволяє користувачам експортувати багатосторінкові документи в растрові зображення. Це може бути корисно для створення попередніх переглядів, архівів або візуальних подань документів для використання без редагування.

## Які формати підтримують багатосторінковий експорт?

Aspose.Words підтримує багатосторінковий експорт у наступні формати растрових зображень:

* Формат Jpeg
* Gif
* Png-файл
* Bmp (англ .)
* Незлагода
* WebP

## Як експортувати багатосторінковий документ у зображення

Функція експорту багатосторінкового документа в зображення реалізована за допомогою класу [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) - ви можете вказати, як сторінки повинні бути організовані при збереженні в зображення:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) – зберегти тільки першу із зазначених сторінок
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) – розташуйте сторінки у вигляді сітки зліва направо і зверху вниз, вказавши кількість стовпців
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) – розташуйте сторінки горизонтально, поруч, зліва направо, як єдиний вихід
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) – розташуйте сторінки вертикально, одну під іншою, в єдиному виводі
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) – оформити кожну сторінку у вигляді окремого кадру в многокадровом зображенні TIFF, застосовно тільки до форматів зображень TIFF

Наступний приклад коду показує, як зберегти багатосторінковий DOCX документ як JPEG зображення з горизонтальним розташуванням:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Ви також можете налаштувати зовнішній вигляд сторінки вихідного файлу – вкажіть [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) та [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

Наступний приклад коду показує, як зберегти багатосторінковий DOCX документ як PNG зображення з розміткою сітки:

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