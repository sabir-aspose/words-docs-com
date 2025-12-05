---
title: Робота з водяним знаком в Java
second_title: Aspose.Words для Java
articleTitle: Робота з водяними знаками
linktitle: Робота з водяними знаками
type: docs
description: "Маніпулювання водяними знаками документа за допомогою Java."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/java/working-with-watermark/
timestamp: 2025-04-22-08-07-04
---

У цьому розділі обговорюється, як програмно працювати з водяним знаком за допомогою Aspose.Words. Водяний знак-це фонове зображення, яке відображається за текстом у документі. Водяний знак може містити текст або зображення, представлені класом [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/).

{{% alert color="primary" %}}

**Спробуйте онлайн**

Ви можете випробувати цю функцію з нашим [Безкоштовний онлайн документ водяного знака](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Додавання водяного знака до документа

Microsoft Word водяний знак можна легко вставити в документ за допомогою команди Вставити водяний знак. Aspose.Words надає клас [watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) для додавання або видалення водяних знаків у документах. Aspose.Words містить перелік [WatermarkType ](https://reference.aspose.com/words/java/com.aspose.words/watermarktype/), що визначає три можливі типи водяних знаків (текст, зображення та без водяних знаків) для роботи.

### Додати текстовий водяний знак

Наступний приклад коду показує, як вставити текстовий водяний знак у документ, визначивши [TextWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/textwatermarkoptions/) методом [SetText](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setText-java.lang.String):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddTextWatermarkWithSpecificOptions.java" >}}

### Додати водяний знак на зображення

Наступний приклад коду показує, як вставити водяний знак зображення в документ, визначивши [ImageWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/imagewatermarkoptions/) методом [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.awt.image.BufferedImage):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddImageWatermarkWithSpecificOptions.java" >}}

Водяний знак зображення може бути вставлений у вигляді зображення, рядка або потоку.

Водяний знак також можна вставити за допомогою класу shape. Дуже легко вставити будь-яку фігуру чи зображення у верхній або нижній колонтитул і таким чином створити водяний знак будь-якого типу, який можна уявити.

Наступний приклад коду вставляє водяний знак у документ Word:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-AddWatermarkToADocument-AddWatermarkToADocument.java" >}}

{{% alert color="primary" %}}

Ви можете завантажити приклад файлу цього прикладу з сайту [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Document.doc).

{{% /alert %}}


## Видалення водяного знака з документа

Клас [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) надає метод `Remove` для видалення водяного знака з документа.

Наступні приклади коду показують, як видалити водяний знак з документів:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-RemoveWatermarkFromDocument.java" >}}

Щоб видалити водяний знак з документа, вам потрібно встановити лише назву форми водяного знака під час вставки, а потім видалити форму водяного знака за допомогою призначеного імені.

У наступному прикладі коду показано, як задати назву форми водяного знака і видалити його з документа:

{{< highlight csharp >}}

// Set name to be able to remove it afterwards
watermark.Name("WaterMark");
{{< /highlight >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-RemoveWatermark-RemoveWatermark.java" >}}

## Додайте водяний знак до комірки таблиці

Іноді вам потрібно вставити водяний знак / зображення в комірку таблиці та відобразити його поза таблицею, ви можете використовувати властивість [IsLayoutInCell](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#isLayoutInCell-boolean). Ця властивість повертає або встановлює прапор, який вказує, чи відображається фігура всередині таблиці або поза нею. Зверніть увагу, що ця властивість працює лише при оптимізації документа для Microsoft Word 2010 року за допомогою методу [OptimizeFor](https://reference.aspose.com/words/java/com.aspose.words/compatibilityoptions/#optimizeFor-int).

Наступний приклад коду показує, як використовувати цю властивість:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-Shapes-WorkingWithShapes-SetShapeLayoutInCell.java" >}}
