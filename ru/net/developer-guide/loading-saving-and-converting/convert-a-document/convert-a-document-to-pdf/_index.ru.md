---
title: Конвертировать Ворд в ПДФ на C#
second_title: Aspose.Words для .NET
articleTitle: Конвертация документа в PDF
linktitle: Конвертация документа в PDF
description: "Конвертировать Word в PDF на C#. Простые примеры кода для преобразования DOCX в PDF. Поддержка всех форматов Ворд и изображений."
type: docs
weight: 10
url: /ru/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Возможность легко и надёжно конвертировать документы из одного формата в другой является ключевой особенностью Aspose.Words. PDF является одним из самых популярных форматов конвертации – это формат с фиксированным макетом, который сохраняет исходный вид документа при отображении на различных платформах. В Aspose.Words термин "рендеринг" обозначает процесс конвертации документа в формат файла, разбитый на страницы.

## Конвертировать документ Word в PDF

Конвертация из Word в PDF является достаточно сложным процессом, требующим нескольких этапов вычислений. Механизм компоновки Aspose.Words имитирует работу движка макета страниц Microsoft Word, благодаря чему выходные PDF-документы максимально похожи на то, что отображается в Microsoft Word.

С помощью Aspose.Words вы можете программно конвертировать документы Word в PDF из форматов DOC или DOCX без использования Microsoft Office. Эта статья показывает, как выполнить такую конвертацию.

{{% alert color="primary" %}}

Обратите внимание, что количество страниц в документе влияет на время конвертации.

{{% /alert %}}

### Конвертировать из Word в PDF

Конвертация документов DOC или DOCX в PDF в Aspose.Words очень проста – достаточно всего двух строк кода:

1. Загрузите документ в объект [Document](https://reference.aspose.com/words/net/aspose.words/document/), используя один из его конструкторов и указав имя документа с расширением.
1. Вызовите один из методов [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) для объекта **Document** и укажите желаемый выходной формат как PDF, введя имя файла с расширением ".PDF".

Следующий пример кода показывает, как конвертировать документ Word в PDF с помощью метода [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Файл шаблона для этого примера можно скачать из [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Иногда требуется указать дополнительные параметры, влияющие на результат сохранения документа в PDF. Эти параметры задаются с помощью класса [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), содержащего свойства, определяющие способ отображения выходного PDF-файла.

Обратите внимание, что с помощью той же техники можно конвертировать любой документ с потоковой разметкой в PDF.

{{% /alert %}}

### Конвертировать в различные стандарты PDF

Aspose.Words предоставляет перечисление [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) для поддержки конвертации DOC или DOCX в различные стандарты PDF (например, PDF 1.7, PDF 1.5 и т.д.).

Следующий пример кода показывает, как конвертировать документ в PDF 1.7 с помощью [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) с соответствием стандарту PDF 1.7:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Конвертировать изображения в PDF

Конвертация в PDF не ограничивается документами Microsoft Word. Любой формат, поддерживаемый Aspose.Words, включая программно созданные документы, также можно конвертировать в PDF. Например, можно конвертировать одностраничные изображения (JPEG, PNG, BMP, EMF, WMF) и многостраничные изображения (TIFF, GIF) в PDF.

Следующий пример кода показывает, как конвертировать изображения JPEG и TIFF в PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Чтобы этот код работал, необходимо добавить ссылки на `Aspose.Words` и `System.Drawing` в ваш проект.

## Уменьшение размера выходного PDF-файла

При сохранении в PDF можно включить оптимизацию выходного файла. Для этого установите флаг [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) в значение `true` – тогда будут удалены избыточные вложенные и пустые области рисования, а соседние глифы с одинаковым форматированием будут объединены.

Следующий пример кода показывает, как оптимизировать выходной файл:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Использование свойства **OptimizeOutput** может повлиять на точность отображения содержимого.

{{% /alert %}}

## См. также

- Статья [Рендеринг](/words/ru/net/rendering/) для получения дополнительной информации о форматах с фиксированной разметкой и потоковой разметкой
- Статья [Конвертация в формат с фиксированной разметкой](/words/net/converting-to-fixed-page-format/#what-is-a-page-layout) для получения дополнительной информации о макете страницы
- Статья [Указание параметров рендеринга при конвертации в PDF](/words/ru/net/specify-rendering-options-when-converting-to-pdf/) для получения дополнительной информации об использовании класса `PdfSaveOptions`
- Статья [Особенности конвертации в PDF/A и PDF/UA](/words/ru/net/learn-features-of-conversion-to-pdf-a-pdf-ua/), описывающая, какой стандарт PDF и соответствующие стандарты ISO для PDF поддерживает Aspose.Words
- Статья [Какой стандарт PDF лучше выбрать](/words/ru/net/which-pdf-standard-is-better-to-choose/) для определения того, какие стандарты PDF подходят для каких случаев
- Статья [Работа с PDF/A или PDF/UA](/words/ru/net/working-with-pdfa-or-pdfua/) описывает требования к содержимому документа в форматах PDF/A и PDF/UA – в основном требования к структуре и шрифтам
- Статья [Предупреждения о проблемах доступности при сохранении в PDF/A и PDF/UA](/words/ru/net/warnings-when-saving-to-pdfa-and-pdfua/) описывает требования к доступности содержимого, которые предъявляют форматы PDF/A и PDF/UA
