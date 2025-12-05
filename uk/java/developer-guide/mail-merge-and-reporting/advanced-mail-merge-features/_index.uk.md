---
title: Розширені функції Mail Merge в Java
second_title: Aspose.Words для Java
articleTitle: Розширені функції Mail Merge
linktitle: Розширені функції Mail Merge
type: docs
description: "Aspose.Words для Java надає деякі розширені функції Mail Merge, які дозволяють виконувати подальшу настройку Mail Merge. Наприклад, отримання інформації про структуру шаблону, налаштування правил, очищення після виконання операції Mail Merge та інші."
keywords: "use advanced Mail Merge features java, Mail Merge java"
weight: 50
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/java/advanced-mail-merge-features/
timestamp: 2024-01-27-14-07-04
---

Aspose.Words надає деякі додаткові Mail Merge властивості та методи, які дозволяють додатково налаштувати процес Mail Merge Як простий Mail Merge або Mail Merge з регіонами.

Розширені функції Mail Merge включають, але не обмежуються ними, отримання інформації про структуру шаблону перед виконанням операції Mail Merge, налаштування правил для операції Mail Merge та очищення під час операції Mail Merge. У цій статті ми розглянемо лише кілька властивостей та прикладів, які покажуть вам, як використовувати розширені функції.

## Встановіть правила для операцій Mail Merge

Додавання правил до шаблону дозволяє зробити робочий процес більш ефективним та гнучким. Використовуючи правила Mail Merge, ви можете налаштувати вміст, який можна швидко змінити, і уникнути необхідності створювати кілька документів.

Aspose.Words дозволяє налаштувати Mail Merge на основі правил, які запускаються під час виконання операції Mail Merge та управління інформацією про злиття. Наприклад, коли ви створюєте електронне повідомлення або листування для відправки всім своїм клієнтам. Ви можете налаштувати правило таким чином, щоб лист міг містити різні дані на основі різних значень у певних полях вашого джерела даних.

Погляньте на деякі правила Mail Merge, які ви можете реалізувати.

### Реалізуйте наступне поле для об'єднання записів даних у поточному документі

Ви можете використовувати поле [Next](https://reference.aspose.com/words/java/com.aspose.words/fieldnext/) для об'єднання наступного запису даних у поточний отриманий об'єднаний документ, замість того, щоб створювати новий об'єднаний документ. Воно використовується для відображення декількох записів в одному документі.

### Реалізуйте поля NextIf та SkipIf для порівняння двох виразів

Ви можете використовувати поле [NextIf](https://reference.aspose.com/words/java/com.aspose.words/fieldnextif/) або поле [SkipIf](https://reference.aspose.com/words/java/com.aspose.words/fieldskipif/), якщо хочете порівняти два вирази (вирази [right](https://reference.aspose.com/words/java/com.aspose.words/fieldif/#getRightExpression) та [left](https://reference.aspose.com/words/java/com.aspose.words/fieldif/#getLeftExpression)) з деяким значенням [operator](https://reference.aspose.com/words/java/com.aspose.words/fieldskipif/#getComparisonOperator).

**NextIf**

| **Field Name** | **Comparison Result "True"** | **Comparison Result "False"** |
| -------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `NextIf` | Aspose.Words призведе до об'єднання наступного запису даних з поточним документом злиття, і всі поля злиття в шаблоні, які знаходяться після поля *NextIf*, будуть замінені значеннями з наступного запису даних, а не з поточного запису даних. | Aspose.Words призведе до об'єднання наступного запису даних у Новий об'єднуючий документ. |
| `SkipIf` | Aspose.Words скасує поточний об'єднуючий документ, перейде до наступного запису даних у джерелі даних та запустить новий об'єднуючий документ. | Aspose.Words продовжить роботу з поточним об'єднуючим документом. |

Наступний приклад коду показує, як порівняти два вирази з **NextIf** або **SkipIf**:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-AdvancedMailMergeFeatures-CompareTwoExpressions.java" >}}

## Отримати інформацію про структуру шаблону

Aspose.Words Дозволяє збирати різну інформацію у вашому шаблоні різними способами. Наприклад, вам може знадобитися отримати назви деяких полів злиття або ієрархію регіонів у вашому шаблоні. Тепер ми пояснимо можливі варіанти отримання певної інформації з вашого шаблону.

### Отримання імен полів злиття

Ви можете зіткнутися зі сценарієм, коли вам захочеться об'єднати дані з полями злиття, створеними іншими користувачами, і в цьому випадку ви не будете впевнені в точних назвах полів злиття. Отже, для досягнення мети Mail Merge, по-перше, вам потрібно буде прочитати та відобразити назви всіх полів злиття. Aspose.Words дозволяє отримати колекцію імен полів злиття, використовуючи метод [GetFieldNames](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/getfieldnames/).

Наступний приклад коду показує, як отримати імена всіх полів злиття в шаблоні:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-fields-GetFieldNames-GetFieldNames.java" >}}

### Отримайте інформацію про регіони злиття

Можливо, у вас є сценарій, коли ви хочете зрозуміти, як структурований ваш шаблон за допомогою зазначених областей злиття. Ви можете використовувати деякі методи для збору всієї необхідної інформації про регіони злиття або для отримання ієрархії областей злиття у вашому шаблоні, наприклад, метод [GetRegionsHierarchy](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#getRegionsHierarchy). Ви можете використовувати властивості та методи з [MailMergeRegionInfo](https://reference.aspose.com/words/java/com.aspose.words/mailmergeregioninfo/) class.The наступного прикладу коду, який показує, як отримати ієрархію областей злиття:

**Java**
{{< highlight java >}}

MailMergeRegionInfo regionInfo = doc.getMailMerge().getRegionsHierarchy();

{{< /highlight >}}

Наступний приклад коду показує, як отримати певні області злиття всередині вашого шаблону на основі їх назв:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ExecuteMailMergeWithRegions-GetRegionsByName.java" >}}

{{% alert color="primary" %}}

Ви можете завантажити приклад файлу цього прикладу з сайту [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/tree/master/Examples/src/main/resources/MailMerge).

{{% /alert %}}

### Додавання зіставлених полів

Aspose.Words дозволяє автоматично зіставляти назви полів у вашому джерелі даних та назви полів Mail Merge у шаблоні, використовуючи властивість [MappedDataFields](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#getMappedDataFields). Наприклад, якщо у вашому шаблоні є поле з назвою "Last Name", а у вашому джерелі даних є поле з назвою "Last Name" або іншим варіантом, таким як "Last_Name" або "LastName", тоді поле у джерелі даних буде автоматично зіставлено з відповідним іменем. відображене поле. Якщо шаблон злиття повинен бути об'єднаний з багатьма джерелами даних, зіставлені поля не вимагають повторного введення полів у шаблон для узгодження з іменами полів у базі даних.

Наступний приклад коду показує, як додати зіставлене поле за допомогою методу [Add](https://reference.aspose.com/words/java/com.aspose.words/mappeddatafieldcollection/#add-java.lang.String-java.lang.String), коли комбіноване поле в шаблоні та поле даних у джерелі даних мають різні назви:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-fields-GetFieldNames-MappedFieldNames.java" >}}
