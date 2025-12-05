---
title: Python içinde Filigranla çalışma
second_title: Aspose.Words için Python via .NET
articleTitle: Filigran ile çalışma
linktitle: Filigran ile çalışma
description: "Python kullanarak bir belgede filigran oluşturun ve yönetin."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Bu konuda Aspose.Words kullanarak filigranla programlı olarak nasıl çalışılacağı anlatılmaktadır. Filigran, belgedeki metnin arkasında görüntülenen bir arka plan görüntüsüdür. Filigran, [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) sınıfı tarafından temsil edilen bir metin veya resim içerebilir.

{{% alert color="primary" %}}

**Çevrimiçi deneyin**

Bu işlevselliği bizim ile deneyebilirsiniz [Ücretsiz çevrimiçi belge filigranı](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Belgeye Filigran Nasıl Eklenir

Microsoft Word 'te Filigran Ekle komutunu kullanarak bir belgeye kolayca filigran eklenebilir. Aspose.Words belgelere filigran eklemek veya kaldırmak için [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) sınıfını sağlar. Aspose.Words çalışmak için üç olası filigran türünü ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) ve [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) tanımlayan [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) numaralandırmasını sağlar.

### Metin Filigranı Ekle

Aşağıdaki kod örneği, [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/) yöntemini kullanarak [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) tanımlayarak bir belgeye nasıl metin filigranı ekleneceğini gösterir:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### Resim Filigranı Ekle

Aşağıdaki kod örneği, [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/) yöntemini kullanarak [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) tanımlayarak bir belgeye resim filigranının nasıl ekleneceğini gösterir:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

Görüntü filigranı görüntü, dize veya akış olarak eklenebilir.

Filigran, shape sınıfı kullanılarak da eklenebilir. Bir üstbilgi veya altbilgiye herhangi bir şekil veya görüntü eklemek ve böylece akla gelebilecek herhangi bir türde bir filigran oluşturmak çok kolaydır.

Aşağıdaki kod örneği Word belgesine filigran ekler:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

Bu örneğin şablon dosyasını şu adresten indirebilirsiniz: [burada](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Bir Belgeden Filigranı Kaldırma

[Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) sınıfı, filigranı bir belgeden kaldırmak için kaldır yöntemini sağlar.

Aşağıdaki kod örneği, belgelerden filigranın nasıl kaldırılacağını gösterir:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

Filigranlar [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/) sınıf nesnesi kullanılarak eklenirse, filigranı bir belgeden kaldırmak için ekleme sırasında yalnızca filigran şeklinin adını ayarlamanız ve ardından filigran şeklini atanmış bir adla kaldırmanız gerekir.

Aşağıdaki kod örneği, filigran şeklinin adını nasıl ayarlayacağınızı ve belgeden nasıl kaldıracağınızı gösterir:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## Tablo Hücresine Filigran Ekleme

Bazen bir tablonun hücresine filigran / resim eklemeniz ve tablonun dışında görüntülemeniz gerekir, [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/) özelliğini kullanabilirsiniz. Bu özellik, şeklin bir tablonun içinde mi yoksa dışında mı görüntülendiğini gösteren bir bayrak alır veya ayarlar. Bu özelliğin yalnızca [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/) yöntemini kullanarak belgeyi Microsoft Word 2010 için en iyileştirdiğinizde çalıştığını unutmayın.

Aşağıdaki kod örneği, bu özelliğin nasıl kullanılacağını gösterir:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
