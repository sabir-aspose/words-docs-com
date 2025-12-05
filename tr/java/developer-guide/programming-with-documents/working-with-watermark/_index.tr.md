---
title: Java içinde Filigranla çalışma
second_title: Aspose.Words için Java
articleTitle: Filigran ile çalışma
linktitle: Filigran ile çalışma
type: docs
description: "Java kullanarak filigran manipülasyonunu belgeleyin."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/java/working-with-watermark/
timestamp: 2025-04-22-08-07-04
---

Bu konuda Aspose.Words kullanarak filigranla programlı olarak nasıl çalışılacağı anlatılmaktadır. Filigran, belgedeki metnin arkasında görüntülenen bir arka plan görüntüsüdür. Filigran, [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) sınıfı tarafından temsil edilen bir metin veya resim içerebilir.

{{% alert color="primary" %}}

**Çevrimiçi deneyin**

Bu işlevselliği bizim ile deneyebilirsiniz [Ücretsiz çevrimiçi belge filigranı](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Belgeye Filigran Ekleme

Microsoft Word 'de Filigran Ekle komutunu kullanarak bir belgeye kolayca filigran eklenebilir. Aspose.Words belgelere filigran eklemek veya kaldırmak için [watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) sınıfını sağlar. Aspose.Words çalışmak için üç olası filigran türünü (Metin, Resim ve Hiçbiri) tanımlayan [WatermarkType ](https://reference.aspose.com/words/java/com.aspose.words/watermarktype/) numaralandırmasını sağlar.

### Metin Filigranı Ekle

Aşağıdaki kod örneği, [SetText](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setText-java.lang.String) yöntemini kullanarak [TextWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/textwatermarkoptions/) tanımlayarak bir belgeye nasıl metin filigranı ekleneceğini gösterir:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddTextWatermarkWithSpecificOptions.java" >}}

### Resim Filigranı Ekle

Aşağıdaki kod örneği, [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.awt.image.BufferedImage) yöntemini kullanarak [ImageWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/imagewatermarkoptions/) tanımlayarak bir belgeye resim filigranının nasıl ekleneceğini gösterir:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddImageWatermarkWithSpecificOptions.java" >}}

Görüntü filigranı görüntü, dize veya akış olarak eklenebilir.

Filigran, shape sınıfı kullanılarak da eklenebilir. Bir üstbilgi veya altbilgiye herhangi bir şekil veya görüntü eklemek ve böylece akla gelebilecek herhangi bir türde bir filigran oluşturmak çok kolaydır.

Aşağıdaki kod örneği Word belgesine filigran ekler:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-AddWatermarkToADocument-AddWatermarkToADocument.java" >}}

{{% alert color="primary" %}}

Bu örneğin örnek dosyasını şu adresten indirebilirsiniz [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Document.doc).

{{% /alert %}}


## Bir Belgeden Filigranı Kaldırma

[Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) sınıfı, filigranı bir belgeden kaldırmak için `Remove` yöntemini sağlar.

Aşağıdaki kod örnekleri, belgelerden filigranın nasıl kaldırılacağını gösterir:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-RemoveWatermarkFromDocument.java" >}}

Filigranı bir belgeden kaldırmak için, ekleme sırasında yalnızca filigran şeklinin adını ayarlamanız ve ardından filigran şeklini atanmış bir adla kaldırmanız gerekir.

Aşağıdaki kod örneği, filigran şeklinin adını nasıl ayarlayacağınızı ve belgeden nasıl kaldıracağınızı gösterir:

{{< highlight csharp >}}

// Set name to be able to remove it afterwards
watermark.Name("WaterMark");
{{< /highlight >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-RemoveWatermark-RemoveWatermark.java" >}}

## Tablo Hücresine Filigran Ekleme

Bazen bir tablonun hücresine filigran / resim eklemeniz ve tablonun dışında görüntülemeniz gerekir, [IsLayoutInCell](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#isLayoutInCell-boolean) özelliğini kullanabilirsiniz. Bu özellik, şeklin bir tablonun içinde mi yoksa dışında mı görüntülendiğini gösteren bir bayrak alır veya ayarlar. Bu özelliğin yalnızca [OptimizeFor](https://reference.aspose.com/words/java/com.aspose.words/compatibilityoptions/#optimizeFor-int) yöntemini kullanarak belgeyi Microsoft Word 2010 için en iyileştirdiğinizde çalıştığını unutmayın.

Aşağıdaki kod örneği, bu özelliğin nasıl kullanılacağını gösterir:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-Shapes-WorkingWithShapes-SetShapeLayoutInCell.java" >}}
