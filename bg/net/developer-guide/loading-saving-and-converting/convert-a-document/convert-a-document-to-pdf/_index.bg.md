---
title: Конвертиране на Word в PDF с C#
second_title: Aspose.Words за .NET
articleTitle: Преобразуване на документ в PDF
linktitle: Преобразуване на документ в PDF
description: "Конвертиране на Word в PDF с C#. Прости примери за код за преобразуване на DOCX в PDF. Поддържа всички Word формати и изображения."
type: docs
weight: 10
url: /bg/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Възможността за лесно и надеждно конвертиране на документи от един формат в друг е ключова функция на Aspose.Words. PDF е един от най-популярните формати за преобразуване – това е формат с фиксирано оформление, който запазва оригиналния вид на документа при рендиране на различни платформи. Терминът "рендиране" се използва в Aspose.Words за описание на процеса на конвертиране на документ във файлов формат, който е разделен на страници или има концепцията за страници.

## Конвертиране на Word документ в PDF

Конвертирането от Word в PDF е доста сложен процес, който изисква няколко етапа на изчисления. Механизмът за оформление на Aspose.Words имитира начина, по който работи механизмът за оформление на страници на Microsoft Word, което прави изходните PDF документи да изглеждат възможно най-близо до това, което можете да видите в Microsoft Word.

С Aspose.Words можете програмно да преобразувате документ от Word формати, като DOC или DOCX, в PDF без да използвате Microsoft Office. Тази статия обяснява как да извършите това превръщане.

{{% alert color="primary" %}}

Обърнете внимание, че броят страници в документа влияе на времето за конвертиране.

{{% /alert %}}

### Конвертиране на DOCX или DOC в PDF

Преобразуването от DOC или DOCX документен формат в PDF формат в Aspose.Words е много лесно и може да се постигне само с два реда код, които:

1. Заредете документа си в [Document](https://reference.aspose.com/words/net/aspose.words/document/) обект, използвайки един от неговите конструктори чрез указване на името на документа с неговото файлово разширение.
1. Извикайте един от [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) методите на **Document** обекта и укажете желания изходен формат като PDF, като въведете файлово име с разширение ".PDF".

Следният пример за код показва как да конвертирате документ от DOCX в PDF, използвайки [Save](https://reference.aspose.com/words/net/aspose.words/document/save/) метода:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Можете да изтеглите шаблонния файл на този пример от [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Понякога е необходимо да се специфицират допълнителни опции, които могат да повлияят на резултата от записването на документ като PDF. Тези опции могат да се специфицират чрез използването на [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) класа, съдържащ свойства, които определят как ще се показва PDF изходът.

Обърнете внимание, че със същата техника можете да превърнете всеки документ с течно оформление в PDF формат.

{{% /alert %}}

### Преобразуване в различни PDF стандарти

Aspose.Words предоставя [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) изброяване за поддържка на конвертирането на DOC или DOCX в различни PDF формат стандарти (като PDF 1.7, PDF 1.5, и т.н.).

Следният пример за код демонстрира как да конвертирате документ в PDF 1.7, използвайки [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) със съответствие с PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Преобразуване на изображения в PDF

Конвертирането в PDF не е ограничено до Microsoft Word документни формати. Всеки формат, поддържан от Aspose.Words, включително програмно създадени, също може да се превърне в PDF. Например, можем да конвертираме едностранични изображения, като JPEG, PNG, BMP, EMF, или WMF, както и многостранични изображения, като TIFF и GIF, в PDF.

Следният пример за код показва как да преобразувате JPEG и TIFF изображения в PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

За да работи този код, трябва да добавите референции към Aspose.Words и `System.Drawing` във вашия проект.

## Намаляване на размера на PDF изхода

При записване в PDF, можете да укажете дали искате да оптимизирате изхода. За да направите това, трябва да зададете [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) флага на true, и тогава излишните вложени и празни платна ще бъдат премахнати, съседните глифове с еднакво форматиране ще бъдат обединени.

Следният пример за код показва как да оптимизирате изхода:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Използването на **OptimizeOutput** свойството може да повлияе на точността на показване на съдържанието.

{{% /alert %}}

## Вижте също

- Статията [Рендиране](/words/bg/net/rendering/) за повече информация за форматите с фиксирани страници и течно оформление
- Статията [Преобразуване в формат с фиксирани страници](/words/net/converting-to-fixed-page-format/#what-is-a-page-layout) за повече информация за оформлението на страници
- Статията [Уточняване на опции за рендиране при конвертиране в PDF](/words/bg/net/specify-rendering-options-when-converting-to-pdf/) за повече информация за използването на `PdfSaveOptions` класа
- Статията [Научете особеностите на конвертирането в PDF/A и PDF/UA](/words/bg/net/learn-features-of-conversion-to-pdf-a-pdf-ua/), описваща кой PDF стандарт и съответните ISO за PDF стандарти поддържа Aspose.Words
- Статията [Кой PDF стандарт е по-добре да изберете](/words/bg/net/which-pdf-standard-is-better-to-choose/) за определяне кои PDF стандарти са подходящи за кои случаи

- Статията [Работа с PDF/A или PDF/UA](/words/bg/net/working-with-pdfa-or-pdfua/) описва изискванията за съдържанието на документа в PDF/A и PDF/UA формати – главно изискванията за структурата и шрифтовете

- Статията [Предупреждения за проблеми с достъпността при записване в PDF/A и PDF/UA](/words/bg/net/warnings-when-saving-to-pdfa-and-pdfua/) описва какви изисквания за достъпност на съдържанието налагат PDF/A и PDF/UA
