---
title: C#'ta Word'ü PDF'ye Dönüştürme
second_title: .NET için Aspose.Words
articleTitle: Belgeyi PDF'ye Çevirme
linktitle: Belgeyi PDF'ye Çevirme
description: "C#'ta Word'ü PDF'ye dönüştürme. DOCX'i PDF'ye dönüştürme için basit kod örnekleri. Tüm Word formatlarını ve resimleri destekler."
type: docs
weight: 10
url: /tr/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Belgeleri bir formattan diğerine kolay ve güvenilir bir şekilde dönüştürme yeteneği Aspose.Words'ün temel özelliğidir. PDF, dönüştürme için en popüler formatlardan biridir – çeşitli platformlarda işleme sırasında belgenin orijinal görünümünü koruyan sabit düzenli bir formattır. "İşleme" terimi Aspose.Words'te bir belgeyi sayfalanmış veya sayfa kavramına sahip bir dosya formatına çevirme işlemini tanımlamak için kullanılır.

## Word Belgesini PDF'ye Dönüştürme

Word'den PDF'ye dönüşüm, birkaç hesaplama aşaması gerektiren oldukça karmaşık bir süreçtir. Aspose.Words düzen motoru, Microsoft Word'ün sayfa düzen motorunun çalışma şeklini taklit ederek PDF çıktı belgelerinin Microsoft Word'de görebileceğinize mümkün olduğunca yakın görünmesini sağlar.

Aspose.Words ile DOC veya DOCX gibi Word formatlarından bir belgeyi Microsoft Office kullanmadan programlı olarak PDF'ye değiştirebilirsiniz. Bu makale, bu dönüşümü nasıl gerçekleştireceğinizi açıklamaktadır.

{{% alert color="primary" %}}

Bir belgedeki sayfa sayısının dönüştürme süresini etkilediğini unutmayın.

{{% /alert %}}

### DOCX veya DOC'u PDF'ye Dönüştürme

Aspose.Words'te DOC veya DOCX belge formatından PDF formatına çevirme çok kolaydır ve sadece iki satır kodla gerçekleştirilebilir:

1. Belgenizi format uzantısıyla birlikte belge adını belirterek yapıcılarından birini kullanarak [Document](https://reference.aspose.com/words/net/aspose.words/document/) nesnesine yükleyin.
1. **Document** nesnesinde [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) yöntemlerinden birini çağırın ve ".PDF" uzantısına sahip bir dosya adı girerek istenen çıktı formatını PDF olarak belirtin.

Aşağıdaki kod örneği, [Save](https://reference.aspose.com/words/net/aspose.words/document/save/) yöntemini kullanarak bir belgeyi DOCX'ten PDF'ye nasıl dönüştüreceğinizi gösterir:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Bu örneğin şablon dosyasını [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx)'dan indirebilirsiniz.

{{% alert color="primary" %}}

Bazen bir belgeyi PDF olarak kaydetmenin sonucunu etkileyebilecek ek seçenekler belirtmek gerekir. Bu seçenekler, PDF çıktısının nasıl görüntüleneceğini belirleyen özellikler içeren [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) sınıfı kullanılarak belirtilebilir.

Aynı teknikle herhangi bir akış-düzen formatı belgeyi PDF formatına değiştirebileceğinizi unutmayın.

{{% /alert %}}

### Farklı PDF Standartlarına Çevirme

Aspose.Words, DOC veya DOCX'i çeşitli PDF format standartlarına (PDF 1.7, PDF 1.5, vb.) dönüştürmeyi desteklemek için [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) numaralandırması sağlar.

Aşağıdaki kod örneği, PDF17 uyumluluğuyla [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) kullanarak bir belgeyi PDF 1.7'ye nasıl dönüştüreceğinizi gösterir:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Resimleri PDF'ye Dönüştürme

PDF'ye dönüştürme Microsoft Word belge formatlarıyla sınırlı değildir. Programlı olarak oluşturulanlar da dahil olmak üzere Aspose.Words tarafından desteklenen herhangi bir format da PDF'ye değiştirilebilir. Örneğin, JPEG, PNG, BMP, EMF veya WMF gibi tek sayfalı resimleri ve TIFF ve GIF gibi çok sayfalı resimleri PDF'ye çevirebiliriz.

Aşağıdaki kod örneği, JPEG ve TIFF resimlerini PDF'ye nasıl değiştireceğinizi gösterir:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Bu kodun çalışması için projenize Aspose.Words ve `System.Drawing` referansları eklemeniz gerekir.

## PDF Çıktı Boyutunu Azaltma

PDF'ye kaydederken çıktıyı optimize etmek isteyip istemediğinizi belirtebilirsiniz. Bunu yapmak için [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) bayrağını true olarak ayarlamanız gerekir, ardından gereksiz iç içe geçmiş ve boş tuvaller kaldırılır, aynı biçimlendirmeye sahip komşu glifler birleştirilir.

Aşağıdaki kod örneği çıktının nasıl optimize edileceğini gösterir:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

**OptimizeOutput** özelliğini kullanmak içerik görüntülemenin doğruluğunu etkileyebilir.

{{% /alert %}}

## Ayrıca Bakınız

- [İşleme](/words/tr/net/rendering/) makalesinde sabit sayfa ve akış-düzen formatları hakkında daha fazla bilgi
- [Sabit Sayfa Formatına Dönüştürme](/words/net/converting-to-fixed-page-format/#what-is-a-page-layout) makalesinde sayfa düzeni hakkında daha fazla bilgi
- [PDF'ye Çevirirken İşleme Seçeneklerini Belirtme](/words/tr/net/specify-rendering-options-when-converting-to-pdf/) makalesinde `PdfSaveOptions` sınıfını kullanma hakkında daha fazla bilgi
- [PDF/A ve PDF/UA'ya Dönüştürme Özelliklerini Öğrenin](/words/tr/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) makalesinde Aspose.Words'ün desteklediği PDF standardı ve PDF standartları için ilgili ISO'ları açıklayan
- [Hangi PDF Standardının Seçilmesi Daha İyi](/words/tr/net/which-pdf-standard-is-better-to-choose/) makalesinde hangi PDF standartlarının hangi durumlar için mantıklı olduğunu belirleme

- [PDF/A veya PDF/UA ile Çalışma](/words/tr/net/working-with-pdfa-or-pdfua/) makalesinde PDF/A ve PDF/UA formatlarında belge içeriği gereksinimlerini açıklayan – öncelikle yapı ve yazı tipi gereksinimleri

- [PDF/A ve PDF/UA'ya Kaydederken Erişilebilirlik Sorunları Uyarıları](/words/tr/net/warnings-when-saving-to-pdfa-and-pdfua/) makalesinde PDF/A ve PDF/UA'nın ne tür içerik erişilebilirlik gereksinimlerini getirdiğini açıklayan
