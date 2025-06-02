---
title: Jak použít vlastní formátování během Mail Merge
second_title: Aspose.Words pro Java
articleTitle: Jak použít vlastní formátování během Mail Merge
linktitle: Jak použít vlastní formátování během Mail Merge
type: docs
description: "Použijte vlastní formátování během operace Mail Merge pomocí Java."
weight: 60
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/java/how-to-apply-custom-formatting-during-mail-merge/
timestamp: 2024-01-27-14-07-04
---

Třída [MailMerge](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/) poskytuje dvě události, které by mohly být velmi užitečné při rozšiřování funkcí Mail Merge. Vlastnost [setFieldMergingCallback(IFieldMergingCallback)](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#FieldMergingCallback) přijímá třídu, která implementuje metody [fieldMerging(FieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#fieldMerging-com.aspose.words.FieldMergingArgs) a [imageFieldMerging(ImageFieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#imageFieldMerging-com.aspose.words.ImageFieldMergingArgs). Ty lze použít k implementaci vlastní kontroly nad procesem Mail Merge.

Událost **fieldMerging(FieldMergingArgs)** nastane během Mail Merge, když se v dokumentu objeví jednoduché pole Mail Merge. To dává další kontrolu nad Mail Merge a můžete provádět jakékoli akce, když dojde k události. Tato metoda je zabalena do třídy, která implementuje rozhraní [IFieldMergingCallBack](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/) a přijímá objekt [FieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/fieldmergingargs/), který poskytuje data pro odpovídající událost.

Příklad kódu uvedený níže ukazuje, jak implementovat vlastní logiku v události `MergeField` pro použití formátování buňky.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomFormattingDuringMailMerge-ApplyCustomFormattingDuringMailMerge.java" >}}
