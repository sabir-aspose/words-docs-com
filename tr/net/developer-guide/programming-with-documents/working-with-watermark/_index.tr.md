---
title: C# içinde Filigranla çalışma
second_title: Aspose.Words için .NET
articleTitle: Filigran ile çalışma
linktitle: Filigran ile çalışma
description: "C# kullanarak filigran manipülasyonunu belgeleyin."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Bu konuda Aspose.Words kullanarak filigranla programlı olarak nasıl çalışılacağı anlatılmaktadır. Filigran, belgedeki metnin arkasında görüntülenen bir arka plan görüntüsüdür. Filigran, [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) sınıfı tarafından temsil edilen bir metin veya resim içerebilir.

{{% alert color="primary" %}}

**Çevrimiçi deneyin**

Bu işlevselliği bizim ile deneyebilirsiniz [Ücretsiz çevrimiçi belge filigranı](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Belgeye Filigran Ekleme

Microsoft Word 'de Filigran Ekle komutunu kullanarak bir belgeye kolayca filigran eklenebilir. Aspose.Words belgelere filigran eklemek veya kaldırmak için [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) sınıfını sağlar. Aspose.Words çalışmak için üç olası filigran türünü (Metin, Resim ve Hiçbiri) tanımlayan [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/) numaralandırmasını sağlar.

### Metin Filigranı Ekle

Aşağıdaki kod örneği, [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext) yöntemini kullanarak [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) tanımlayarak bir belgeye nasıl metin filigranı ekleneceğini gösterir:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Resim Filigranı Ekle

Aşağıdaki kod örneği, [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage) yöntemini kullanarak [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) tanımlayarak bir belgeye resim filigranının nasıl ekleneceğini gösterir:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Görüntü filigranı görüntü, dize veya akış olarak eklenebilir.

Filigran, shape sınıfı kullanılarak da eklenebilir. Bir üstbilgi veya altbilgiye herhangi bir şekil veya görüntü eklemek ve böylece akla gelebilecek herhangi bir türde bir filigran oluşturmak çok kolaydır.

Aşağıdaki kod örneği Word belgesine filigran ekler:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Bu örneğin örnek dosyasını şu adresten indirebilirsiniz [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Bir Belgeden Filigranı Kaldırma

[Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) sınıfı, filigranı bir belgeden kaldırmak için kaldır yöntemini sağlar.

Aşağıdaki kod örneği, belgelerden filigranın nasıl kaldırılacağını gösterir:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Filigranlar [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/) sınıf nesnesi kullanılarak eklenirse, filigranı bir belgeden kaldırmak için ekleme sırasında yalnızca filigran şeklinin adını ayarlamanız ve ardından filigran şeklini atanmış bir adla kaldırmanız gerekir.

Aşağıdaki kod örneği, filigran şeklinin adını nasıl ayarlayacağınızı ve belgeden nasıl kaldıracağınızı gösterir:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Tablo Hücresine Filigran Ekleme

Bazen bir tablonun hücresine filigran / resim eklemeniz ve tablonun dışında görüntülemeniz gerekir, [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/) özelliğini kullanabilirsiniz. Bu özellik, şeklin bir tablonun içinde mi yoksa dışında mı görüntülendiğini gösteren bir bayrak alır veya ayarlar. Bu özelliğin yalnızca [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/) yöntemini kullanarak belgeyi Microsoft Word 2010 için en iyileştirdiğinizde çalıştığını unutmayın.

Aşağıdaki kod örneği, bu özelliğin nasıl kullanılacağını gösterir:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
