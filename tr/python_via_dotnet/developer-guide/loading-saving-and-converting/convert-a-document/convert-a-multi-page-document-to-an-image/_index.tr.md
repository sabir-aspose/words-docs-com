---
title: Çok Sayfalı Bir Belgeyi Python içindeki Bir Görüntüye Dönüştürme
second_title: Aspose.Words için Python
articleTitle: Çok Sayfalı Bir Belgeyi Görüntüye Dönüştürme
linktitle: Çok Sayfalı Bir Belgeyi Görüntüye Dönüştürme
type: docs
description: "Çok sayfalı belgeleri raster görüntülere dışa aktarma (JPG, PNG, GIF, BMP, TIFF, WebP) Python kullanarak."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /tr/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Python via .NET için Aspose.Words, kullanıcıların çok sayfalı belgeleri raster görüntülere dışa aktarmasına olanak tanır. Bu, düzenlenebilir olmayan kullanım için belgelerin önizlemelerini, arşivlerini veya görsel temsillerini oluşturmak için yararlı olabilir.

## Hangi Formatlar Çok Sayfalı Dışa Aktarmayı Destekler?

Aspose.Words aşağıdaki raster görüntü formatlarına çok sayfalı dışa aktarmayı destekler:

* Jpeg
* Gıf
* Png
* Bmp
* Tıff
* WebP

## Çok Sayfalı Bir Belgeyi Görüntüye Nasıl Dışa Aktarabilirim

Çok sayfalı bir belgeyi bir görüntüye dışa aktarma özelliği [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) sınıfı kullanılarak uygulanır - bir görüntüye kaydederken sayfaların nasıl düzenlenmesi gerektiğini belirtebilirsiniz:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - belirtilen sayfaların yalnızca ilkini kaydedin
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - sütun sayısını belirtirken sayfaları soldan sağa ve yukarıdan aşağıya bir ızgara halinde düzenleyin
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - sayfaları yatay olarak yan yana, soldan sağa, tek bir çıktıda düzenleyin
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - sayfaları tek bir çıktıda dikey olarak birbiri altına yerleştirin
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - her sayfayı çok çerçeveli TIFF bir görüntüde ayrı bir çerçeve olarak düzenleyin, yalnızca TIFF görüntü formatları için geçerlidir

Aşağıdaki kod örneği, çok sayfalı bir DOCX belgenin Yatay düzende JPEG görüntü olarak nasıl kaydedileceğini gösterir:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Çıktı dosyası sayfası görünümünü de özelleştirebilirsiniz - [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) ve [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/) belirtin.

Aşağıdaki kod örneği, çok sayfalı bir DOCX belgenin Izgara düzenine sahip PNG görüntü olarak nasıl kaydedileceğini gösterir:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.PNG)
# Set up a grid layout with:
# - 3 columns per row.
# - 10pts spacing between pages (horizontal and vertical).
options.page_layout = aw.saving.MultiPageLayout.grid(3, 10, 10)

# Customize the background and border.
options.page_layout.back_color = aspose.pydrawing.Color.light_gray
options.page_layout.border_color = aspose.pydrawing.Color.blue
options.page_layout.border_width = 2

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}