---
title: Работа с водяным знаком в C#
second_title: Aspose.Words для .NET
articleTitle: Работа с водяными знаками
linktitle: Работа с водяными знаками
description: "Манипулирование водяными знаками документа с помощью C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ru/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

В этом разделе обсуждается, как программно работать с водяными знаками с помощью Aspose.Words. Водяной знак - это фоновое изображение, которое отображается за текстом в документе. Водяной знак может содержать текст или изображение, представленные классом [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Попробуйте онлайн**

Вы можете опробовать эту функцию с нашим [Бесплатный онлайн документ водяного знака](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Добавление водяного знака к документу

В Microsoft Word водяной знак может быть легко вставлен в документ с помощью команды Вставить водяной знак. Aspose.Words предоставляет класс [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) для добавления или удаления водяных знаков в документах. Aspose.Words содержит перечисление [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/), определяющее три возможных типа водяных знаков (текст, изображение и без водяных знаков) для работы.

### Добавить текстовый водяной знак

В следующем примере кода показано, как вставить текстовый водяной знак в документ, определив [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) с помощью метода [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Добавить водяной знак на изображение

В следующем примере кода показано, как вставить водяной знак изображения в документ, определив [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) с помощью метода [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Водяной знак изображения может быть вставлен в виде изображения, строки или потока.

Водяной знак также можно вставить с помощью класса shape. Очень легко вставить любую фигуру или изображение в верхний или нижний колонтитул и, таким образом, создать водяной знак любого мыслимого типа.

Следующий пример кода вставляет водяной знак в документ Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Вы можете скачать примерный файл этого примера с сайта [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Удаление водяного знака из документа

Класс [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) предоставляет метод remove для удаления водяного знака с документа.

В следующем примере кода показано, как удалить водяной знак с документов:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Если водяные знаки добавляются с использованием объекта класса [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/), то для удаления водяного знака из документа вам необходимо задать только название формы водяного знака во время вставки, а затем удалить форму водяного знака с помощью назначенного имени.

В следующем примере кода показано, как задать название формы водяного знака и удалить его из документа:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Добавьте водяной знак в ячейку таблицы

Иногда вам нужно вставить водяной знак/изображение в ячейку таблицы и отобразить его за пределами таблицы, вы можете использовать свойство [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). Это свойство устанавливает флажок, указывающий, отображается ли фигура внутри таблицы или за ее пределами. Обратите внимание, что это свойство работает только при оптимизации документа для Microsoft Word 2010 года с использованием метода [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

В следующем примере кода показано, как использовать это свойство:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
