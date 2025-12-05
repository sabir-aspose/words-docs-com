---
title: Робота з водяним знаком в C#
second_title: Aspose.Words для .NET
articleTitle: Робота з водяними знаками
linktitle: Робота з водяними знаками
description: "Маніпулювання водяними знаками документа за допомогою C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

У цьому розділі обговорюється, як програмно працювати з водяними знаками за допомогою Aspose.Words. Водяний знак-це фонове зображення, яке відображається за текстом у документі. Водяний знак може містити текст або зображення, представлені класом [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Спробуйте онлайн**

Ви можете випробувати цю функцію з нашим [Безкоштовний онлайн документ водяного знака](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Додавання водяного знака до документа

Microsoft Word водяний знак можна легко вставити в документ за допомогою команди Вставити водяний знак. Aspose.Words надає клас [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) для додавання або видалення водяних знаків у документах. Aspose.Words містить перелік [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/), що визначає три можливі типи водяних знаків (текст, зображення та без водяних знаків) для роботи.

### Додати текстовий водяний знак

Наступний приклад коду показує, як вставити текстовий водяний знак у документ, визначивши [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) методом [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Додати водяний знак на зображення

Наступний приклад коду показує, як вставити водяний знак зображення в документ, визначивши [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) методом [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Водяний знак зображення може бути вставлений у вигляді зображення, рядка або потоку.

Водяний знак також можна вставити за допомогою класу shape. Дуже легко вставити будь-яку фігуру чи зображення у верхній або нижній колонтитул і таким чином створити водяний знак будь-якого типу, який можна уявити.

Наступний приклад коду вставляє водяний знак у документ Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Ви можете завантажити приклад файлу цього прикладу з сайту [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Видалення водяного знака з документа

Клас [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) надає метод видалення для видалення водяного знака з документа.

Наступний приклад коду показує, як видалити водяний знак з документів:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Якщо водяні знаки додаються з використанням об'єкта класу [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/), то для видалення водяного знака з документа вам необхідно задати тільки назву форми водяного знака під час вставки, а потім видалити форму водяного знака за допомогою призначеного імені.

У наступному прикладі коду показано, як задати назву форми водяного знака і видалити його з документа:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Додайте водяний знак до комірки таблиці

Іноді вам потрібно вставити водяний знак / зображення в комірку таблиці та відобразити його поза таблицею, ви можете використовувати властивість [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). Ця властивість встановлює прапорець, який вказує, чи відображається фігура всередині таблиці або поза нею. Зверніть увагу, що ця властивість працює лише при оптимізації документа для Microsoft Word 2010 року за допомогою методу [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

Наступний приклад коду показує, як використовувати цю властивість:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
