---
title: Преобразуйте многостраничный документ в изображение за C#
second_title: Aspose.Words для .NET
articleTitle: Преобразование многостраничного документа в изображение
linktitle: Преобразование многостраничного документа в изображение
type: docs
description: "Экспортируйте многостраничные документы в растровые изображения (JPG, PNG, GIF, BMP, TIFF, WebP) используя C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ru/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words для .NET позволяет пользователям экспортировать многостраничные документы в растровые изображения. Это может быть полезно для создания предварительных просмотров, архивов или визуальных представлений документов для использования без редактирования.

## Какие форматы поддерживают многостраничный экспорт?

Aspose.Words поддерживает многостраничный экспорт в следующие форматы растровых изображений:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Как экспортировать многостраничный документ в изображение

Функция экспорта многостраничного документа в изображение реализована с помощью класса [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) - вы можете указать, как должны быть организованы страницы при сохранении в изображение:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) – сохранить только первую из указанных страниц
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) – расположите страницы в виде сетки слева направо и сверху вниз, указав количество столбцов
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) – расположите страницы горизонтально, бок о бок, слева направо, в виде единого вывода
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) – расположите страницы вертикально, одну под другой, в одном выводе
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) – оформить каждую страницу как отдельный кадр в многокадровом изображении TIFF, применимо только к форматам изображений TIFF

В следующем примере кода показано, как сохранить многостраничный DOCX документ в виде JPEG изображения с горизонтальным расположением:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Вы также можете настроить внешний вид страницы выходного файла – укажите [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) и [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

В следующем примере кода показано, как сохранить многостраничный DOCX документ в виде PNG изображения с разметкой сетки:

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