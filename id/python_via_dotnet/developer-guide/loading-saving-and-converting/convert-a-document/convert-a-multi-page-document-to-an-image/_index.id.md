---
title: Konversikan Dokumen Multi-halaman menjadi Gambar dalam Python
second_title: Aspose.Words untuk Python
articleTitle: Mengonversi Dokumen Multi-halaman menjadi Gambar
linktitle: Mengonversi Dokumen Multi-halaman menjadi Gambar
type: docs
description: "Ekspor dokumen multi-halaman ke gambar raster(JPG, PNG, GIF, BMP, TIFF, WebP) menggunakan Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /id/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words untuk Python via .NET memungkinkan pengguna mengekspor dokumen multi-halaman ke gambar raster. Ini dapat berguna untuk membuat pratinjau, arsip, atau representasi visual dokumen untuk penggunaan yang tidak dapat diedit.

## Format apa yang mendukung Ekspor Multi-halaman?

Aspose.Words mendukung ekspor multi-halaman ke format gambar raster berikut:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Cara Mengekspor Dokumen Multi-halaman ke Gambar

Fitur mengekspor dokumen multi-halaman ke gambar diimplementasikan menggunakan kelas [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) – Anda dapat menentukan bagaimana halaman harus diatur saat menyimpan ke gambar:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - simpan hanya halaman pertama dari halaman yang ditentukan
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - susun halaman dalam kisi, dari kiri ke kanan dan dari atas ke bawah, sambil menentukan jumlah kolom
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - susun halaman secara horizontal berdampingan, kiri ke kanan, dalam satu keluaran
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - susun halaman secara vertikal satu di bawah yang lain dalam satu keluaran
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - susun setiap halaman sebagai bingkai terpisah dalam gambar TIFF multi-bingkai, hanya berlaku untuk format gambar TIFF 

Contoh kode berikut menunjukkan cara menyimpan dokumen DOCX multi-halaman sebagai gambar JPEG dengan tata letak Horizontal:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Anda juga dapat menyesuaikan tampilan halaman file keluaran-tentukan [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/), dan [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

Contoh kode berikut menunjukkan cara menyimpan dokumen DOCX multi-halaman sebagai gambar PNG dengan tata letak Kisi:

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