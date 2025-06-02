---
title: Cách Áp dụng Định dạng Tùy chỉnh trong Mail Merge
second_title: Aspose.Words cho Java
articleTitle: Cách Áp dụng Định dạng Tùy chỉnh trong Mail Merge
linktitle: Cách Áp dụng Định dạng Tùy chỉnh trong Mail Merge
type: docs
description: "Áp dụng định dạng tùy chỉnh trong thao tác Mail Merge bằng Java."
weight: 60
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /vi/java/how-to-apply-custom-formatting-during-mail-merge/
timestamp: 2024-01-27-14-07-04
---

Lớp [MailMerge](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/) cung cấp hai sự kiện có thể rất hữu ích trong việc mở rộng khả năng Mail Merge. Thuộc tính [setFieldMergingCallback(IFieldMergingCallback)](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#FieldMergingCallback) chấp nhận một lớp thực hiện các phương thức [fieldMerging(FieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#fieldMerging-com.aspose.words.FieldMergingArgs) và [imageFieldMerging(ImageFieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#imageFieldMerging-com.aspose.words.ImageFieldMergingArgs). Chúng có thể được sử dụng để thực hiện kiểm soát tùy chỉnh đối với quy trình Mail Merge.

Sự kiện **fieldMerging(FieldMergingArgs)** xảy ra trong Mail Merge khi gặp trường Mail Merge đơn giản trong tài liệu. Điều này cho phép kiểm soát thêm Mail Merge và bạn có thể thực hiện bất kỳ hành động nào khi sự kiện xảy ra. Phương thức này được bọc trong một lớp thực hiện giao diện [IFieldMergingCallBack](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/) và chấp nhận một đối tượng [FieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/fieldmergingargs/) cung cấp dữ liệu cho sự kiện tương ứng.

Ví dụ mã được đưa ra dưới đây cho thấy cách triển khai logic tùy chỉnh trong sự kiện `MergeField` để áp dụng định dạng ô.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomFormattingDuringMailMerge-ApplyCustomFormattingDuringMailMerge.java" >}}
