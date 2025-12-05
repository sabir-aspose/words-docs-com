---
title: Konversikan Dokumen Multi-halaman menjadi Gambar dalam C#
second_title: Aspose.Words untuk .NET
articleTitle: Mengonversi Dokumen Multi-halaman menjadi Gambar
linktitle: Mengonversi Dokumen Multi-halaman menjadi Gambar
type: docs
description: "Ekspor dokumen multi-halaman ke gambar raster(JPG, PNG, GIF, BMP, TIFF, WebP) menggunakan C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /id/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words untuk .NET memungkinkan pengguna mengekspor dokumen multi-halaman ke gambar raster. Ini dapat berguna untuk membuat pratinjau, arsip, atau representasi visual dokumen untuk penggunaan yang tidak dapat diedit.

## Format apa yang mendukung Ekspor Multi-halaman?

Aspose.Words mendukung ekspor multi-halaman ke format gambar raster berikut:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Cara Mengekspor Dokumen Multi-halaman ke Gambar

Fitur mengekspor dokumen multi-halaman ke gambar diimplementasikan menggunakan kelas [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) – Anda dapat menentukan bagaimana halaman harus diatur saat menyimpan ke gambar:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - simpan hanya halaman pertama dari halaman yang ditentukan
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - susun halaman dalam kisi, dari kiri ke kanan dan dari atas ke bawah, sambil menentukan jumlah kolom
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - susun halaman secara horizontal berdampingan, kiri ke kanan, dalam satu keluaran
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - susun halaman secara vertikal satu di bawah yang lain dalam satu keluaran
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - susun setiap halaman sebagai bingkai terpisah dalam gambar TIFF multi-bingkai, hanya berlaku untuk format gambar TIFF 

Contoh kode berikut menunjukkan cara menyimpan dokumen DOCX multi-halaman sebagai gambar JPEG dengan tata letak Horizontal:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Anda juga dapat menyesuaikan tampilan halaman file keluaran-tentukan [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/), dan [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

Contoh kode berikut menunjukkan cara menyimpan dokumen DOCX multi-halaman sebagai gambar PNG dengan tata letak Kisi:

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