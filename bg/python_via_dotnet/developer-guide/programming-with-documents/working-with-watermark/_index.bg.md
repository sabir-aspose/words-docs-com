---
title: Работа с воден знак Python
second_title: Aspose.Words за Python via .NET
articleTitle: Работа с воден знак
linktitle: Работа с воден знак
description: "Създаване и управление на водни знаци в документ с Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Тази тема обсъжда как да се работи програмно с воден знак, използвайки Aspose.Words. Водният знак е фоново изображение, което се показва зад текста в документ. Водният знак може да съдържа текст или изображение, представлявано от класа [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Опитайте онлайн**

Можете да опитате тази функционалност с нашата [Безплатен онлайн воден знак за документ](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Как да добавите воден знак към документ

В Microsoft Word воден знак може лесно да се вмъкне в документ с помощта на командата Вмъкване на воден знак. Aspose.Words осигурява класа [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) за добавяне или премахване на воден знак в документи. Aspose.Words осигурява [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) изброяване, дефиниращо три възможни типа водни знаци ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) и [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)), с които да се работи.

### Добавяне На Текстов Воден Знак

Следващият пример за код показва как да вмъкнете текстов воден знак в документ, като дефинирате [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/), като използвате метода [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### Добавяне На Воден Знак За Изображение

Следващият пример за код показва как да вмъкнете воден знак на изображение в документ, като дефинирате [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/), като използвате метода [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

Водният знак на изображението може да бъде вмъкнат като изображение, низ или поток.

Водният знак също може да бъде вмъкнат, като се използва и клас на формата. Много е лесно да вмъкнете всяка форма или изображение в горен или долен колонтитул и по този начин да създадете воден знак от всякакъв вид.

Следващият пример за код вмъква воден знак в документ Word:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

Можете да изтеглите шаблонния файл на този пример от [ето](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Премахване на воден знак от документ

Клас [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) предоставя метод за премахване, за да премахнете водния знак от документ.

Следният пример за код показва как да премахнете воден знак от документи:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

Ако водните знаци се добавят с помощта на обект [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/) клас, тогава за да премахнете водния знак от документ, трябва да зададете само името на фигурата на водния знак по време на вмъкването и след това да премахнете фигурата на водния знак с зададено име.

Следващият пример за код ви показва как да зададете името на фигурата на водния знак и да я премахнете от документа:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## Добавяне на воден знак в клетка на таблица

Понякога трябва да вмъкнете воден знак/изображение в клетката на таблицата и да го покажете извън таблицата, можете да използвате свойството [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/). Това свойство получава или задава флаг, показващ дали фигурата се показва в таблица или извън нея. Обърнете внимание, че това свойство работи само когато оптимизирате документа за Microsoft Word 2010 г., като използвате метода [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

Следният пример за код показва как да използвате това свойство:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
