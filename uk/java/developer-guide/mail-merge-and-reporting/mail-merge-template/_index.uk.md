---
title: Mail Merge Шаблон в Java
second_title: Aspose.Words для Java
articleTitle: Mail Merge Шаблон
linktitle: Mail Merge Шаблон
type: docs
description: "Створіть шаблон Mail Merge для визначення фіксованого вмісту у вихідних документах, а потім створіть документи, що об'єднуються, використовуючи поля об'єднання в Java."
keywords: "create Mail Merge template Java, Mail Merge Java"
weight: 10
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /uk/java/mail-merge-template/
timestamp: 2024-01-31-14-23-37
---

Зазвичай шаблон злиття використовується як базовий документ для операції Mail Merge, якщо це простий Mail Merge або Mail Merge з регіонами. Mail merge з регіонами є більш ефективним і популярним способом, ніж простий mail merge. Простий Mail Merge розглядається як окремий випадок Mail Merge з областями, де областю є весь документ. Більш детально все пояснюється в наступній статті " типи операцій Mail Merge".

Шаблон гарантує, що текст у вихідному об'єднаному документі відформатований правильно, а операція Mail Merge гарантує, що текст із джерела даних правильно введений у шаблон об'єднання.

Aspose.Words надає можливість створити шаблон Mail Merge для визначення фіксованого вмісту, а потім генерувати документи злиття за допомогою полів злиття. Таким чином, шаблон злиття міститиме необхідний текст, який буде однаковим у всіх вихідних документах, і поля злиття для заповнення мінливого вмісту. В результаті інформація із зазначеного джерела даних буде додана в шаблон об'єднання через ці поля під час створення об'єднаного документа.

## Що таке шаблон Mail Merge

Шаблон Mail Merge - це персоналізований документ, що містить фіксовані дані та об'єднані поля, де ви хочете розмістити змінний текст. Шаблон злиття може бути в будь-якому форматі, що підтримує поля, наприклад, DOC, DOCX, DOT, DOTX, RTF. Крім того, ви також можете використовувати шаблон mustache, який детальніше описаний у статті "Синтаксис шаблону Mustache".

Ви можете створити шаблон об'єднання, який буде служити зразком для нових документів, і він повинен містити основний текст, який повинен бути однаковим для кожної версії документа, що об'єднується. Додавання полів об'єднання в шаблон буде представляти дані персоналізації, такі як Імена або адреси, які витягуються з джерела даних. Операція Mail Merge автоматично вставить дані персоналізації з вашого джерела даних у документ шаблону злиття.

Крім того, ви можете додати регіон Mail Merge до свого шаблону, вставивши два поля Mail Merge, щоб позначити початок і кінець поштового регіону. У наступній статті " типи операцій Mail Merge" це пояснюється більш детально.

## Створіть шаблон Mail Merge

Ви можете створити шаблон і додати до нього певні поля злиття, які будуть замінені значеннями з джерела даних або вручну, наприклад, за допомогою Microsoft Word, або програмно, використовуючи Aspose.Words. У цій статті ми розглянемо програмний спосіб створення шаблону.

Використовуйте клас [DocumentBuilder](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/), щоб створити необхідний шаблон злиття за допомогою Aspose.Words. Ви можете включити текст, поле для об'єднання та розрив рядка в такий шаблон, використовуючи методи [InsertTextInput](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertTextInput(java.lang.String,int,java.lang.String,java.lang.String,int)), [InsertField](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertField(int,boolean)), і [InsertParagraph](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertParagraph()).

Наступний приклад коду показує, як створити шаблон Mail Merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeTemplate-CreateMailMergeTemplate.java" >}}

На малюнку нижче показано створений шаблон:

<img src="mail-merge-template-1.png" alt="mail_merge_template_aspose_words_java" style="width:650px"/>

## Налаштування властивостей шаблону Mail Merge

Aspose.Words дозволяє налаштувати ваш шаблон за допомогою багатьох властивостей. Налаштування шаблону буде описана нижче на прикладі настройки деяких властивостей зображень і тексту.

### Налаштування властивостей зображення

Ви можете вказати Властивості зображення за допомогою класу [ImageFieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/). Зверніть увагу, що ви можете вставити зображення з бази даних, як описано в [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/c693ec7a8957051c206edc69612094a4169f6def/Examples/DocsExamples/Java/src/main/java/DocsExamples/Mail_Merge_And_Reporting/WorkingWithFields.java#L226).

Наступний приклад коду показує, як вказати ім'я файлу зображення та розмір зображення:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-ImageFieldMerging.java" >}}

### Налаштування властивостей тексту

Ви можете використовувати класи [Text]https://reference.aspose.com/words/java/com.aspose.words/Fieldmergingargs#Text) property to insert text into the document for the current merge field. Also, you can change the formatting of texts and paragraphs inside your template using [Font](https://reference.aspose.com/words/java/com.aspose.words/font/) та [ParagraphFormat](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/). Ви можете обробляти текст, який буде вставлений до або після поля об'єднання, використовуючи властивості [TextBefore](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/#TextBefore) та [TextAfter](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/#TextAfter), які включені до класу [FieldMergeField](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/).

Наступний приклад коду показує, як вставити прапорці або HTML під час операції Mail Merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-MailMergeFormFields.java" >}}

{{% alert color="primary" %}}

Ви можете завантажити приклад файлу цього прикладу з сайту [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20destinations%20-%20Fax.docx).

Ви також можете перевірити реалізацію класу `HandleMergeField` з [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/DocsExamples/Java/src/main/java/DocsExamples/Mail_Merge_And_Reporting/WorkingWithFields.java).

{{% /alert %}}

## Дивіться також

* Для отримання більш докладної інформації про те, як створювати шаблони в Microsoft Word вручну, будь ласка, ознайомтеся зі статтею [Створити шаблон](https://support.microsoft.com/en-us/office/save-a-word-document-as-a-template-cb17846d-ecec-49d4-82ea-a6f5e3e8b9ae) у документації Microsoft
