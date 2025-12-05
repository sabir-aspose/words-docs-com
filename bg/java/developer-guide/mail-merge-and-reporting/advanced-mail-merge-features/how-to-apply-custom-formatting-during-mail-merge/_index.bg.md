---
title: Как да приложите персонализирано Форматиране по време на Mail Merge
second_title: Aspose.Words за Java
articleTitle: Как да приложите персонализирано Форматиране по време на Mail Merge
linktitle: Как да приложите персонализирано Форматиране по време на Mail Merge
type: docs
description: "Прилагане на форматиране по избор по време на операция Mail Merge, използвайки Java."
weight: 60
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/java/how-to-apply-custom-formatting-during-mail-merge/
timestamp: 2024-01-27-14-07-04
---

Клас [MailMerge](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/) предлага две събития, които биха могли да бъдат много полезни за разширяване на възможностите Mail Merge. Свойство [setFieldMergingCallback(IFieldMergingCallback)](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#FieldMergingCallback) приема клас, който имплементира методите [fieldMerging(FieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#fieldMerging-com.aspose.words.FieldMergingArgs) и [imageFieldMerging(ImageFieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#imageFieldMerging-com.aspose.words.ImageFieldMergingArgs). Те могат да се използват за осъществяване на персонализиран контрол върху процеса Mail Merge.

Събитието **fieldMerging(FieldMergingArgs)** възниква по време на Mail Merge, когато в документа се срещне просто Mail Merge поле. Това дава допълнителен контрол върху Mail Merge и можете да извършвате всякакви действия, когато настъпи събитието. Този метод е опакован в клас, който имплементира интерфейс [IFieldMergingCallBack](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/) и приема обект [FieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/fieldmergingargs/), който предоставя данни за съответното събитие.

Примерът с код, даден по-долу, показва как да се приложи потребителска логика в събитието `MergeField`, за да се приложи форматирането на клетки.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomFormattingDuringMailMerge-ApplyCustomFormattingDuringMailMerge.java" >}}
