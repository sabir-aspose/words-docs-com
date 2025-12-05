---
title: Mail Merge та звіт у Java
second_title: Aspose.Words для Java
articleTitle: Mail Merge та звітність
linktitle: Mail Merge та звітність
type: docs
description: "Mail Merge - популярна функція для швидкого створення документів. Aspose.Words для Java використовує стандартну функціональність Mail Merge і розвиває її на багато кроків вперед, перетворюючи в повноцінне рішення для створення звітів, яке дозволяє створювати ще більш складні документи, такі як звіти, каталоги, інвентаризації та рахунки-фактури."
keywords: "how to use Mail Merge Java"
weight: 40
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/java/mail-merge-and-reporting/
timestamp: 2024-01-27-14-07-04
---

Mail Merge - популярна функція для швидкого та простого створення документів, таких як листи, етикетки та конверти. Aspose.Words дозволяє створювати документи на основі шаблонів з полями Mail Merge.

Поле Mail Merge - це поле, яке можна вставити в шаблон mail merge для включення певних значень із запису джерела даних у вихідні документи. Наприклад, ви можете вставити об'єднуюче поле в шаблон електронної пошти, щоб у привітанні було вказано ім'я одержувача, а не звичайне " Привіт!". Aspose.Words у ці поля розміщуються дані із зовнішнього джерела, такі як база даних або файл, і вони форматуються. Отриманий документ зберігається в зазначеній папці.

Aspose.Words використовує стандартну функціональність Mail Merge і розвиває її на багато кроків вперед, перетворюючи в повноцінне рішення для створення звітів, яке дозволяє створювати ще більш складні документи, такі як звіти, каталоги, інвентаризації та рахунки-фактури. Ось кілька переваг рішення для створення звітів Aspose.Words:

- Створюйте звіти в Microsoft Word за допомогою стандартних Mail Merge полів
- Визначте області в документі, які збільшуються, наприклад рядки детального замовлення
- Вставка зображень під час mail merge
- Виконуйте будь-яку логіку користувача, керуйте форматуванням або вставляйте складний вміст за допомогою обробників подій Mail Merge
- Заповнювати документи даними з будь-якого типу джерела даних

## Механізм та основні компоненти Mail Merge {#mechanism-and-main-components-of-a-mail-merge-operation}

Aspose.Words надає можливість завантажувати документи в різних [supported formats](https://reference.aspose.com/words/java/com.aspose.words/loadformat/) форматах, а потім дозволяє користувачам виконувати Mail Merge операції.

Зазвичай завантажений документ дозволяє зберігати поля злиття, наприклад, документ у форматі DOCX. Але є формати, які не зберігають такі поля, наприклад, TXT. Якщо Aspose.Words підтримує завантаження таких форматів файлів, ви можете додати поля злиття безпосередньо до моделі документа, зберегти документ у зручному [supported format](https://reference.aspose.com/words/java/com.aspose.words/saveformat/) вигляді та виконати операцію Mail Merge.

Операція Mail Merge об'єднає ваші *mail merge template* та ваші *data source*, щоб створити окремий *merged documents*.

## Що таке шаблон Mail Merge {#what-is-a-mail-merge-template}

Мета застосування операції mail merge з використанням шаблону злиття полягає в тому, щоб спростити процес створення документа.

Існує кілька способів створення і оформлення шаблону злиття. Ви можете використовувати Microsoft Word, і шаблон злиття не повинен бути шаблоном Microsoft Word, тобто документом у форматі DOT або DOTX, це може бути звичайний документ у форматі DOC або DOCX. Вам потрібно вставити в цей шаблон кілька спеціальних полів, які називаються полями злиття, у місцях, куди ви хочете пізніше вставити дані з джерела даних. Або ви можете програмно створити шаблон злиття за допомогою класу [DocumentBuilder](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/).

Шаблон об'єднання містить основний текст, який повинен бути однаковим у всіх вихідних документах після виконання операції Mail Merge. Ви можете використовувати будь-який формат для свого шаблону, якщо є можливість додати до нього поля для об'єднання. Усі поля для об'єднання у вашому шаблоні будуть заповнені з вашого джерела даних під час операції Mail Merge.

## Джерела даних для операції Mail Merge {#data-source-types-for-a-mail-merge-operation}

Aspose.Words Mail Merge приймає різні джерела даних. Це може бути або DataTable, DataView, DataSet, IDataReader, масив значень, підтримуваних ADO .NET, або користувацькі джерела даних, представлені реалізаціями [IMailMergeDataSource](https://reference.aspose.com/words/java/com.aspose.words/imailmergedatasource/).

Джерело даних містить всю інформацію, яка отримується під час операції Mail Merge для персоналізації окремих електронних листів та документів. Джерела даних можуть бути створені вручну або згенеровані за допомогою звітів з існуючої бази даних або Програми. Якщо у вас є дані у форматі XML, ви можете завантажити їх та об'єднати у формат DataSet. Операція Mail Merge пройде всі записи джерела даних і Вставить їх у поля Mail Merge документа. Ви можете реалізувати деякі інтерфейси mail merge, такі як [IMailMergeDataSourceRoot](https://reference.aspose.com/words/java/com.aspose.words/imailmergedatasourceroot/), щоб об'єднати дані з будь-якого джерела даних, включаючи запит LINQ, файл XML або бізнес-об'єкти.

Наступний приклад коду показує, як завантажити таблицю даних як джерело даних для операції Mail Merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ExecuteMailMergeWithRegions-ExecuteMailMergeWithRegions.java" >}}

{{% alert color="primary" %}}

Ви можете завантажити приклад файлу цього прикладу з сайту [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20destinations%20-%20Orders.docx).

{{% /alert %}}

## Об'єднані документи операції Mail Merge {#merged-documents-of-a-mail-merge-operation}

Об'єднаний документ є результатом операції Mail Merge, що виконується при об'єднанні шаблону з джерелом даних. Усі поля для об'єднання в об'єднаному документі замінюються фактичними даними з вашого джерела даних.

На наступному малюнку показаний приклад шаблону об'єднання з об'єднаними полями перед виконанням операції Mail Merge.

![mail-merge-and-reporting-aspose-words-java-1](mail-merge-and-reporting-1.jpg)

На наступному малюнку показаний приклад вихідного об'єднаного документа, отриманого в результаті виконання операції Mail Merge.

![mail-merge-and-reporting-aspose-words-java-2](mail-merge-and-reporting-2.jpg)

## Дивіться також

- [Робота з шаблонами Mail Merge в Word](https://docs.microsoft.com/en-us/power-platform/admin/work-mail-merge-templates)
