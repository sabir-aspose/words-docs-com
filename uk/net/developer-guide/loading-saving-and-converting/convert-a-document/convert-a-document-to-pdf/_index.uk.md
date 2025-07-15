---
title: Конвертувати Word у PDF на C#
second_title: Aspose.Words для .NET
articleTitle: Перетворити документ у PDF
linktitle: Перетворити документ у PDF
description: "Конвертувати Word у PDF на C#. Прості приклади коду для конвертації DOCX у PDF. Підтримує всі формати Word та зображення."
type: docs
weight: 10
url: /uk/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Можливість легко та надійно конвертувати документи з одного формату в інший є ключовою функцією Aspose.Words. PDF є одним з найпопулярніших форматів для конвертації – це формат з фіксованим макетом, який зберігає оригінальний вигляд документа під час рендерингу на різних платформах. Термін "рендеринг" використовується в Aspose.Words для опису процесу перетворення документа у формат файлу, який має сторінки або концепцію сторінок.

## Конвертувати документ Word у PDF

Конвертація з Word у PDF є досить складним процесом, який потребує кілька етапів обчислень. Механізм макета Aspose.Words імітує спосіб роботи механізму макета сторінок Microsoft Word, завдяки чому вихідні PDF-документи виглядають якомога ближче до того, що ви можете побачити в Microsoft Word.

За допомогою Aspose.Words ви можете програмно перетворити документ з форматів Word, таких як DOC або DOCX, у PDF без використання Microsoft Office. Ця стаття пояснює, як виконати цю конвертацію.

{{% alert color="primary" %}}

Зверніть увагу, що кількість сторінок у документі впливає на час конвертації.

{{% /alert %}}

### Конвертувати DOCX або DOC у PDF

Перетворення з формату документа DOC або DOCX у формат PDF в Aspose.Words дуже просте і може бути досягнуто лише двома рядками коду, які:

1. Завантажте свій документ у об'єкт [Document](https://reference.aspose.com/words/net/aspose.words/document/) за допомогою одного з його конструкторів, вказавши назву документа з розширенням його формату.
1. Викличте один з методів [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) на об'єкті **Document** і вкажіть бажаний формат виводу як PDF, ввівши назву файлу з розширенням ".PDF".

Наступний приклад коду показує, як конвертувати документ з DOCX у PDF за допомогою методу [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Ви можете завантажити файл шаблону цього прикладу з [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Іноді необхідно вказати додаткові параметри, які можуть вплинути на результат збереження документа як PDF. Ці параметри можуть бути вказані за допомогою класу [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), який містить властивості, що визначають, як буде відображатися PDF-вивід.

Зверніть увагу, що за допомогою тієї ж техніки ви можете переводити будь-який документ формату потокового макета у формат PDF.

{{% /alert %}}

### Перетворити у різні стандарти PDF

Aspose.Words надає перелік [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) для підтримки конвертації DOC або DOCX у різні стандарти формату PDF (наприклад, PDF 1.7, PDF 1.5 тощо).

Наступний приклад коду демонструє, як конвертувати документ у PDF 1.7 за допомогою [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) з відповідністю до PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Конвертувати зображення у PDF

Конвертація у PDF не обмежується форматами документів Microsoft Word. Будь-який формат, що підтримується Aspose.Words, включаючи ті, що створені програмно, також може бути перетворений у PDF. Наприклад, ми можемо конвертувати односторінкові зображення, такі як JPEG, PNG, BMP, EMF або WMF, а також багатосторінкові зображення, такі як TIFF та GIF, у PDF.

Наступний приклад коду показує, як переводити зображення JPEG та TIFF у PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Щоб цей код працював, вам потрібно додати посилання на Aspose.Words та `System.Drawing` до вашого проекту.

## Зменшення розміру PDF-виводу

При збереженні у PDF ви можете вказати, чи хочете ви оптимізувати вивід. Для цього вам потрібно встановити прапорець [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) у значення true, і тоді зайві вкладені та порожні полотна будуть видалені, сусідні гліфи з однаковим форматуванням будуть об'єднані.

Наступний приклад коду показує, як оптимізувати вивід:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Використання властивості **OptimizeOutput** може вплинути на точність відображення вмісту.

{{% /alert %}}

## Дивіться також

- Стаття [Рендеринг](/words/uk/net/rendering/) для отримання додаткової інформації про формати фіксованої сторінки та потокового макета
- Стаття [Конвертація у формат фіксованої сторінки](/words/net/converting-to-fixed-page-format/#what-is-a-page-layout) для отримання додаткової інформації про макет сторінки
- Стаття [Вказівка параметрів рендерингу при перетворенні у PDF](/words/uk/net/specify-rendering-options-when-converting-to-pdf/) для отримання додаткової інформації про використання класу `PdfSaveOptions`
- Стаття [Дізнайтеся про особливості конвертації у PDF/A та PDF/UA](/words/uk/net/learn-features-of-conversion-to-pdf-a-pdf-ua/), що описує, який стандарт PDF та відповідні ISO для стандартів PDF підтримуються Aspose.Words
- Стаття [Який стандарт PDF краще вибрати](/words/uk/net/which-pdf-standard-is-better-to-choose/) для визначення того, які стандарти PDF підходять для яких випадків

- Стаття [Робота з PDF/A або PDF/UA](/words/uk/net/working-with-pdfa-or-pdfua/) описує вимоги до вмісту документа у форматах PDF/A та PDF/UA – в основному вимоги до структури та шрифтів

- Стаття [Попередження про проблеми доступності при збереженні у PDF/A та PDF/UA](/words/uk/net/warnings-when-saving-to-pdfa-and-pdfua/) описує, які вимоги доступності вмісту накладають PDF/A та PDF/UA
