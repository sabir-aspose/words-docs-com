---
title: Jak zastosować niestandardowe formatowanie podczas Mail Merge
second_title: Aspose.Words dla Java
articleTitle: Jak zastosować niestandardowe formatowanie podczas Mail Merge
linktitle: Jak zastosować niestandardowe formatowanie podczas Mail Merge
type: docs
description: "Zastosuj niestandardowe formatowanie podczas operacji Mail Merge przy użyciu Java."
weight: 60
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pl/java/how-to-apply-custom-formatting-during-mail-merge/
timestamp: 2024-01-27-14-07-04
---

Klasa [MailMerge](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/) zapewnia dwa zdarzenia, które mogą być bardzo przydatne w rozszerzaniu możliwości Mail Merge. Właściwość [setFieldMergingCallback(IFieldMergingCallback)](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#FieldMergingCallback) akceptuje klasę, która implementuje metody [fieldMerging(FieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#fieldMerging-com.aspose.words.FieldMergingArgs) i [imageFieldMerging(ImageFieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#imageFieldMerging-com.aspose.words.ImageFieldMergingArgs). Można ich użyć do zaimplementowania niestandardowej kontroli nad procesem Mail Merge.

Zdarzenie **fieldMerging(FieldMergingArgs)** występuje podczas Mail Merge, gdy w dokumencie napotkane jest proste pole Mail Merge. Daje to dalszą kontrolę nad Mail Merge i możesz wykonywać dowolne działania, gdy wystąpi zdarzenie. Ta metoda jest opakowana w klasę, która implementuje interfejs [IFieldMergingCallBack](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/) i akceptuje obiekt [FieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/fieldmergingargs/), który dostarcza dane dla odpowiedniego zdarzenia.

Poniższy przykład kodu pokazuje, jak zaimplementować logikę niestandardową w zdarzeniu `MergeField`, Aby zastosować formatowanie komórek.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomFormattingDuringMailMerge-ApplyCustomFormattingDuringMailMerge.java" >}}
