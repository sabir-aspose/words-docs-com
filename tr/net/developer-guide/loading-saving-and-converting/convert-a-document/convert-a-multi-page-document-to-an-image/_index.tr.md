---
title: Çok Sayfalı Bir Belgeyi C# içindeki Bir Görüntüye Dönüştürme
second_title: Aspose.Words için .NET
articleTitle: Çok Sayfalı Bir Belgeyi Görüntüye Dönüştürme
linktitle: Çok Sayfalı Bir Belgeyi Görüntüye Dönüştürme
type: docs
description: "Çok sayfalı belgeleri raster görüntülere dışa aktarma (JPG, PNG, GIF, BMP, TIFF, WebP) C# kullanarak."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words for .NET, kullanıcıların çok sayfalı belgeleri raster görüntülere dışa aktarmasına olanak tanır. Bu, düzenlenebilir olmayan kullanım için belgelerin önizlemelerini, arşivlerini veya görsel temsillerini oluşturmak için yararlı olabilir.

## Hangi Formatlar Çok Sayfalı Dışa Aktarmayı Destekler?

Aspose.Words aşağıdaki raster görüntü formatlarına çok sayfalı dışa aktarmayı destekler:

* Jpeg
* Gıf
* Png
* Bmp
* Tıff
* WebP

## Çok Sayfalı Bir Belgeyi Görüntüye Nasıl Dışa Aktarabilirim

Çok sayfalı bir belgeyi bir görüntüye dışa aktarma özelliği [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) sınıfı kullanılarak uygulanır - bir görüntüye kaydederken sayfaların nasıl düzenlenmesi gerektiğini belirtebilirsiniz:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - belirtilen sayfaların yalnızca ilkini kaydedin
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - sütun sayısını belirtirken sayfaları soldan sağa ve yukarıdan aşağıya bir ızgara halinde düzenleyin
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - sayfaları yatay olarak yan yana, soldan sağa, tek bir çıktıda düzenleyin
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - sayfaları tek bir çıktıda dikey olarak birbiri altına yerleştirin
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - her sayfayı çok çerçeveli TIFF bir görüntüde ayrı bir çerçeve olarak düzenleyin, yalnızca TIFF görüntü formatları için geçerlidir

Aşağıdaki kod örneği, çok sayfalı bir DOCX belgenin Yatay düzende JPEG görüntü olarak nasıl kaydedileceğini gösterir:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Çıktı dosyası sayfası görünümünü de özelleştirebilirsiniz - [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) ve [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/) belirtin.

Aşağıdaki kod örneği, çok sayfalı bir DOCX belgenin Izgara düzenine sahip PNG görüntü olarak nasıl kaydedileceğini gösterir:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Png);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.PageLayout = MultiPageLayout.Grid(3, 10, 10);

// Customize the background and border.
options.PageLayout.BackColor = Color.LightGray;
options.PageLayout.BorderColor = Color.Blue;
options.PageLayout.BorderWidth = 2;

doc.Save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}