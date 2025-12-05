---
title: Mail Merge sırasında Checkbox es, Metin Girişi veya Resim ekleyin
second_title: Aspose.Words için Java
articleTitle: Checkboxes, Metin Girişi veya Resim Ekleme
linktitle: Checkboxes, Metin Girişi veya Resim Ekleme
description: "Java kullanarak Mail Merge sırasında checkbox es veya metin giriş alanları ekleyin. Ayrıca Mail Merge sırasında Java içindeki bir Veritabanından görüntüler ekleyin."
type: docs
weight: 20
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/java/insert-checkboxes-text-input-or-images-mail-merge/
timestamp: 2024-01-27-14-07-04
---

Birleştirme altyapısı bir belgeyi girdi olarak alır, içindeki `MERGEFIELD` alanları arar ve bunları veri kaynağından elde edilen verilerle değiştirir. Genellikle düz metin ve HTML eklenir, ancak Aspose.Words kullanıcıları Mail Merge alanlar için daha sıra dışı senaryoları işleyen bir belge de oluşturabilir.

Güçlü Aspose.Words işlevi, Mail Merge işlemini genişletmenize olanak tanır:

- mail merge sırasında belgeye checkboxes ve metin giriş formu alanları ekleyin
- herhangi bir özel depolama alanından (dosyalar, BLOB alanlar vb.) Görüntüler ekleyin.)

## Mail Merge sırasında Checkbox es ve Metin Girişi ekleyin

Bazen birleştirme alanında metnin yerine Mail Merge değil, checkbox veya metin giriş alanının geçmesi için bir checkbox işlemi gerçekleştirmek gerekir. Bu en yaygın senaryo olmasa da, bazı görevler için çok kullanışlıdır.

Word belgesinin aşağıdaki ekran görüntüsü, birleştirme alanlarına sahip bir şablonu gösterir:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-1](insert-checkboxes-html-or-images-during-mail-merge_1.jpeg)

Aşağıdaki Word belgesinin bu ekran görüntüsü, önceden oluşturulmuş belgeyi gösterir:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-2](insert-checkboxes-html-or-images-during-mail-merge-2.png)

{{% alert color="primary" %}}

Bazı alanların düz metinle değiştirildiğini, bazı alanların checkbox form alanlarıyla değiştirildiğini ve `Subject` alanının bir metin giriş alanıyla değiştirildiğini unutmayın.

{{% /alert %}}

Aşağıdaki kod örneği, bir mail merge sırasında bir belgeye checkbox'lerin nasıl ekleneceğini ve metin alanlarının nasıl girileceğini gösterir.:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-MailMergeFormFields.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-HandleMergeField.java" >}}

## Mail Merge sırasında Resim ekleme

Bir Mail Merge işlemi gerçekleştirirken, özel ımage Mail Merge alanlarını kullanarak veritabanından görüntüleri belgeye ekleyebilirsiniz. Image Mail Merge alanı, Image:MyFieldName adlı bir birleştirme alanıdır.

### Veritabanından Resim Ekleme

Bir mail merge sırasında, bir belgede bir görüntü Mail Merge alanıyla karşılaşıldığında, [FieldMergingCallback](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#getFieldMergingCallback) olayı tetiklenir. Belgeye eklenebilmesi için Mail Merge altyapısına bir dosya adı, akış veya görüntü nesnesi döndürmek üzere bu olaya yanıt verebilirsiniz.

Aşağıdaki kod örneği, bir veritabanı BLOB alanında depolanan görüntülerin bir rapora nasıl ekleneceğini gösterir:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageFromBlob.java" >}}

### Mail Merge sırasında Görüntü Özelliklerini Ayarlama

Bir görüntü birleştirme alanını birleştirirken, bazen [WrapType](https://reference.aspose.com/words/java/com.aspose.words/wraptype/) gibi çeşitli görüntü özelliklerini kontrol etmeniz gerekebilir.

Şu anda [ImageFieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/) kullanarak sırasıyla yalnızca görüntü genişliği veya yükseklik özelliklerini ayarlayabilirsiniz. Bu sorunun üstesinden gelmek için Aspose.Words, eklenen görüntü veya başka herhangi bir şekil üzerinde tam kontrol sahibi olmayı kolaylaştıran [Shape](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/#getShape) özelliğini sağlar.

Aşağıdaki kod örneği, çeşitli görüntü özelliklerinin nasıl ayarlanacağını gösterir:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-MailMergeImageField.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-FieldMergingHandler.java" >}}

