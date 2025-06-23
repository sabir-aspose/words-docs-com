---
title: Перетворіть багатосторінковий документ на зображення для Java
second_title: Aspose.Words для Java
articleTitle: Перетворення багатосторінкового документа в зображення
linktitle: Перетворення багатосторінкового документа в зображення
type: docs
description: "Експортуйте багатосторінкові документи в растрові зображення (JPG, PNG, GIF, BMP, TIFF, WebP) використовуючи Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /uk/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words для Java дозволяє користувачам експортувати багатосторінкові документи в растрові зображення. Це може бути корисно для створення попередніх переглядів, архівів або візуальних подань документів для використання без редагування.

## Які формати підтримують багатосторінковий експорт?

Aspose.Words підтримує багатосторінковий експорт у наступні формати растрових зображень:

* Формат Jpeg
* Gif
* Png-файл
* Bmp (англ .)
* Незлагода
* WebP

## Як експортувати багатосторінковий документ у зображення

Функція експорту багатосторінкового документа в зображення реалізована за допомогою класу [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) - ви можете вказати, як сторінки повинні бути організовані при збереженні в зображення:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) – зберегти тільки першу із зазначених сторінок
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) – розташуйте сторінки у вигляді сітки зліва направо і зверху вниз, вказавши кількість стовпців
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) – розташуйте сторінки горизонтально, поруч, зліва направо, як єдиний вихід
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) – розташуйте сторінки вертикально, одну під іншою, в єдиному виводі
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) – оформити кожну сторінку у вигляді окремого кадру в многокадровом зображенні TIFF, застосовно тільки до форматів зображень TIFF

Наступний приклад коду показує, як зберегти багатосторінковий DOCX документ як JPEG зображення з горизонтальним розташуванням:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Ви також можете налаштувати зовнішній вигляд сторінки вихідного файлу – вкажіть [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) та [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

Наступний приклад коду показує, як зберегти багатосторінковий DOCX документ як PNG зображення з розміткою сітки:

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