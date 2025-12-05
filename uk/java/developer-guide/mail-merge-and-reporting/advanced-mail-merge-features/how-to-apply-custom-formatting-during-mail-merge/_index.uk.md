---
title: Як застосувати спеціальне форматування під час Mail Merge
second_title: Aspose.Words для Java
articleTitle: Як застосувати спеціальне форматування під час Mail Merge
linktitle: Як застосувати спеціальне форматування під час Mail Merge
type: docs
description: "Застосуйте спеціальне форматування під час операції Mail Merge за допомогою Java."
weight: 60
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/java/how-to-apply-custom-formatting-during-mail-merge/
timestamp: 2024-01-27-14-07-04
---

Клас [MailMerge](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/) надає дві події, які можуть бути дуже корисними для розширення можливостей Mail Merge. Властивість [setFieldMergingCallback(IFieldMergingCallback)](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#FieldMergingCallback) приймає клас, який реалізує методи [fieldMerging(FieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#fieldMerging-com.aspose.words.FieldMergingArgs) та [imageFieldMerging(ImageFieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#imageFieldMerging-com.aspose.words.ImageFieldMergingArgs). Вони можуть бути використані для реалізації користувальницького управління процесом Mail Merge.

Подія **fieldMerging(FieldMergingArgs)** відбувається під час Mail Merge, коли в документі зустрічається просте поле Mail Merge. Це дає додатковий контроль над Mail Merge, і ви можете виконувати будь-які дії при виникненні події. Цей метод укладений у клас, який реалізує інтерфейс [IFieldMergingCallBack](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/) і приймає об'єкт [FieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/fieldmergingargs/), що надає дані для відповідної події.

Наведений нижче приклад коду демонструє, як реалізувати логіку користувача в події `MergeField` для застосування форматування комірок.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomFormattingDuringMailMerge-ApplyCustomFormattingDuringMailMerge.java" >}}
