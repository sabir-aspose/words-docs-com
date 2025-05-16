---
title: Работа с воден знак C#
second_title: Aspose.Words за .NET
articleTitle: Работа с воден знак
linktitle: Работа с воден знак
description: "Документ воден знак манипулация с C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /bg/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Тази тема обсъжда как да се работи програмно с воден знак, използвайки Aspose.Words. Водният знак е фоново изображение, което се показва зад текста в документ. Водният знак може да съдържа текст или изображение, представлявано от класа [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Опитайте онлайн**

Можете да опитате тази функционалност с нашата [Безплатен онлайн воден знак за документ](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Добавяне на воден знак към документ

В Microsoft Word воден знак може лесно да се вмъкне в документ с помощта на командата Вмъкване на воден знак. Aspose.Words осигурява класа [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) за добавяне или премахване на воден знак в документи. Aspose.Words осигурява [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)изброяване, дефиниращо три възможни типа водни знаци (текст, изображение и нито един), с които да се работи.

### Добавяне На Текстов Воден Знак

Следващият пример за код показва как да вмъкнете текстов воден знак в документ, като дефинирате [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/), като използвате метода [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Добавяне На Воден Знак За Изображение

Следващият пример за код показва как да вмъкнете воден знак на изображение в документ, като дефинирате [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/), като използвате метода [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Водният знак на изображението може да бъде вмъкнат като изображение, низ или поток.

Водният знак също може да бъде вмъкнат, като се използва и клас на формата. Много е лесно да вмъкнете всяка форма или изображение в горен или долен колонтитул и по този начин да създадете воден знак от всякакъв вид.

Следващият пример за код вмъква воден знак в документ Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Можете да изтеглите примерния файл на този пример от [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Премахване на воден знак от документ

Клас [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) предоставя метод за премахване, за да премахнете водния знак от документ.

Следният пример за код показва как да премахнете воден знак от документи:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Ако водните знаци се добавят с помощта на обект [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/) клас, тогава за да премахнете водния знак от документ, трябва да зададете само името на фигурата на водния знак по време на вмъкването и след това да премахнете фигурата на водния знак с зададено име.

Следващият пример за код ви показва как да зададете името на фигурата на водния знак и да я премахнете от документа:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Добавяне на воден знак в клетка на таблица

Понякога трябва да вмъкнете воден знак/изображение в клетката на таблицата и да го покажете извън таблицата, можете да използвате свойството [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). Това свойство получава или задава флаг, показващ дали фигурата се показва в таблица или извън нея. Обърнете внимание, че това свойство работи само когато оптимизирате документа за Microsoft Word 2010 г., като използвате метода [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

Следният пример за код показва как да използвате това свойство:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
