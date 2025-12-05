---
title: Yenilikler
second_title: Aspose.Words için Python via .NET
articleTitle: İçerideki yenilikler Aspose.Words için Python via .NET
linktitle: İçerideki yenilikler Aspose.Words için Python via .NET
type: docs
description: "Aspose.Words için Python via .NET her gün genişler ve gelişir. Bu sayfada, ürünün devasa ve en ilginç özellikleri hakkında bilgi edinebilirsiniz."
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-06-23-21-02-49
---

Bu sayfa, son sürümlerde tanıtılan en ilginç yeni Aspose.Words özellikleri açıklamaktadır.

## Aspose.Words için Python via .NET 25.5, 25.6

Aspose.Words 25.5, yeni stil seçenekleriyle grafik özelleştirmesini geliştirir ve boş paragrafların nasıl işleneceği üzerinde kontrol sunarak Markdown dışa aktarmayı geliştirir.

Aspose.Words 25.6 gelişmiş görüntü dışa aktarma seçenekleri, geliştirilmiş MathML işleme ve daha iyi grafik gösterimi sunarak işleme hassasiyetini ve görselleştirme özelliklerini geliştirir.

### Belgeleri Dönüştürme, Yükleme ve Kaydetme

#### Boş Paragrafları Markdown <sup>25.5'e Aktar</sup>

**MarkdownEmptyParagraphExportMode** numaralandırma ve **empty_paragraph_export_mode** özelliği eklenerek boş paragrafların Markdown'ye nasıl dışa aktarılacağını kontrol etme yeteneği getirildi.

#### Çok Sayfalı Belgeleri Raster Görüntü Biçimlerine Dışa Aktarma <sup>25.6</sup>

Çok sayfalı belgeleri raster görüntü biçimlerine (PNG ve JPEG gibi) [customizable layouts](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) (Yatay, Dikey veya Izgara) ile dışa aktarma özelliği, görüntü dışa aktarma işlevi genişletilerek tanıtıldı.

### İşleme

#### Grafik Stilini Ayarlama <sup>25.5</sup>

Grafik stilini ayarlama yeteneği, **ChartStyle** numaralandırma ve **style** özelliği eklenerek tanıtıldı.

#### MathML İfadelerinde Bağlayıcı Satırları Oluşturma <sup>25.6</sup>

Bağlayıcı satırların MathML ifadelerde oluşturulması, matematiksel formüllerin daha doğru ve görsel olarak tutarlı görüntülenmesini sağlamak için uygulanmıştır.

#### Şelale Çizelgeleri için Efsane Oluşturma <sup>25.6</sup>

["Waterfall" charts](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriestype/) için efsanelerin oluşturulması, veri şeffaflığının artırılması ve bu grafiklerin yorumlanabilirliğinin iyileştirilmesi tanıtıldı.

### Diğer

* Birden çok eğik çizgi içeren matematiksel formülleri sarma yeteneği geliştirilerek düzen netliği ve formül okunabilirliği iyileştirildi. <sup>25.6</sup>

{{% alert color="primary" %}}

Hakkında daha fazla bilgi edinin [Aspose.Words Python via .NET 25.5 Sürüm Notları için](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-5-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words Python via .NET 25.6 Sürüm Notları için](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words .NET üzerinden Python için 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1, AI destekli dilbilgisi denetimini sunar ve HTML, SVG ve Markdown biçimleri için gelişmiş seçeneklerle belge kaydetmeyi geliştirir.

Aspose.Words 25.2 Anthropic AI modellerle metin özetlemeyi tanıtır, MsWorks biçim desteği ekler, tipografik kontrolü geliştirir ve PDF yapı ve liste işlemeyi geliştirir.

Aspose.Words 25.3 UpdateAmbiguousTextFont özelliğine sahip AI destekli bir dilbilgisi denetleyicisini ve yazı tipi seçimini geliştirir ve ayrıca PDF eklerin dışa aktarılmasını geliştirir.

Aspose.Words 25.4 yeni kağıt boyutları için destek sunar, gelişmiş HTML dışa aktarma kontrolünü etkinleştirir ve filigran işlemeyi geliştirir.

### AI -güçlendirilmiş Özellikler

#### Belge AI Dilbilgisi Denetimi

* Sağlanan belgenin dilbilgisini OpenAI üretici modelleri kullanarak kontrol etme yeteneği, yeni bir [check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/) yöntemi eklenerek tanıtıldı. <sup>25.1</sup>
* AI destekli Dilbilgisi Denetimi özelliği, [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/) numaralandırmasında bulunan tüm modelleri destekleyecek şekilde güncellendi. <sup>25.3</sup>

#### Anthropic Üretici Dil Modellerini Kullanarak Özetleme <sup>25.2</sup>

Anthropic üretici dil modellerini kullanarak metin özetlemesi, yeni bir genel sınıf [AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/) getirilerek etkinleştirildi.

### Desteklenen Biçimler <sup>25.2</sup>

25.2 sürümünden başlayarak, Microsoft Works belgeleri için yeni MsWorks yükleme biçimiyle uyumluluk eklendi.

### Belgeleri Dönüştürme, Yükleme ve Kaydetme

#### HTML ve SVG Biçimlerine Geliştirilmiş Kaydetme <sup>25.1</sup>

HTML ve SVG biçimlerine kaydetme, hem [HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/) hem de [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) sınıflarına **id_prefix** ve **remove_java_script_from_links** özellikleri eklenerek geliştirilmiştir.

#### Kaydederken Görüntü Çözünürlüğünü ve OfficeMath Çıkış Modunu Markdown <sup>25.1 olarak Ayarlayın</sup>

* Görüntü çözünürlüğünü ayarlamak için [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) sınıfına yeni bir [image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/) seçeneği eklendi.
* OfficeMath çıktı modunu ayarlamak için [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) sınıfına yeni bir [office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/) seçeneği ve [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/) numaralandırması eklendi ve eklendi.

### İşleme

#### Geliştirilmiş Tipografik Kontrol <sup>25.2</sup>

Geliştirilmiş tipografik kontrol için [number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/) özelliği eklendi.

#### Belirsiz Karakterler için Yazı Tipi Seçimini Denetleme <sup>25.3</sup>

Kullanılan karakter koduna göre yazı tipi seçimini denetlemek için [SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/) sınıfına yeni bir genel özellik [update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/) eklendi.

#### Kağıt Boyutu Seçenekleri <sup>25.4</sup>

JIS B4 ve JIS B5 kağıt boyutlarını kullanma yeteneği, [PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/) numaralandırmasına yeni değerler eklenerek tanıtıldı.

#### HTML Çıkış Kontrolü <sup>25.4</sup>

HTML dışa aktarma sırasında JavaScript köprüsünden URLs kaldırma özelliği, [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/) özelliği eklenerek tanıtıldı.

### Diğer

* PDF mantıksal yapı TOA, BIBLIOGRAPHY ve INDEX alanları desteği ile geliştirilmiştir. <sup>25.2</sup>
* Geliştirilmiş liste işleme için [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate) yöntemi tanıtıldı. <sup>25.2</sup>
* PDF eklerin dışa aktarımını iyileştirmek için **EmbedAttachments** yerine [attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/) yeni bir özellik eklendi. Ayrıca, PDF/A sürüm eklerini desteklemek için [PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/) numaralandırmasına yeni değerler eklenmiştir. Ek olarak, ekler artık şifreleme ile desteklenmektedir. <sup>25.3</sup>
* [SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions) yöntemine yeni bir aşırı yük eklenerek bir akıştan görüntü filigranı ayarlama özelliği tanıtıldı. <sup>25.4</sup>

{{% alert color="primary" %}}

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 25.1 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 25.2 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 25.3 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 25.4 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words Python için .NET üzerinden 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 group shape ekleme ve StructuredDocumentTag ekleme işlemlerini DocumentBuilder aracılığıyla tanıtır, mezuniyetlerle radyal grafik oluşturmayı geliştirir, XAdES-EPES desteğiyle dijital imzaları geliştirir, Markdown altı çizili tanıma ekler ve dipnot / sonnot ayırıcılarına erişim sağlar.

Aspose.Words 24.10, CommandButton oluşturma, yeni şekil görünürlüğü kontrolü, group shapes yeteneği, tablolar için geliştirilmiş Markdown dışa aktarma, Pie ve Doughnut grafikler için grafik biçimlendirme, daha iyi Bıg5 kodlama işleme ve eski sürümler için destek ile gelişmiş ActiveX kontrol desteği sunar Tayvanlı yazı tipleri.

Aspose.Words 24.11, AI destekli belge özetleme, gelişmiş oluşturma seçenekleri, belge özelliklerine geliştirilmiş erişim ve ActiveX altyazı denetimini sunar.

Aspose.Words 24.12 özelleştirilebilir veri etiketi yerleşimi, Google AI destekli metin çevirisi ve geliştirilmiş yeni LowCode işleme sınıfları sunar.

### AI -güçlendirilmiş Özellikler

#### OpenAI ve Google <sup>24.11 Kullanarak Belge Özetleme</sup>

**OpenAI** ve **Google** üretici dil modellerini kullanarak belge özetleme desteği, genel üyeleriyle [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) ad alanı eklenerek entegre edilmiştir.

#### Google'ın üretken dil modellerini kullanarak metin çevirisi <sup>24.12</sup>

Google'ın üretken dil modellerini kullanarak metni çevirme yeteneği, [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) ad alanına [translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/) yöntemi ve [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) numaralandırması eklenerek Aspose.Words'te uygulanmıştır.

### Low Code <sup>24.12</sup>

Yeni LowCode sınıflar gibi [Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) vb. belge işleme için basitlik ve esneklik arasında mükemmel dengeyi sağlayan bir dizi yöntem sunan tanıtıldı.

### Oluşturma ve Yazdırma

#### Radyal Grafiklerde Mezuniyetler <sup>24.9</sup>

Radyal grafiklerde mezuniyetlerin oluşturulması uygulanmıştır.

#### CommandButton ActiveX Kontroller <sup>24.10</sup>

CommandButton ActiveX denetimleri oluşturma yeteneği, yeni bir genel yöntem [insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/) ve yeni bir genel sınıf [Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/) eklenerek tanıtıldı.

#### Kontrol Şekli Görünürlüğü <sup>24.10</sup>

Şekillerin görünürlüğünü denetlemek için yeni bir genel özellik [hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/) eklendi.

#### Pie ve Doughnut Grafiklerindeki Değişiklikler <sup>24.10</sup>

Pie ve Doughnut grafiklerini biçimlendirmek için birkaç yeni genel özellik eklendi.

#### PDF Seçim Formu Alanı Kenarlıklarının Oluşturulmasını Denetleme <sup>24.11</sup>

PDF seçim formu alanı kenarlıklarının oluşturulmasını denetlemek için yeni bir genel seçenek [render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/) eklenerek yeni bir seçenek uygulandı.

#### Grafik Verileri için Biçim Kodlarını Alın ve Ayarlayın <sup>24.11</sup>

Grafik verileri için biçim kodları alma ve ayarlama yeteneği, [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/) ve [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/) sınıflarında [format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/) özelliği uygulanarak eklenmiştir.

#### Histogram Grafiklerini Kutular ve Etiketlerle Oluşturma <sup>24.11</sup>

Histogram grafik oluşturma, belirli sayıda kutu ve etikete izin verilerek geliştirilmiştir.

#### Veri Etiketlerinin Yerleşimini Özelleştirme <sup>24.12</sup>

Veri etiketlerinin yerleşimini özelleştirme yeteneği, [ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/) ve [ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/) sınıflarına yeni özellikler eklenerek eklenmiştir.

### Belgeleri Dönüştürme, Yükleme ve Kaydetme

#### Markdown Dosyaları <sup>24.9 Yüklerken Biçimlendirmenin Altını Çizin</sup>

Markdown belgeleri yüklerken altı çizili biçimlendirmeyi tanıma seçeneği, yeni bir genel özellik [import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/) eklenerek eklenmiştir.

#### Markdown <sup>24.10'e kaydederken tabloları HTML olarak dışa aktarma</sup>

Belgeleri Markdown biçimine kaydederken tabloları HTML olarak dışa aktarma seçeneği, yeni bir genel özellik [export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/) ve bir numaralandırma [MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/) eklenerek uygulanmıştır.

#### Güncellenmiş Mantıksal Yapı <sup>24.11 ile PDF dışa Aktar</sup>

PDF dışa aktarma, tablo başlığı özelliklerini PDF mantıksal yapı öğesi başlıkları olarak ekleyerek geliştirilmiştir.

### Dijital İmzalar

#### Belgeleri XAdES-EPES <sup>24.9 ile imzalayın</sup>

XAdES-EPES düzey XML-DSig imzalı belgeleri imzalama yeteneği, yeni bir genel özellik [xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/) ve yeni bir genel numaralandırma [XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/) eklenerek kullanılmıştır.

### Diğer

* Group shapes 'e yeni bir genel yöntem [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/) eklendi. <sup>24.9</sup>
* Bir belgeye **StructuredDocumentTags** eklemek için yeni bir genel yöntem [insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/) eklendi. <sup>24.9</sup>
* Dipnot / sonnot ayırıcılarına genel erişim, birkaç genel sınıf ve özellik eklenerek sağlanmıştır. <sup>24.9</sup>
* Tek tek şekilleri group shapes birlikte gruplama ve hem şekilleri hem de group shapes 'i doğrudan gruplama yeteneği, [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist) yöntemi eklenerek tanıtıldı. <sup>24.10</sup>
* TrueType cmap tabloları için Bıg5 kodlama işlemi geliştirildi. <sup>24.10</sup>
* Eski Tayvanlı yazı tipleri için destek geliştirildi. <sup>24.10</sup>
* Genişletilmiş belge özelliklerine erişmek için [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/) sınıfına salt okunur özellikler eklenmiştir. <sup>24.11</sup>
* ActiveX denetimleri için altyazı ayarlama, [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/) özelliğine yeni bir genel ayarlayıcı eklenerek etkinleştirildi. <sup>24.11</sup>

{{% alert color="primary" %}}

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.9 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.10 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.11 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.12 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words .NET üzerinden Python için 24,5, 24,6, 24,7, 24,8

Aspose.Words 24.5 derlemeler için seçenekleri genişletir, oluşturma yeteneklerini geliştirir ve diğer bazı seçenekleri genişletir.

Aspose.Words 24.6 işleme seçeneklerini iyileştirir, arama ve karşılaştırma işlevselliğini geliştirir ve diğer birçok özelliği genişletir.

Aspose.Words 24.7 ActiveX ile çalışma şeklinizi değiştirir, oluşturma yeteneklerini genişletir ve Markdown ve XLSX biçimlerine dışa aktarır.

Aspose.Words 24.8 eksen etiketleri üzerinde hassas kontrolle grafik özelleştirmesini geliştirir, yazı tipi yönetimini genişletir, belge yapısı işlemeyi geliştirir ve HTML / XAML dışa aktarma, PDF işlevsellik, belge dönüştürme ve dijital imzalar için yeni özellikler ekler.

### Desteklenen Formatlar

24.7 sürümünden başlayarak, engelli kullanıcıların erişilebilirliğini sağlamak için PDF/UA-2 sürümüne dışa aktarma desteklenir.

### Oluşturma ve Yazdırma

#### Grafiklerdeki, Şekillerdeki ve DrawingML <sup>24.5'deki Değişiklikler</sup>

* DrawingML görüntülerle sınırlı önceki işlevleri genişleten SVG grafikler için efekt oluşturma uygulandı.
* [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/) ve [ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/) sınıfları ve [series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/) özelliği eklenerek birleşik grafikler oluşturma ve seri grupları içinde boşluk genişliği, üst üste binme ve kabarcık ölçeği gibi özellikleri ayarlama desteği getirildi.
* Şekillerin SoftEdge etkisini değiştirme işlevi, [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/) sınıfı eklenerek uygulanmıştır.
* **AdjustmentCollection** ve **Adjustment** genel sınıfları ve [adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/) özelliği eklenerek şekillerin değerlerini ayarlama özelliğini değiştirme özelliği uygulanmıştır.

#### Çizelge, Şekil ve Çizimdeki Değişiklikler <sup>24.6</sup>

- Grafik yetenekleri geliştirildi. Artık aşağıdakiler de dahil olmak üzere daha geniş bir grafik yelpazesi oluşturabilirsiniz *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* grafikler, *Box & Whisker* grafikler, *Waterfalls* ve *Funnels*. Bu, verilerinizi daha çeşitli ve bilgilendirici bir şekilde görselleştirmenizi sağlar.
- Gölge biçimlendirme için renk kontrolü geliştirildi. Gölge renklerine erişerek belgelerinizin görünümü üzerinde daha hassas kontrol sahibi olabilirsiniz.
- Arka plan oluşturma için performans artışı iyileştirildi. Yerel döşeme teknolojisi sayesinde küçük öğeler içeren arka planların oluşturulmasını önemli ölçüde hızlandırabilirsiniz.
- Şekiller için gerçekçi degradeler eklendi. Artık daha parlak bir görünüm için Microsoft Word görsel stilini taklit ederek doğrusal olmayan degradelere sahip DML şekiller oluşturabilirsiniz.

#### Grafik Veri Etiketi Özelleştirme <sup>24.7</sup>

**Orientation** ve **Rotation** gibi grafik veri etiketlerini özelleştirme yeteneği eklendi.

#### Liste Seviyeleri için Özel Numara Stili <sup>24.7</sup>

[custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/) genel mülkü için bir ayarlayıcı eklendi. Artık liste seviyeleri için özel bir numara stili tanımlayabilirsiniz.

#### ActiveX <sup>24.7 ile çalışmadaki değişiklikler</sup>

- ActiveX nesnelerinin özellikleri artık değiştirilebilir, böylece davranışları üzerinde daha fazla kontrol sahibi olursunuz.
- Dinamik etkileşimi etkinleştirmek için radyo düğmesi ActiveX kontrolünün değerini değiştirme yeteneği eklendi.
- Bir ActiveX checkbox öğesini "işaretli" veya "işaretlenmemiş" olarak değiştirme yeteneği eklendi.

#### Grafik Ekseni Üzerinde Kontrol İşaret Etiketleri Yönlendirme ve Döndürme <sup>24.8</sup>

Daha rahat grafik özelleştirmesi için grafik ekseni onay etiketlerinin yönlendirilmesi ve döndürülmesi üzerinde hassas kontrol eklendi – [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) sınıfı yeni [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) ve [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/) özellikleriyle genişletildi.

#### Ters Eğik Çizgiyi Yen İşareti <sup>24.8 ile Değiştirme</sup>

Ters eğik çizgi karakterini Yen işareti ile değiştirmek için geriye dönük uyumlu HTML ve XAML dışa aktarma geliştirildi. Bunu başarmak için **replace_backslash_with_yen_sign** özelliği [HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/) ve [XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/) sınıflarına eklenmiştir.

#### PDF <sup>24.8'a Dışa Aktarırken SDT Etiketlerini Form Alanı Adları Olarak Kullanma</sup>

PDF SDT etiketlerini form alan adları olarak kullanma desteğiyle dışa aktarma, [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) sınıfına yeni bir [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) özelliği eklenerek geliştirilmiştir.

### Belgeleri Dönüştürme, Yükleme ve Kaydetme

#### Bağlantıları Markdown Biçimine <sup>24.7 Dışa Aktarma</sup>

Bağlantıların Markdown biçiminde dışa aktarılmasını kontrol etme yeteneği, [link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/) özelliğinin uygulanmasıyla eklenmiştir.

#### LowCode 24.8 <sup>24.8</sup>

Çeşitli belge türlerini tek bir kod satırıyla dönüştürmek için bir dizi yöntem sağlamak üzere tasarlanmış yeni bir [LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/) sınıfı tanıtıldı.

### Ara ve Karşılaştır

#### Gelişmiş Karşılaştırma Seçenekleri <sup>24.6</sup>

Geliştirilmiş karşılaştırma işlevselliği ile veri analizi iş akışlarını kolaylaştırma yeteneği eklendi. Buna yeni bir [ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/) seçeneği ve gelişmiş karşılaştırmalar için yeniden tasarlanmış bir arayüz dahildir.

### Diğer

* Bir belgedeki boş sayfaları ortadan kaldırma işlevi [remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/) yöntemi eklenerek uygulanmıştır. <sup>24.5</sup>
* Belge yüklemeden VBA makro olup olmadığını denetleme yeteneği, [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/) özelliği eklenerek sağlanmıştır. <sup>24.5</sup>
* LINQ Raporlama Altyapısını kullanarak bir belge eklerken kaynak numaralandırmanın tutulması artık destekleniyor. <sup>24.5</sup>
* Yeni bir [date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/) özelliği eklendi – bu, yorumlar için daha kesin bir zaman damgası sağlayarak organizasyonu ve izlenebilirliği iyileştirir. <sup>24.6</sup>
* XLSX biçimine kesintisiz dışa aktarma için datetime biçimi artık otomatik olarak algılanır. <sup>24.7</sup>
* Bir VBA projesinin korunup korunmadığını doğrulamanıza izin veren [is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/) ortak mülkü eklenmiştir. <sup>24.7</sup>
* [FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/) ve [PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/) sınıflarına **embedding_licensing_rights** özelliği eklenerek yazı tipi bilgileri genişletildi. <sup>24.8</sup>
* Belge yapısıyla daha doğru çalışmak için filigranları korurken bölüm üstbilgilerini ve altbilgilerini verimli bir şekilde temizlemenin bir yolu eklendi. Bölüm üstbilgilerini ve altbilgilerini temizlemek için yeni genel yöntemi [clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default) kullanın. <sup>24.8</sup>
* XPS belgelerin [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/) kullanılarak dijital olarak imzalanması etkinleştirildi - bu amaçla yeni bir özellik [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/) eklendi. <sup>24.8</sup>

{{% alert color="primary" %}}

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.5 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.6 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.7 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.8 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words Python için .NET üzerinden 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 kontur renklerini yönetme deneyimini geliştirir, OLE nesneleri geliştirir ve yeni bir `Bibliography Sources` herkese açık API sunar.

Aspose.Words 24.2 genişletilmiş Grafikler API ve stil yönetimi. Aspose.Words'in bu sürümü ayrıca oluşturma sırasında SvgSaveOptions belirtme, Markdown dosyalarını daha esnek kontrol yükleme ve dipnotlar ve sonnotlar için referans metni ile çalışma özelliğini de tanıttı.

Aspose.Words 24.3 yeni bir TIFF Okuyucu / Yazıcı ve WMF meta dosyaları için ikili raster işlemlerinin Öykünmesini sunar. Aspose.Words 24.3 ayrıca Grafikleri genişletmeye devam ediyor API.

Aspose.Words 24.4 kaydetme biçimlerini, bazı oluşturma seçeneklerini geliştirir ve dijital imzalarla çalışmayı geliştirir.

### Desteklenen Biçimler <sup>24.4</sup>

Modern **WebP** görüntü formatı artık şu şekilde destekleniyor: Aspose.Words için .NET Framework 4.6.2 ve daha yükseğe. Artık WebP görüntüleri okuyabilir ve belgelere ekleyebilir, ayrıca görüntüleri WebP biçiminde kaydedebilirsiniz.

WebP'ün şu anda yalnızca .NET Standard ve .NET Framework v 4.6.2 ve üzeri sürümlerde mevcut olduğunu lütfen unutmayın.

### Oluşturma ve Yazdırma

#### Kontur Renk Kontrolü <sup>24.1</sup>

[Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) sınıfı, kontur renklerini yönetmekle ilgili bir dizi yeni genel özellik ile genişletildi: [fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/) ve [back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/), [fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/) ve [back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### DrawingML Grafikler API Uzantı <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** genişletilmeye devam ediyor.

#### @font-face Kurallarında Bildirilen Fontları Göm <sup>24.4</sup>

@font-face kurallarında bildirilen fontları, yeni bir [support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/) özelliği eklenerek ortaya çıkan belgenin font tanımlarına gömme özelliği eklendi.

#### Işıma ve Yansıma Biçimlendirmesiyle Çalışın <sup>24.4</sup>

Bir çizim nesnesi için ışıma ve yansıma biçimlendirmesiyle çalışma yeteneği uygulanmıştır.

### Belgeleri Yükleme ve Kaydetme

#### Oluşturma Sırasında SvgSaveOptions belirtin <sup>24.2</sup>

Oluşturma sırasında [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) belirtme özelliği [ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/) kullanılarak eklenmiştir.[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) ve [OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) yöntemler.

#### Markdown dosyaları <sup>24.2 yüklerken Boş Satırları Koru</sup>

Markdown dosyaları yüklerken boş satırları koruma özelliği eklendi.

#### Yeni Bir TIFF Okuyucu / Yazar <sup>24.3</sup>

Aspose.Words için yeni bir TIFF okuyucu / yazar geliştirildi. Aspose.Words için .NET 24.3 JPEG ve Eski JPEG sıkıştırma türlerine sahip TIFF görüntüleri okumak için destek eklendi ve ayrıca okuma ve yazma işlemlerinin kalitesini önemli ölçüde iyileştirdi.

### Diğer

* `TextBox` OLE denetiminin metnini değiştirme özelliği, yeni **TextBoxControl** sınıfına yeni bir **Text** özelliği eklenerek kullanıma sunulmuştur. <sup>24.1</sup>
* Kaynakça Kaynakları genel API, yeni sınıfları ve numaralandırmalarıyla yeni bir ad alanı [Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/) ekleyerek ve [Document](https://reference.aspose.com/words/python-net/aspose.words/document/) sınıfına yeni bir [bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/) özelliği ekleyerek uygulandı. <sup>24.1</sup>
* Gelişmiş stil yönetimi için [Style](https://reference.aspose.com/words/python-net/aspose.words/style/) sınıfına yeni genel özellikler [priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/), [unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/) ve [semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/) eklenmiştir. <sup>24.2</sup>
* Dipnotlar ve sonnotlar için gerçek referans işareti metnini alma işlevi [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/) özelliği ve [update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default) yöntemi ile geliştirilmiştir. <sup>24.2</sup>
* WMF meta dosyaları için ikili raster işlemlerinin öykünmesi uygulandı. <sup>24.3</sup>
* **SaveOptions** içindeki belgeler için imza seçeneklerini tanımlama yeteneği, yeni genel üyelerle birlikte yeni bir [DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/) sınıfı eklenerek ve [OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/) ve [OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/) sınıflarına yeni özellikler eklenerek etkinleştirildi. <sup>24.4</sup>

{{% alert color="primary" %}}

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.1 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.2 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.3 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 24.4 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words Python için .NET üzerinden 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 oluşturma seçeneklerini, meta dosyası oluşturma öykünmesini ve markdown kaydetme seçeneklerini genişletir.

Aspose.Words 23.10 oluşturmayı iyileştirir, belgeleri yükleme ve kaydetme seçeneklerini genişletir ve kullanıcıların belgeleri yeni yollarla birleştirmesine olanak tanır.

Aspose.Words 23.11 grafik göstergesindeki düzeltmeler, XLSX biçim ve yazı tipleriyle çalışmayı ek seçeneklerle geliştirir.

Aspose.Words 23.12, PDF ve OOXML belgelerle çalışmak için yeni özellikler ve numaralandırmaların yanı sıra WebP görüntüler için destek sunar.

### Oluşturma ve Yazdırma

#### Eksen Başlıklarını DrawingML Grafiklerde Özelleştirme <sup>23.9</sup>

DrawingML grafiklerdeki eksen başlıklarını özelleştirme yeteneği, yeni bir genel sınıf [ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/) ve [title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/) özelliğinin uygulanmasıyla tanıtıldı.

####  Bir Paragraf içindeki Yazı Tiplerinin Dikey Konumunu Belirleme <sup>23.9</sup>

Yeni genel [baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/) özelliğini ve yeni [BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/) numaralandırmasını kullanarak bir paragraf içindeki yazı tiplerinin dikey konumunu tanımlamak artık mümkün.

#### Ön Plan Renk Kontrolü <sup>23.10</sup>

**BaseForeColor** özelliği aracılığıyla [Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/) ve [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) sınıflarına değiştiriciler olmadan ön plan rengini alma yeteneği eklendi.

#### Grafiklerin İşlevselliğini Genişletme <sup>23.10</sup>

[ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/) ve [ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/) sınıflarının işlevselliği yeni yöntemler ve özelliklerle genişletildi.

#### Görüntüyü Otomatik Olarak Ayarlayın ve Şekle Sığdırın <sup>23.10</sup>

Yeni [fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default) yöntemi ile bir görüntüyü belirli bir şekle otomatik olarak ayarlamanın ve sığdırmanın basit bir yolu sağlanmıştır.

#### DrawingML Grafik Gösterge Girişleri <sup>23.11 için Varsayılan Yazı Tipi Biçimlendirmesi</sup>

DrawingML grafiklerin gösterge girişleri için varsayılan yazı tipi biçimlendirmesini belirtme özelliği [font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/) özelliği aracılığıyla eklenmiştir. Bu özellik, grafik öğeleri için daha akıcı ve tutarlı bir görünüm sağlayarak genel belge estetiğini geliştirir.

#### Reader <sup>23.12'da PDF'i Açarken Sayfa Düzenini Belirtin</sup>

Bir belgeyi PDF okuyucuda açarken kullanılacak sayfa düzenini belirleme yeteneği, [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) sınıfına yeni bir [page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/) özelliğinin getirilmesi ve yeni bir [PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/) numaralandırmasının getirilmesi yoluyla eklenmiştir.

### Belgeleri Yükleme ve Kaydetme

#### Markdown <sup>23.9 içinde URIs Resmi Oluşturmak için Bir Klasör Adı Belirtme</sup>

[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) sınıfı, Markdown belgesine yazılan URIs görüntüsünü oluşturmak için kullanılan klasörün adını belirtmeye izin veren [images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/) özelliği dahil edilerek genişletildi.

#### PDF Çıktı Boyutunu Küçült <sup>23.10</sup>

[optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/) ayarları kullanılırken çıktı boyutunu küçültmek için çeşitli PDF işleme optimizasyonları uygulanmıştır.

#### TXT Belgeleri Yüklerken Köprüleri Tanıma <sup>23.10</sup>

TXT belgeleri yüklerken köprüleri tanıma özelliği, yeni bir [detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/) özelliği eklenerek uygulanmıştır.

### Diğer

- Rasterleştirme boyutunu belirlemek için meta dosyası oluşturma öykünmesi, özellikle WMF kalem genişliği ve EMF kozmetik kalem genişliği için uygulanmıştır. Bunu başarmak için **ScaleWmfFontsToMetafileSize** özelliği [emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/) özelliği ile değiştirildi ve [emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/) özelliği eklendi. <sup>23.9</sup>
- [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions) yöntemi kullanılarak, geçerli imleç konumunda bir belgeyi başka bir belgeye eklemek için basitleştirilmiş bir yöntem getirilmiştir. <sup>23.10</sup>
- Stil özelliklerine erişme ve bunları değiştirme yeteneği, yeni [locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/) özelliğinin eklenmesiyle eklenmiştir. <sup>23.10</sup>
- [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/) sınıfının yöntemlerine genel bir tür parametresi eklenmiştir. <sup>23.10</sup>
- Bir belgenin tüm bölümlerini aynı XLSX çalışma sayfasına yazma yeteneği, yeni [XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/) numaralandırma türü ve yeni [section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/) özelliği aracılığıyla sağlanmıştır. <sup>23.11</sup>
* ZIP64 biçim uzantılarının OOXML belgeler için nasıl kullanılacağını denetlemenin bir yolu, `OoxmlSaveOptions` sınıfının yeni Zip64Mode özelliği ve yeni Zip64Mode numaralandırması aracılığıyla uygulanmıştır. <sup>23.12</sup>
* WebP görüntüsü için destek sunuldu. Lütfen bu özelliğin yalnızca .NetStandart ve .NET6+ sürümleri için mevcut olduğunu unutmayın. <sup>23.12</sup>

{{% alert color="primary" %}}

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 23.9 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 23.10 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 23.11 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için .NET 23.12 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words .NET üzerinden Python için 23,5, 23,6, 23,7, 23,8

Aspose.Words 23.5 grafik serisi verileriyle ve ODT belgelerle çalışma becerisini geliştirir, ayrıca üstbilgileri / altbilgileri ve bunların metin kaydırmalarını geliştirir.

Aspose.Words 23.6 işleme seçeneklerini genişletir, yeni bir dışa aktarma biçimi ekler, LINQ raporlama ve LowCode araçlarını geliştirir.

Aspose.Words 23.7 raporlama yeteneklerini geliştirir, yeni bir dışa aktarma biçimi ekler ve tablolar ve dijital imzalarla çalışmaya değişiklikler getirir.

Aspose.Words 23.8 farklı biçimlerin yeteneklerini genişletir, oluşturmayı geliştirir ve alanlarla çalışmak için yeni seçenekler ekler.

### Desteklenen Formatlar

* 23.6 sürümünden başlayarak, bir belgeyi XLSX biçiminde kaydetmek mümkündür. Artık belgelerinizi Excel formatına dönüştürebilirsiniz. <sup>23.6</sup>

* 23.7 sürümünden başlayarak, bir belge sayfasını veya şeklini EPS biçiminde kaydetmek mümkündür. <sup>23.7</sup>

### Yeni Format Özellikleri

- MOBI belgeler için otomatik olarak İçindekiler Tablosu (TOC) oluşturma işlevi tanıtıldı. <sup>23.8</sup>
- [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) oluşturucu [PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) ile genişletildi. <sup>23.8</sup>
- EMF meta dosyaları için dikey metnin şekillendirilmesi uygulanmıştır. <sup>23.8</sup>

### İşleme

#### Grafik Serisi Verilerini Alma ve Değiştirme <sup>23.5</sup>

Grafik serisi verilerini alma ve değiştirme özelliği eklenerek sağlandı:

- yeni sınıflar: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- yeni numaralandırma türleri: [ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### Gelişmiş Tipografi Desteği <sup>23.6</sup>

WMF, EMF ve EMF + görüntülemede Gelişmiş Tipografi Desteği eklendi.

#### Sayfadaki Renkli İçerik <sup>23.6</sup>

Sayfanın renkli olup olmadığını gösteren genel özellik [PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/) eklenmiştir.

#### Grafik Veri Etiketleri için Biçimlendirme <sup>23.6</sup>

Grafik veri etiketleri için dolgu, kontur ve belirtme çizgisi biçimlendirmesini ayarlama özelliği uygulanmıştır.

### Mail Merge ve Raporlama

#### LINQ Raporlama Motoru <sup>23.6 için Dinamik HTML Ekleme</sup>

LINQ Raporlama Altyapısı için dinamik HTML eklemenin yeni bir yolu eklendi.

#### Mustache Etiket Desteği <sup>23.7</sup>

Mustache etiketleri artık [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/) ve [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/) yöntemlerinde destekleniyor.

#### İşlenen Görüntülerin Boyutunu Belirtme <sup>23.8</sup>

İşlenen görüntülerin piksel cinsinden boyutunu belirtmek için yeni bir genel özellik [image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/) tanıtıldı.

#### Boşlukları JSON Dize Değerleri için Koru - LINQ <sup>23.8</sup>

JSON dize değerlerinin boşluklarını korumak için LINQ Raporlama Altyapısına bir seçenek eklendi.

### LowCode <sup>23.6</sup>

Farklı belge türlerini tek bir çıktı belgesinde birleştirmeyi amaçlayan yeni LowCode yöntemler eklendi.

### Diğer

- Üstbilgilerde / altbilgilerde metin kaydırma desteği uygulanmıştır. <sup>23.5</sup>
- ODT belgelerden dijital imzaları kaldırma özelliği [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str) yöntemi ile eklenmiştir. <sup>23.5</sup>
- Fonetik kılavuzun temel ve yakut metnini elde etmek için [phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/) kamu malı [Run](https://reference.aspose.com/words/python-net/aspose.words/run/) eklenmiştir. <sup>23.5</sup>
- Dijital olarak imzalanmış bir belgeden bayt dizisi olarak dijital imza değeri alma özelliği, yeni bir [signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/) özelliği eklenerek eklenmiştir. <sup>23.7</sup>
- [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/) ve [Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/) sınıfları yeni genel üyelerle genişletildi – [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), ve [Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/). <sup>23.7</sup>

{{% alert color="primary" %}}

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 23.5 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-5-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 23.6 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-6-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 23.7 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

Hakkında daha fazla bilgi edinin [Aspose.Words için Python via .NET 23.8 Sürüm Notları](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## Ayrıca bakınız

{{% alert color="primary" %}}

Bu sayfa, son 2 yılın en son sürüm haberlerini içerir. Önceki sürümlerle ilgili ayrıntılar için bkz. [Sürüm Notları'](https://releases.aspose.com/words/python/release-notes/) ilgili bölümlerdeki sayfalar.

{{% /alert %}}
