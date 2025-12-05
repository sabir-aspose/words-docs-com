---
title: Birleştirilmemiş Bölgelere Özel Mantık Nasıl Uygulanır
second_title: Aspose.Words için Java
articleTitle: Birleştirilmemiş Bölgelere Özel Mantık Nasıl Uygulanır
linktitle: Birleştirilmemiş Bölgelere Özel Mantık Nasıl Uygulanır
type: docs
description: "Java kullanarak Mail Merge işlemi sırasında birleştirilmemiş bölgelere özel mantık uygulayın."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/java/how-to-apply-custom-logic-to-unmerged-regions/
timestamp: 2024-01-27-14-07-04
---

Mail Merge sırasında birleştirilmemiş bölgelerin belgeden tamamen kaldırılmasının istenmediği veya belgenin eksik görünmesine neden olduğu bazı durumlar vardır. Bu, giriş verilerinin yokluğunun kullanıcıya tamamen kaldırılan bölge yerine bir mesaj şeklinde görüntülenmesi gerektiğinde ortaya çıkabilir.

Kullanılmayan bölgenin kendi başına kaldırılmasının yeterli olmadığı zamanlar da vardır, örneğin, bölgenin önünde bir başlık varsa veya bölge bir tabloda yer alıyorsa. Bu bölge kullanılmazsa, belgede yer almayan bölge kaldırıldıktan sonra başlık ve tablo kalır.

Bu makalede, belgedeki kullanılmayan bölgelerin nasıl işleneceğini el ile tanımlamak için bir çözüm sunulmaktadır. Bu işlevin temel kodu sağlanır ve başka bir projede kolayca yeniden kullanılabilir.

Her bölgeye uygulanacak mantık, [IFieldMergingCallback](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/) arabirimini uygulayan bir sınıfın içinde tanımlanır. Aynı şekilde, her alanın nasıl birleştirileceğini kontrol etmek için bir Mail Merge işleyicisi ayarlanabilir, bu işleyici kullanılmayan bir bölgedeki her alan veya bir bütün olarak bölge üzerinde eylemler gerçekleştirecek şekilde ayarlanabilir. Bu işleyicide, kodu bir bölgenin metnini değiştirecek, düğümleri veya boş satırları ve hücreleri kaldıracak şekilde ayarlayabilirsiniz.

Bu örnekte, aşağıda görüntülenen belgeyi kullanacağız. İç içe geçmiş bölgeleri ve bir tablonun içinde bulunan bir bölgeyi içerir.

![apply-custom-logic-to-unmerged-regions-aspose-words-java](how-to-apply-custom-logic-to-unmerged-regions-1.png)

Hızlı bir gösteri olarak, örnek belge üzerinde [MailMergeCleanupOptions.REMOVE_UNUSED_REGIONS](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/) bayrağı etkinleştirilmiş örnek bir veritabanı çalıştırabiliriz. Bu özellik, mail merge sırasında birleştirilmemiş bölgeleri belgeden otomatik olarak kaldıracaktır.

Veri kaynağı **StoreDetails** bölgesi için iki kayıt içerir, ancak kasıtlı olarak kayıtlardan biri için alt **ContactDetails** bölgeleri için herhangi bir veriye sahiptir. Ayrıca, **Suppliers** bölgesinde de herhangi bir veri satırı yoktur. Bu, kullanılmayan bölgelerin belgede kalmasına neden olur. Belgeyi bu veri kaynağıyla birleştirdikten sonraki sonuç aşağıdadır.

![merged-regions-aspose-words-java](how-to-apply-custom-logic-to-unmerged-regions-2.png)

Resimde belirtildiği gibi, ikinci kayıt için **ContactDetails** bölgesinin ve **Suppliers** bölgelerinin, verileri olmadığı için Mail Merge motoru tarafından otomatik olarak kaldırıldığını görebilirsiniz. Ancak, bu çıktı belgesinin eksik görünmesine neden olan birkaç sorun vardır:

- **ContactDetails** bölgesi hala "İletişim Bilgileri" metninin bulunduğu bir paragraf bırakır.
- Aynı durumda, telefon numarası olmadığına dair bir işaret yoktur, yalnızca karışıklığa yol açabilecek boş bir alan vardır.
- **Suppliers** bölgesi ile ilgili tablo ve başlık, tablonun içindeki bölge kaldırıldıktan sonra da kalır.

Bu makalede sağlanan teknik, bu sorunları önlemek için birleştirilmemiş her bölgeye özel mantığın nasıl uygulanacağını gösterir.

**Çözüm**

Belgedeki kullanılmayan her bölgeye mantığı manuel olarak uygulamak için Aspose.Words 'da zaten mevcut olan özelliklerden yararlanıyoruz.

Mail Merge altyapısı, kullanılmayan bölgeleri **MailMergeCleanupOptions.RemoveUnusedRegions** bayrağı aracılığıyla kaldırmak için bir özellik sağlar. Bu, mail merge sırasında bu tür bölgelere dokunulmaması için devre dışı bırakılabilir. Bu, birleştirilmemiş bölgeleri belgede bırakmamızı ve bunun yerine bunları kendimiz manuel olarak ele almamızı sağlar.

Daha sonra **MailMerge.FieldMergingCallback** özelliğinden, **IFieldMergingCallback** arabirimini uygulayan bir işleyici sınıfı kullanarak Mail Merge sırasında bu birleştirilmemiş bölgelere kendi özel mantığımızı uygulamak için bir araç olarak yararlanabiliriz.

İşleyici sınıfı içindeki bu kod, birleştirilmemiş bölgelere uygulanan mantığı kontrol etmek için değiştirmeniz gereken tek sınıftır. Bu örnekteki diğer kod, herhangi bir projede değişiklik yapılmadan yeniden kullanılabilir.

Bu örnek proje bu tekniği göstermektedir. Aşağıdaki adımları içerir:

1. Veri kaynağınızı kullanarak belge üzerinde Mail Merge yürütün. **MailMergeCleanupOptions.RemoveUnusedRegions** bayrağı devre dışı şimdilik bölgelerin kalmasını istiyoruz, böylece bunları manuel olarak halledebiliriz. Veri içermeyen tüm bölgeler belgede birleştirilmeden bırakılacaktır.
1. **ExecuteCustomLogicOnEmptyRegions** yöntemini çağırın. Bu yöntem, bu örnekte verilmiştir. Birleştirilmemiş her bölge için belirtilen işleyicinin çağrılmasına izin veren eylemler gerçekleştirir. Bu yöntem yeniden kullanılabilir ve bunu gerektiren herhangi bir projeye (bağımlı yöntemlerle birlikte) değiştirilmeden kopyalanabilir.Bu yöntem aşağıdaki adımları yürütür:
   1. Kullanıcı tarafından belirtilen işleyiciyi **MailMerge.FieldMergingCallback** özelliğine ayarlar.
   1. Kullanıcının **Document** ve **ArrayList** içeren bölge adlarını kabul eden **CreateDataSourceFromDocumentRegions** yöntemini çağırır. Bu yöntem, belgedeki birleştirilmemiş her bölge için tablolar içeren sahte bir veri kaynağı oluşturacaktır.
   1. Sahte veri kaynağını kullanarak belge üzerinde Mail Merge yürütür. Mail Merge bu veri kaynağıyla çalıştırıldığında, her birleştirme bölgesi ve uygulanan özel mantık için kullanıcı tarafından belirtilen işleyicinin çağrılmasına izin verir

**Kod**

**ExecuteCustomLogicOnEmptyRegions** yönteminin uygulaması aşağıda bulunur. Bu yöntem birkaç parametreyi kabul eder:

1. Geçirilen işleyici tarafından işlenecek birleştirilmemiş bölgeleri içeren [Document](https://reference.aspose.com/words/java/com.aspose.words/document/) nesnesi.
1. Birleştirilmemiş bölgelere uygulanacak mantığı tanımlayan işleyici sınıfı. Bu işleyici aşağıdakileri uygulamalıdır: [IFieldMergingCallback](https://www.aspose.com/api/java/words/com.aspose.words/interfaces/IFieldMergingCallback) arayüz.
1. Uygun aşırı yükün kullanılmasıyla, yöntem üçüncü bir parametreyi de kabul edebilir – bölge adlarının dize olarak bir listesi. Bu belirtilirse, yalnızca listede belirtilen belgede kalan bölge adları el ile işlenir. Karşılaşılan diğer bölgeler işleyici tarafından çağrılmayacak ve otomatik olarak kaldırılacaktır. Yalnızca iki parametreli aşırı yük belirtildiğinde, belgede kalan her bölge el ile işlenecek yönteme dahil edilir.

**Örnek**

Belirtilen işleyiciyi kullanarak kullanılmayan bölgelerde özel mantığın nasıl çalıştırılacağını gösterir.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ExecuteCustomLogicOnUnusedRegions.java" >}}

{{% alert color="primary" %}}

**ExecuteCustomLogicOnEmptyRegions** yöntemini farklı işleyicilerle ardışık olarak çalıştırmayı düşünüyorsanız (örneğin, her işleyici belirli alanlara mantık uygular), kullanılmayan bölgelerin kaldırılmasını devre dışı bırakmanız gerekir, böylece bu tür bölgeler bu çağrılar arasında kaldırılmaz.

{{% /alert %}}

**Örnek**

Birleştirilmemiş bölgeleri el ile işlemek için kullanılan yöntemi tanımlar.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ManuallyHandleUnmergedRegions.java" >}}

Bu yöntem, belgedeki birleştirilmemiş tüm bölgeleri bulmayı içerir. Bu **MailMerge.GetFieldNames** yöntemi kullanılarak gerçekleştirilir. Bu yöntem, bölge başlangıç ve bitiş işaretçileri de dahil olmak üzere belgedeki tüm birleştirme alanlarını döndürür (*TableStart* veya *TableEnd* önekine sahip birleştirme alanlarıyla temsil edilir).

Bir `TableStart` birleştirme alanıyla karşılaşıldığında bu, **DataSet** 'ye yeni bir **DataTable** olarak eklenir. Bir bölge birden çok kez görünebileceğinden (örneğin, üst bölgenin birden çok kayıtla birleştirildiği iç içe geçmiş bir bölge olduğu için), tablo yalnızca **DataSet** içinde zaten yoksa oluşturulur ve eklenir.

Uygun bir bölge başlangıcı bulunup veritabanına eklendiğinde, bir sonraki alan (bölgedeki ilk alana karşılık gelir) **DataTable** 'a eklenir. Birleştirilecek ve işleyiciye iletilecek bölgedeki her alan için yalnızca ilk alanın eklenmesi gerekir.

Ayrıca, bölgedeki ilk veya diğer alanlara mantık uygulamayı kolaylaştırmak için ilk alanın alan değerini "FirstField" olarak ayarladık. Bunu dahil ederek, ilk alanın adını sabit kodlamanın gerekli olmadığı veya geçerli alanın işleyici kodunda ilk olup olmadığını kontrol etmek için fazladan kod uygulamanın gerekli olmadığı anlamına gelir.

Aşağıdaki kod, bu sistemin nasıl çalıştığını gösterir. Bu makalenin başında gösterilen belge aynı veri kaynağıyla yeniden birleştirilir, ancak bu sefer kullanılmayan bölgeler özel kodla işlenir.

**Örnek**

Mail Merge'dan sonraki birleştirilmemiş bölgelerin kullanıcı tanımlı kodla nasıl işleneceğini gösterir.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-HandleUnmergedRegionsAfterMailMerge.java" >}}


Kod, **FieldMergingArgs.TableName** özelliği kullanılarak alınan bölgenin adına göre farklı işlemler gerçekleştirir. Belgenize ve bölgelerinize bağlı olarak, işleyiciyi, belgedeki birleştirilmemiş her bölge veya her ikisinin birleşimi için geçerli olan her bölgeye veya koda bağlı mantığı çalıştıracak şekilde kodlayabileceğinizi unutmayın.

**ContactDetails** bölgesinin mantığı, **ContactDetails** bölgesindeki her alanın metnini, veri olmadığını belirten uygun bir mesajla değiştirmeyi içerir. Her alanın adları, **FieldMergingArgs.FieldName** özelliği kullanılarak işleyici içinde eşleştirilir.

**Suppliers** bölgesine, bölgeyi içeren tabloyu işlemek için fazladan kod eklenerek benzer bir işlem uygulanır. Kod, bölgenin bir tabloda yer alıp almadığını kontrol edecektir (daha önce kaldırılmış olabileceğinden). Eğer öyleyse, "Heading 1" gibi bir başlık stiliyle biçimlendirildiği sürece tüm tabloyu ve ondan önceki paragrafı belgeden kaldıracaktır.

**Örnek**

Belgedeki birleştirilmemiş bölgeler için yürütülen IFieldMergingCallback uygulayan bir işleyicide özel mantığın nasıl tanımlanacağını gösterir.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-EmptyRegionsHandler.java" >}}

Yukarıdaki kodun sonucu aşağıda gösterilmiştir. İlk bölgedeki birleştirilmemiş alanlar bilgilendirici metinle değiştirilir ve tablonun ve başlığın kaldırılması belgenin eksiksiz görünmesini sağlar.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-2](how-to-apply-custom-logic-to-unmerged-regions-3.png)


Üst tabloyu kaldıran kod, tablo adı denetimini kaldırarak yalnızca belirli bir bölge yerine kullanılmayan her bölgede çalışacak şekilde de yapılabilir. Bu durumda, bir tablonun içindeki herhangi bir bölge herhangi bir veriyle birleştirilmediyse, hem bölge hem de kapsayıcı tablosu da otomatik olarak kaldırılır.

Birleştirilmemiş bölgelerin nasıl işleneceğini kontrol etmek için işleyiciye farklı kodlar ekleyebiliriz. Bunun yerine işleyicide aşağıdaki kodu kullanmak, bölgedeki sonraki paragraflar kaldırılırken bölgenin ilk paragrafındaki metni yararlı bir iletiye dönüştürür. Bu diğer paragraflar, mesajımızı birleştirdikten sonra bölgede kalacakları şekilde kaldırılır.

Değiştirilen metin, belirtilen metni **FieldMergingArgs.Text** özelliğine ayarlayarak ilk alana birleştirilir. Bu özellikteki metin Mail Merge altyapısı tarafından alana birleştirilir.

Kod, **FieldMergingArgs.FieldValue** özelliğini kontrol ederek bunu yalnızca bölgedeki ilk alan için uygular. Bölgedeki ilk alanın alan değeri "FirstField" ile işaretlenmiştir. Bu, fazladan kod gerekmediği için bu tür bir mantığın birçok bölgede uygulanmasını kolaylaştırır.

**Örnek**

Kullanılmayan bir bölgenin bir mesajla nasıl değiştirileceğini ve fazladan paragrafların nasıl kaldırılacağını gösterir.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ReplaceAnUnusedRegionWithAMessage.java" >}}

Yukarıdaki kod yürütüldükten sonra ortaya çıkan belge aşağıda gösterilmiştir. Kullanılmayan bölge, görüntülenecek kayıt olmadığını belirten bir mesajla değiştirilir.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-3](how-to-apply-custom-logic-to-unmerged-regions-4.png)


Başka bir örnek olarak, orijinal olarak **SuppliersRegion** 'ı işleyen kodun yerine aşağıdaki kodu ekleyebiliriz. Bu, tablo içinde bir ileti görüntüler ve tabloyu belgeden kaldırmak yerine hücreleri birleştirir. Bölge, birden çok hücreye sahip bir tablonun içinde bulunduğundan, tablonun hücrelerinin bir araya getirilmesi ve mesajın ortalanması daha hoş görünür.

**Örnek**

Kullanılmayan bir bölgenin tüm üst hücrelerinin nasıl birleştirileceğini ve tablo içinde bir iletinin nasıl görüntüleneceğini gösterir.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-MergeAllTheParentCellsOfAnUnusedRegion.java" >}}

Yukarıdaki kod yürütüldükten sonra ortaya çıkan belge aşağıda gösterilmiştir.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-4](how-to-apply-custom-logic-to-unmerged-regions-5.png)


Son olarak, **ExecuteCustomLogicOnEmptyRegions** yöntemini çağırabilir ve diğerlerinin otomatik olarak kaldırılacağını belirtirken, işleyici yöntemimizde ele alınması gereken tablo adlarını belirleyebiliriz.

**Örnek**

İşleyici sınıfı aracılığıyla işlenecek yalnızca `ContactDetails` bölgesinin nasıl belirtileceğini gösterir.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-HandleTheContactDetailsRegion.java" >}}

Bu aşırı yüklemeyi belirtilen ArrayList ile çağırmak, yalnızca belirtilen bölgeler için veri satırları içeren veri kaynağını oluşturacaktır. `ContactDetails` bölgesi dışındaki bölgeler işlenmeyecek ve bunun yerine Mail Merge motoru tarafından otomatik olarak kaldırılacaktır. Orijinal işleyicimizdeki kodu kullanan yukarıdaki çağrının sonucu aşağıda gösterilmiştir.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-5](how-to-apply-custom-logic-to-unmerged-regions-6.png)
