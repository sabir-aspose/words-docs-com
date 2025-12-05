---
title: Работа с воден знак Java
second_title: Aspose.Words за Java
articleTitle: Работа с воден знак
linktitle: Работа с воден знак
type: docs
description: "Документ воден знак манипулация с Java."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/java/working-with-watermark/
timestamp: 2025-04-22-08-07-04
---

Тази тема обсъжда как да се работи програмно с воден знак, използвайки Aspose.Words. Водният знак е фоново изображение, което се показва зад текста в документ. Водният знак може да съдържа текст или изображение, представлявано от класа [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/).

{{% alert color="primary" %}}

**Опитайте онлайн**

Можете да опитате тази функционалност с нашата [Безплатен онлайн воден знак за документ](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Добавяне на воден знак към документ

В Microsoft Word воден знак може лесно да се вмъкне в документ с помощта на командата Вмъкване на воден знак. Aspose.Words осигурява класа [watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) за добавяне или премахване на воден знак в документи. Aspose.Words осигурява [WatermarkType ](https://reference.aspose.com/words/java/com.aspose.words/watermarktype/)изброяване, дефиниращо три възможни типа водни знаци (текст, изображение и нито един), с които да се работи.

### Добавяне На Текстов Воден Знак

Следващият пример за код показва как да вмъкнете текстов воден знак в документ, като дефинирате [TextWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/textwatermarkoptions/), като използвате метода [SetText](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setText-java.lang.String):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddTextWatermarkWithSpecificOptions.java" >}}

### Добавяне На Воден Знак За Изображение

Следващият пример за код показва как да вмъкнете воден знак на изображение в документ, като дефинирате [ImageWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/imagewatermarkoptions/), използвайки метода [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.awt.image.BufferedImage):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddImageWatermarkWithSpecificOptions.java" >}}

Водният знак на изображението може да бъде вмъкнат като изображение, низ или поток.

Водният знак също може да бъде вмъкнат, като се използва и клас на формата. Много е лесно да вмъкнете всяка форма или изображение в горен или долен колонтитул и по този начин да създадете воден знак от всякакъв вид.

Следващият пример за код вмъква воден знак в документ Word:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-AddWatermarkToADocument-AddWatermarkToADocument.java" >}}

{{% alert color="primary" %}}

Можете да изтеглите примерния файл на този пример от [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Document.doc).

{{% /alert %}}


## Премахване на воден знак от документ

Клас [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) предоставя метод `Remove` за премахване на водния знак от документ.

Следните примери за код показват как да премахнете воден знак от документи:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-RemoveWatermarkFromDocument.java" >}}

За да премахнете водния знак от документ, трябва да зададете само името на фигурата на водния знак по време на вмъкването и след това да премахнете фигурата на водния знак с зададено име.

Следващият пример за код ви показва как да зададете името на фигурата на водния знак и да я премахнете от документа:

{{< highlight csharp >}}

// Set name to be able to remove it afterwards
watermark.Name("WaterMark");
{{< /highlight >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-RemoveWatermark-RemoveWatermark.java" >}}

## Добавяне на воден знак в клетка на таблица

Понякога трябва да вмъкнете воден знак/изображение в клетката на таблицата и да го покажете извън таблицата, можете да използвате [IsLayoutInCell](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#isLayoutInCell-boolean) свойство. Това свойство получава или задава флаг, показващ дали фигурата се показва в таблица или извън нея. Обърнете внимание, че това свойство работи само когато оптимизирате документа за Microsoft Word 2010 г., като използвате метода [OptimizeFor](https://reference.aspose.com/words/java/com.aspose.words/compatibilityoptions/#optimizeFor-int).

Следният пример за код показва как да използвате това свойство:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-Shapes-WorkingWithShapes-SetShapeLayoutInCell.java" >}}
