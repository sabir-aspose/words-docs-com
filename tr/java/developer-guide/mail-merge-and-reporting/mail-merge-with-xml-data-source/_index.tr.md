---
title: Mail Merge XML Veri Kaynağıyla Java
second_title: Aspose.Words için Java
articleTitle: Mail Merge ile XML Veri Kaynağı
linktitle: Mail Merge ile XML Veri Kaynağı
type: docs
description: "XML dosyası da dahil olmak üzere Mail Merge işlemi gerçekleştirirken çeşitli veri kaynakları kullanın. XML kullanmanın en büyük avantajı, Java içindeki belgede doğrudan bir hiyerarşi tanımlama yeteneğidir."
keywords: "mail merge XML data source Java, Mail Merge Java"
weight: 30
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /tr/java/mail-merge-with-xml-data-source/
timestamp: 2024-01-27-14-07-04
---

XML dosyası da dahil olmak üzere Mail Merge işlemi gerçekleştirirken çeşitli veri kaynaklarını kullanabilirsiniz. XML kullanmanın en büyük avantajı, belgede bir hiyerarşi tanımlama ve ardından onu Aspose.Words 'a geçirme yeteneğidir.

Bu makalede, doğrudan bir veritabanından değil, bir XML dosyasından verilerin nasıl okunacağı ve bir Mail Merge işleminin gerçekleştirileceği veri kaynağı olarak XML'in nasıl ekleneceği açıklanacaktır.

## Veri Kaynağı Olarak XML'ın Avantajları

XML veri kaynakları, bir veritabanının yükü olmadan veri depolamak için çok kullanışlıdır. Kullanıcıların bir veritabanına bağlanamadıklarında veri eklemeleri, düzenlemeleri ve silmeleri gereken çevrimdışı uygulamalar için mükemmeldir.

XML veriler, özellikle web uygulamalarıyla çalışıyorsanız, ilişkisel veritabanlarına iyi bir veri kaynağı alternatifi olabilir. Çoğu web hizmeti bilgi alışverişinde bulunmak için XML kullanır. XML yönelimli veritabanları mevcut pazarda aktif olarak kullanılmaktadır ve ilişkisel veritabanlarının geliştiricileri, XML döndüren bir veritabanına sahip olmak için ürünlerine XML uyumluluk eklemektedir.

XML verileri düz metin biçiminde depoladığından, depolama platformdan bağımsızdır. Böylece veriler kolayca dışa aktarılabilir, içe aktarılabilir veya basitçe taşınabilir. XML bir veri kaynağı olarak popülerdir çünkü farklı uygulamalar arasında iletişim kurarken verilerin anlamsal anlamını korumanın bir yolunu sunar.

## Birleştirme Şablonunu DataSet kullanarak XML'den Gelen Verilerle Doldurma

XML, veri değişimi için evrensel standarttır ve Microsoft Word belge biçimleri, Mail Merge şablonlar için en popüler biçimlerdir. Bu nedenle, bir Mail Merge dosyasını bir XML dosyasından bir Word şablon belgesine çalıştırma yeteneği yaygın bir gereklilik haline gelmiştir.

Microsoft Word, bir Mail Merge işlemi için veri kaynağı olarak XML verileriyle çalışmak için doğrudan bir yöntem sunmazken, Aspose.Words, bir XML veri kaynağından gelen verilerle bir Mail Merge işlemi gerçekleştirmenize izin verir. XML belgesinin yapısının da değiştirilebileceğini ve verilerin yine de doğru okunacağını unutmayın. Bu, farklı türde XML belgelerin kolayca birleştirilmesini sağlar.

XML şemasını ve verilerini `DataSet` nesnesine okumak için `ReadXML` yöntemini kullanın. Bu nesne daha sonra bir mail merge için veri kaynağı olarak kullanılır.

{{% alert color="primary" %}}

Farklı veri kaynakları için aynı şablonları kullanabilirsiniz.

{{% /alert %}}

Aşağıdaki XML, birleştirme şablonunu doldurmak için gereken verileri içerir:

{{< highlight xml >}}
<?xml version="1.0" encoding="utf-8"?>
<customers>
	 <customer Name="John Ben Jan" ID="1" Domain="History" City="Boston"/>
 	<customer Name="Lisa Lane" ID="2" Domain="Chemistry" City="LA"/>
	 <customer Name="Dagomir Zits" ID="3" Domain="Heraldry" City="Milwaukee"/>
 	<customer Name="Sara Careira Santy" ID="4" Domain="IT" City="Miami"/>
</customers> 
{{< /highlight >}}

Aşağıdaki kod örneği, XML verilerinin DataSet dosyasına nasıl yükleneceğini ve ardından veri kaynağı olarak nasıl kullanılacağını gösterir:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-XMLMailMerge-XMLMailMerge.java" >}}

{{% alert color="primary" %}}

Bu örneğin örnek dosyasını şu adresten indirebilirsiniz [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20data%20-%20Customers.xml).

{{% /alert %}}

Mail Merge işlemini yürütmeden önce şablon arasındaki farkı fark edebilirsiniz:

<img src="fill-merge-template-from-xml-using-dataset-1.png" alt="fill_merge_template_from_xml_using_dataset_aspose_words_java" style="width:250px"/>

Ve Mail Merge işlemini yürüttükten sonra:

<img src="fill-merge-template-from-xml-using-dataset-2.png" alt="fill_merge_template_from_xml_aspose_words_java" style="width:285px"/>
