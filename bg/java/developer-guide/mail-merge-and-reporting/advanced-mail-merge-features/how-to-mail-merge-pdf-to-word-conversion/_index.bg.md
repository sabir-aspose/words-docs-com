---
title: Как да Mail Merge PDF до Word конверсия
second_title: Aspose.Words за Java
articleTitle: Как да Mail Merge PDF до Word конверсия
linktitle: Как да Mail Merge PDF до Word конверсия
type: docs
description: "Aspose.Words за Java предоставя някои разширени Mail Merge функции, които ви позволяват да обедините PDF до Word конверсия."
weight: 100
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/java/how-to-mail-merge-pdf-to-word-conversion/
timestamp: 2024-01-27-14-07-04
---

Тази статия показва прост пример за показване как да Mail Merge на документ дума конвертира от PDF и след това запишете PDF. Използвайки Aspose.Words, изпълнението на прост Mail Merge процес на PDF до Wordконвертиран файл не работи в някои случаи. Проблемът възниква, защото `Aspose.PDF` не записва действителното MERGEFIELDs по време на конвертирането PDF в DOCX (Word документи). Но това може да се постигне чрез конвертиране на тези статични текстове в действителни MERGEFIELDs и след това изпълнение на операцията Mail Merge. Моля, вижте следното заобиколно решение.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-MailMergeWordToPDF.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-mailMergeTemplate.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-HandleMergeFields.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-ReplaceEvaluatorFindAndInsertMergefield.java" >}}
