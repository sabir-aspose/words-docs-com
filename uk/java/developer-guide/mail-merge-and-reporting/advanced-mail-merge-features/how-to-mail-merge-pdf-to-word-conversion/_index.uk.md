---
title: Як перетворити Mail Merge PDF на Word
second_title: Aspose.Words для Java
articleTitle: Як перетворити Mail Merge PDF на Word
linktitle: Як перетворити Mail Merge PDF на Word
type: docs
description: "Aspose.Words для Java надає деякі розширені функції Mail Merge, які дозволяють об'єднувати перетворення з PDF в Word."
weight: 100
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/java/how-to-mail-merge-pdf-to-word-conversion/
timestamp: 2024-01-27-14-07-04
---

У цій статті наведено простий приклад, який показує, як виконати Mail Merge у документі word, перетвореному з PDF, а потім зберегти PDF. Використовуючи Aspose.Words, виконання простого процесу Mail Merge у перетвореному файлі з PDF на Word в деяких випадках не працює. Проблема виникає через те, що `Aspose.PDF` не записує фактичні MERGEFIELDs під час перетворення PDF в DOCX (документи Word). Але цього можна досягти, перетворивши ці статичні тексти на фактичні MERGEFIELDs, а потім виконавши операцію Mail Merge. Будь ласка, ознайомтеся з наступним рішенням.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-MailMergeWordToPDF.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-mailMergeTemplate.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-HandleMergeFields.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-ReplaceEvaluatorFindAndInsertMergefield.java" >}}
