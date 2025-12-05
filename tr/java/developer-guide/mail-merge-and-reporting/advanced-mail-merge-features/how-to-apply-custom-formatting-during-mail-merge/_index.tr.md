---
title: Mail Merge sırasında Özel Biçimlendirme Nasıl Uygulanır
second_title: Aspose.Words için Java
articleTitle: Mail Merge sırasında Özel Biçimlendirme Nasıl Uygulanır
linktitle: Mail Merge sırasında Özel Biçimlendirme Nasıl Uygulanır
type: docs
description: "Java kullanarak Mail Merge işlemi sırasında özel biçimlendirme uygulayın."
weight: 60
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/java/how-to-apply-custom-formatting-during-mail-merge/
timestamp: 2024-01-27-14-07-04
---

[MailMerge](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/) sınıfı, Mail Merge yeteneklerini genişletmede çok yararlı olabilecek iki olay sağlar. [setFieldMergingCallback(IFieldMergingCallback)](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#FieldMergingCallback) özelliği, [fieldMerging(FieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#fieldMerging-com.aspose.words.FieldMergingArgs) ve [imageFieldMerging(ImageFieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#imageFieldMerging-com.aspose.words.ImageFieldMergingArgs) yöntemlerini uygulayan bir sınıfı kabul eder. Bunlar, Mail Merge işlemi üzerinde özel denetim uygulamak için kullanılabilir.

**fieldMerging(FieldMergingArgs)** olayı, belgede basit bir Mail Merge alanıyla karşılaşıldığında Mail Merge sırasında gerçekleşir. Bu, Mail Merge üzerinde daha fazla kontrol sağlar ve olay gerçekleştiğinde herhangi bir işlemi gerçekleştirebilirsiniz. Bu yöntem, [IFieldMergingCallBack](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/) arabirimini uygulayan ve karşılık gelen olay için veri sağlayan bir [FieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/fieldmergingargs/) nesnesini kabul eden bir sınıfa sarılır.

Aşağıda verilen kod örneği, hücre biçimlendirmesini uygulamak için `MergeField` olayında özel mantığın nasıl uygulanacağını gösterir.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomFormattingDuringMailMerge-ApplyCustomFormattingDuringMailMerge.java" >}}
