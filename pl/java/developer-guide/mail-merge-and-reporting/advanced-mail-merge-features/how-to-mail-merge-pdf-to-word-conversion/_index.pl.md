---
title: Jak przeliczyć Mail Merge PDF na Word
second_title: Aspose.Words dla Java
articleTitle: Jak przeliczyć Mail Merge PDF na Word
linktitle: Jak przeliczyć Mail Merge PDF na Word
type: docs
description: "Aspose.Words dla Java zapewnia zaawansowane funkcje Mail Merge, które umożliwiają scalenie konwersji PDF do Word."
weight: 100
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pl/java/how-to-mail-merge-pdf-to-word-conversion/
timestamp: 2024-01-27-14-07-04
---

W tym artykule przedstawiono prosty przykład pokazania, jak Mail Merge na dokumencie programu word przekonwertowanym z PDF, a następnie zapisać PDF. Używając Aspose.Words, wykonanie prostego procesu Mail Merge na przekonwertowanym pliku PDF do Wordnie działa w niektórych przypadkach. Problem występuje, ponieważ `Aspose.PDF` nie zapisuje rzeczywistego MERGEFIELDs podczas konwersji PDF na DOCX (Word dokumentów). Ale można to osiągnąć, konwertując te statyczne teksty na rzeczywiste MERGEFIELDs, a następnie wykonując operację Mail Merge. Zobacz następujące obejście.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-MailMergeWordToPDF.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-mailMergeTemplate.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-HandleMergeFields.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-ReplaceEvaluatorFindAndInsertMergefield.java" >}}
