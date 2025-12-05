---
title: Mail Merge Şablon içinde Java
second_title: Aspose.Words için Java
articleTitle: Mail Merge Şablon
linktitle: Mail Merge Şablon
type: docs
description: "Çıktı belgelerindeki sabit içeriği tanımlamak için bir Mail Merge şablonu oluşturun ve ardından Java içindeki birleştirme alanlarını kullanarak birleştirme belgeleri oluşturun."
keywords: "create Mail Merge template Java, Mail Merge Java"
weight: 10
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/java/mail-merge-template/
timestamp: 2024-01-31-14-23-37
---

Basit bir Mail Merge veya bölgelere sahip Mail Merge ise, Mail Merge işlemi için temel belge olarak bir birleştirme şablonu kullanmak yaygındır. Mail merge bölgelerle basit mail merge 'den daha güçlü ve popülerdir. Basit bir Mail Merge, bölgenin belgenin tamamı olduğu bölgelerle belirli bir Mail Merge durumu olarak kabul edilir. Hepsi bir sonraki makalede "Mail Merge İşlem Türleri" daha ayrıntılı olarak açıklanmıştır.

Şablon, çıktı birleştirilmiş belgedeki metnin doğru biçimlendirilmesini sağlar ve Mail Merge işlemi, veri kaynağındaki metnin birleştirme şablonuna doğru girilmesini garanti eder.

Aspose.Words, sabit içeriği tanımlamak için bir Mail Merge şablonu oluşturma ve ardından birleştirme alanlarını kullanarak birleştirme belgeleri oluşturma olanağı sağlar. Böylece, birleştirme şablonu, tüm çıktı belgelerinde aynı olan gerekli metne ve değişen içeriği doldurmak için birleştirme alanlarına sahip olacaktır. Sonuç olarak, birleştirilmiş belgenin oluşturulması sırasında belirtilen veri kaynağından gelen bilgiler bu alanlar aracılığıyla birleştirme şablonuna eklenecektir.

## Mail Merge Şablonu nedir

Mail Merge şablonu, değişken metnin olmasını istediğiniz sabit verileri ve birleştirilmiş alanları içeren kişiselleştirilmiş bir belgedir. Birleştirme şablonu, alanları destekleyen herhangi bir biçimde olabilir, örneğin, DOC, DOCX, DOT, DOTX, RTF. Ayrıca "Mustache Şablon Sözdizimi" makalesinde açıklanan mustache şablonu daha ayrıntılı olarak da kullanabilirsiniz.

Yeni belgeler için bir model olması için bir birleştirme şablonu oluşturabilirsiniz ve birleştirilmiş belgenin her sürümü için aynı olması gereken ana metni içermelidir. Şablonun içine birleştirme alanları eklemek, bir veri kaynağından getirilen adlar veya adresler gibi kişiselleştirme verilerini temsil eder. Mail Merge işlemi, kişiselleştirme verilerini veri kaynağınızdan birleştirme şablonu belgenize otomatik olarak ekler.

Ayrıca, posta bölgesinin başlangıcını ve sonunu işaretlemek için iki Mail Merge alan ekleyerek şablonunuza bir Mail Merge bölge ekleyebilirsiniz. Bir sonraki makale "Mail Merge İşlem Türleri" bunu daha ayrıntılı olarak açıklar.

## Mail Merge Şablonu Oluşturma

Bir şablon oluşturabilir ve ona belirli birleştirme alanları ekleyebilirsiniz; bu, veri kaynağındaki değerlerle manuel olarak, örneğin Microsoft Word kullanılarak veya programlı olarak Aspose.Words kullanılarak değiştirilir. Bu makalede, bir şablon oluşturmanın programatik yoluna bakacağız.

Aspose.Words kullanarak gerekli birleştirme şablonunu oluşturmak için [DocumentBuilder](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/) sınıfını kullanın. Bir metni, birleştirme alanını ve satır sonunu kullanarak böyle bir şablona ekleyebilirsiniz. [InsertTextInput](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertTextInput(java.lang.String,int,java.lang.String,java.lang.String,int)), [InsertField](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertField(int,boolean)), ve [InsertParagraph](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertParagraph()) yöntemleri.

Aşağıdaki kod örneği, Mail Merge şablonunun nasıl oluşturulacağını gösterir:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeTemplate-CreateMailMergeTemplate.java" >}}

Aşağıdaki resim oluşturulan şablonu göstermektedir:

<img src="mail-merge-template-1.png" alt="mail_merge_template_aspose_words_java" style="width:650px"/>

## Mail Merge Şablon Özelliklerini Özelleştirme

Aspose.Words şablonunuzu birçok özellik aracılığıyla özelleştirmenize olanak tanır. Şablon özelleştirmesi, görüntülerin ve metnin bazı özelliklerinin özelleştirilmesine ilişkin bir örnekle aşağıda açıklanacaktır.

### Görüntü Özelliklerini Özelleştirme

Görüntü özelliklerini [ImageFieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/) sınıfını kullanarak belirtebilirsiniz. Veritabanından, içinde açıklandığı şekilde bir resim ekleyebileceğinizi unutmayın [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/c693ec7a8957051c206edc69612094a4169f6def/Examples/DocsExamples/Java/src/main/java/DocsExamples/Mail_Merge_And_Reporting/WorkingWithFields.java#L226).

Aşağıdaki kod örneği, görüntü dosyası adı ve görüntü boyutunun nasıl belirtileceğini gösterir:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-ImageFieldMerging.java" >}}

### Metin Özelliklerini Özelleştirme

[Text]https://reference.aspose.com/words/java/com.aspose.words/Fieldmergingargs#Text) property to insert text into the document for the current merge field. Also, you can change the formatting of texts and paragraphs inside your template using [Font](https://reference.aspose.com/words/java/com.aspose.words/font/) ve [ParagraphFormat](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/) sınıflarını kullanabilirsiniz. Birleştirme alanından önce veya sonra eklenecek metni, [FieldMergeField](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/) sınıfında bulunan [TextBefore](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/#TextBefore) ve [TextAfter](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/#TextAfter) özelliklerini kullanarak işleyebilirsiniz.

Aşağıdaki kod örneği, Mail Merge işlemi sırasında Onay Kutularının veya HTML'in nasıl ekleneceğini gösterir:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-MailMergeFormFields.java" >}}

{{% alert color="primary" %}}

Bu örneğin örnek dosyasını şu adresten indirebilirsiniz [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20destinations%20-%20Fax.docx).

`HandleMergeField` sınıfının uygulanmasını şu adresten de kontrol edebilirsiniz: [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/DocsExamples/Java/src/main/java/DocsExamples/Mail_Merge_And_Reporting/WorkingWithFields.java).

{{% /alert %}}

## Ayrıca bakınız

* Microsoft Word 'de şablonların manuel olarak nasıl oluşturulacağı hakkında daha fazla ayrıntı için lütfen [Şablon Oluşturma](https://support.microsoft.com/en-us/office/save-a-word-document-as-a-template-cb17846d-ecec-49d4-82ea-a6f5e3e8b9ae) Microsoft Belgelerindeki makale
