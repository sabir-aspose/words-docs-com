---
title: Преобразуйте многостраничный документ в изображение за Java
second_title: Aspose.Words для Java
articleTitle: Преобразование многостраничного документа в изображение
linktitle: Преобразование многостраничного документа в изображение
type: docs
description: "Экспортируйте многостраничные документы в растровые изображения (JPG, PNG, GIF, BMP, TIFF, WebP) используя Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ru/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words для Java позволяет пользователям экспортировать многостраничные документы в растровые изображения. Это может быть полезно для создания предварительных просмотров, архивов или визуальных представлений документов для использования без редактирования.

## Какие форматы поддерживают многостраничный экспорт?

Aspose.Words поддерживает многостраничный экспорт в следующие форматы растровых изображений:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Как экспортировать многостраничный документ в изображение

Функция экспорта многостраничного документа в изображение реализована с помощью класса [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) - вы можете указать, как должны быть организованы страницы при сохранении в изображение:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) – сохранить только первую из указанных страниц
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) – расположите страницы в виде сетки слева направо и сверху вниз, указав количество столбцов
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) – расположите страницы горизонтально, бок о бок, слева направо, в виде единого вывода
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) – расположите страницы вертикально, одну под другой, в едином выводе
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) – оформить каждую страницу как отдельный кадр в многокадровом изображении TIFF, применимо только к форматам изображений TIFF

В следующем примере кода показано, как сохранить многостраничный DOCX документ в виде JPEG изображения с горизонтальным расположением:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Вы также можете настроить внешний вид страницы выходного файла – укажите [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) и [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

В следующем примере кода показано, как сохранить многостраничный DOCX документ в виде PNG изображения с разметкой сетки:

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