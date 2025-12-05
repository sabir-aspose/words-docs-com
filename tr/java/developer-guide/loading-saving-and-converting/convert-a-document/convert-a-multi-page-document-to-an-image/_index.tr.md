---
title: Çok Sayfalı Bir Belgeyi Java içindeki Bir Görüntüye Dönüştürme
second_title: Aspose.Words için Java
articleTitle: Çok Sayfalı Bir Belgeyi Görüntüye Dönüştürme
linktitle: Çok Sayfalı Bir Belgeyi Görüntüye Dönüştürme
type: docs
description: "Çok sayfalı belgeleri raster görüntülere dışa aktarma (JPG, PNG, GIF, BMP, TIFF, WebP) Java kullanarak."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words for Java, kullanıcıların çok sayfalı belgeleri raster görüntülere dışa aktarmasına olanak tanır. Bu, düzenlenebilir olmayan kullanım için belgelerin önizlemelerini, arşivlerini veya görsel temsillerini oluşturmak için yararlı olabilir.

## Hangi Formatlar Çok Sayfalı Dışa Aktarmayı Destekler?

Aspose.Words aşağıdaki raster görüntü formatlarına çok sayfalı dışa aktarmayı destekler:

* Jpeg
* Gıf
* Png
* Bmp
* Tıff
* WebP

## Çok Sayfalı Bir Belgeyi Görüntüye Nasıl Dışa Aktarabilirim

Çok sayfalı bir belgeyi bir görüntüye dışa aktarma özelliği [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) sınıfı kullanılarak uygulanır - bir görüntüye kaydederken sayfaların nasıl düzenlenmesi gerektiğini belirtebilirsiniz:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - belirtilen sayfaların yalnızca ilkini kaydedin
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - sütun sayısını belirtirken sayfaları soldan sağa ve yukarıdan aşağıya bir ızgara halinde düzenleyin
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - sayfaları yatay olarak yan yana, soldan sağa, tek bir çıktıda düzenleyin
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - sayfaları tek bir çıktıda dikey olarak birbiri altına yerleştirin
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - her sayfayı çok çerçeveli TIFF bir görüntüde ayrı bir çerçeve olarak düzenleyin, yalnızca TIFF görüntü formatları için geçerlidir

Aşağıdaki kod örneği, çok sayfalı bir DOCX belgenin Yatay düzende JPEG görüntü olarak nasıl kaydedileceğini gösterir:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Çıktı dosyası sayfası görünümünü de özelleştirebilirsiniz - [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) ve [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth) belirtin.

Aşağıdaki kod örneği, çok sayfalı bir DOCX belgenin Izgara düzenine sahip PNG görüntü olarak nasıl kaydedileceğini gösterir:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.PNG);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.setPageLayout(MultiPageLayout.grid(3, 10f, 10f));

// Customize the background and border.
options.getPageLayout().setBackColor(Color.lightGray);
options.getPageLayout().setBorderColor(Color.BLUE);
options.getPageLayout().setBorderWidth(2f);

doc.save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}