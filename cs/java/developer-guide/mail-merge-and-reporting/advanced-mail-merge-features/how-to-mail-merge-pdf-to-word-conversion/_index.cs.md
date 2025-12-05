---
title: Jak převést Mail Merge PDF na Word
second_title: Aspose.Words pro Java
articleTitle: Jak převést Mail Merge PDF na Word
linktitle: Jak převést Mail Merge PDF na Word
type: docs
description: "Aspose.Words pro Java poskytuje některé pokročilé funkce Mail Merge, které vám umožňují sloučit převod PDF na Word."
weight: 100
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cs/java/how-to-mail-merge-pdf-to-word-conversion/
timestamp: 2024-01-27-14-07-04
---

Tento článek ukazuje jednoduchý příklad, jak ukázat, jak Mail Merge na dokumentu aplikace word převedeném z PDF a poté uložit PDF. Použití Aspose.Words, provádění jednoduchého procesu Mail Merge na převedeném souboru PDF na Words v některých případech nefunguje. K problému dochází, protože `Aspose.PDF` nezapíše skutečné MERGEFIELDs během převodu PDF na DOCX (Word dokumenty). Ale toho lze dosáhnout převedením těchto statických textů na skutečné MERGEFIELDs a následným provedením operace Mail Merge. Viz následující řešení.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-MailMergeWordToPDF.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-mailMergeTemplate.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-HandleMergeFields.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-ReplaceEvaluatorFindAndInsertMergefield.java" >}}
