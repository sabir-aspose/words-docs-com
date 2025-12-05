---
title: Робота з водяним знаком в Python
second_title: Aspose.Words для Python via .NET
articleTitle: Робота з водяними знаками
linktitle: Робота з водяними знаками
description: "Створіть водяні знаки в документі та керуйте ними за допомогою Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

У цьому розділі обговорюється, як програмно працювати з водяними знаками за допомогою Aspose.Words. Водяний знак-це фонове зображення, яке відображається за текстом у документі. Водяний знак може містити текст або зображення, представлені класом [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Спробуйте онлайн**

Ви можете випробувати цю функцію з нашим [Безкоштовний онлайн документ водяного знака](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Як додати водяний знак до документа

Microsoft Word водяний знак можна легко вставити в документ за допомогою команди Вставити водяний знак. Aspose.Words надає клас [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) для додавання або видалення водяних знаків у документах. Aspose.Words містить перелік [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/), що визначає три можливі типи водяних знаків ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) та [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) для роботи.

### Додати текстовий водяний знак

Наступний приклад коду показує, як вставити текстовий водяний знак у документ, визначивши [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) методом [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### Додати водяний знак на зображення

Наступний приклад коду показує, як вставити водяний знак зображення в документ, визначивши [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) методом [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

Водяний знак зображення може бути вставлений у вигляді зображення, рядка або потоку.

Водяний знак також можна вставити за допомогою класу shape. Дуже легко вставити будь-яку фігуру чи зображення у верхній або нижній колонтитул і таким чином створити водяний знак будь-якого типу, який можна уявити.

Наступний приклад коду вставляє водяний знак у документ Word:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

Ви можете завантажити файл шаблону для цього прикладу з сайту [тут](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Видалення водяного знака з документа

Клас [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) надає метод видалення для видалення водяного знака з документа.

Наступний приклад коду показує, як видалити водяний знак з документів:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

Якщо водяні знаки додаються з використанням об'єкта класу [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/), то для видалення водяного знака з документа вам необхідно задати тільки назву форми водяного знака під час вставки, а потім видалити форму водяного знака за допомогою призначеного імені.

У наступному прикладі коду показано, як задати назву форми водяного знака і видалити його з документа:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## Додайте водяний знак до комірки таблиці

Іноді вам потрібно вставити водяний знак / зображення в комірку таблиці та відобразити його поза таблицею, ви можете використовувати властивість [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/). Ця властивість встановлює прапорець, який вказує, чи відображається фігура всередині таблиці або поза нею. Зверніть увагу, що ця властивість працює лише при оптимізації документа для Microsoft Word 2010 року за допомогою методу [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

Наступний приклад коду показує, як використовувати цю властивість:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
