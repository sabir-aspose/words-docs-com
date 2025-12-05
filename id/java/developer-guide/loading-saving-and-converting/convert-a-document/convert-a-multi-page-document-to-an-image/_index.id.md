---
title: Konversikan Dokumen Multi-halaman menjadi Gambar dalam Java
second_title: Aspose.Words untuk Java
articleTitle: Mengonversi Dokumen Multi-halaman menjadi Gambar
linktitle: Mengonversi Dokumen Multi-halaman menjadi Gambar
type: docs
description: "Ekspor dokumen multi-halaman ke gambar raster(JPG, PNG, GIF, BMP, TIFF, WebP) menggunakan Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /id/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words untuk Java memungkinkan pengguna mengekspor dokumen multi-halaman ke gambar raster. Ini dapat berguna untuk membuat pratinjau, arsip, atau representasi visual dokumen untuk penggunaan yang tidak dapat diedit.

## Format apa yang mendukung Ekspor Multi-halaman?

Aspose.Words mendukung ekspor multi-halaman ke format gambar raster berikut:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Cara Mengekspor Dokumen Multi-halaman ke Gambar

Fitur mengekspor dokumen multi-halaman ke gambar diimplementasikan menggunakan kelas [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) – Anda dapat menentukan bagaimana halaman harus diatur saat menyimpan ke gambar:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - simpan hanya halaman pertama dari halaman yang ditentukan
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - susun halaman dalam kisi, dari kiri ke kanan dan dari atas ke bawah, sambil menentukan jumlah kolom
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - susun halaman secara horizontal berdampingan, kiri ke kanan, dalam satu keluaran
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - susun halaman secara vertikal satu di bawah yang lain dalam satu keluaran
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - susun setiap halaman sebagai bingkai terpisah dalam gambar TIFF multi-bingkai, hanya berlaku untuk format gambar TIFF 

Contoh kode berikut menunjukkan cara menyimpan dokumen DOCX multi-halaman sebagai gambar JPEG dengan tata letak Horizontal:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Anda juga dapat menyesuaikan tampilan halaman file keluaran-tentukan [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor), dan [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

Contoh kode berikut menunjukkan cara menyimpan dokumen DOCX multi-halaman sebagai gambar PNG dengan tata letak Kisi:

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