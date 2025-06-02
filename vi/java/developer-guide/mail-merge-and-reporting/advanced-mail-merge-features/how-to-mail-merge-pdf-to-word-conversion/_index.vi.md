---
title: Làm thế nào để Mail Merge PDF để Word Chuyển Đổi
second_title: Aspose.Words cho Java
articleTitle: Làm thế nào để Mail Merge PDF để Word Chuyển Đổi
linktitle: Làm thế nào để Mail Merge PDF để Word Chuyển Đổi
type: docs
description: "Aspose.Words cho Java cung cấp một số tính năng nâng cao Mail Merge cho phép bạn hợp nhất PDF thành Word chuyển đổi."
weight: 100
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /vi/java/how-to-mail-merge-pdf-to-word-conversion/
timestamp: 2024-01-27-14-07-04
---

Bài viết này trình bày một ví dụ đơn giản về cách hiển thị Mail Merge trên tài liệu word được chuyển đổi từ PDF và sau đó lưu PDF. Sử dụng Aspose.Words, thực hiện một quy trình Mail Merge đơn giản trên tệp được chuyển đổi PDF thành Wordkhông hoạt động đối với một số trường hợp. Vấn đề xảy ra do `Aspose.PDF` không ghi MERGEFIELDs thực tế trong quá trình chuyển đổi PDF thành DOCX (Word tài liệu). Nhưng nó có thể đạt được bằng cách chuyển đổi các văn bản tĩnh đó thành MERGEFIELDs thực tế và sau đó thực hiện thao tác Mail Merge. Vui lòng xem cách giải quyết sau.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-MailMergeWordToPDF.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-mailMergeTemplate.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-HandleMergeFields.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeWordToPDF-ReplaceEvaluatorFindAndInsertMergefield.java" >}}
