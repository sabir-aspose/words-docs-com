---
title: Mengkonversi Word ke PDF di C#
second_title: Aspose.Words untuk .NET
articleTitle: Mengubah dokumen ke PDF
linktitle: Mengubah dokumen ke PDF
description: "Mengkonversi Word ke PDF di C#. Contoh kode sederhana untuk konversi DOCX ke PDF. Mendukung semua format Word dan gambar."
type: docs
weight: 10
url: /id/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Kemampuan untuk mengkonversi dokumen dengan mudah dan handal dari satu format ke format lain adalah fitur utama Aspose.Words. PDF adalah salah satu format paling populer untuk konversi – ini adalah format dengan tata letak tetap yang mempertahankan tampilan asli dokumen saat rendering di berbagai platform. Istilah "rendering" digunakan dalam Aspose.Words untuk menggambarkan proses mengubah dokumen menjadi format file yang dipaginasi atau memiliki konsep halaman.

## Mengkonversi dokumen Word ke PDF

Konversi dari Word ke PDF adalah proses yang cukup kompleks yang memerlukan beberapa tahap perhitungan. Mesin tata letak Aspose.Words meniru cara kerja mesin tata letak halaman Microsoft Word, membuat dokumen PDF keluaran terlihat sedekat mungkin dengan yang dapat Anda lihat di Microsoft Word.

Dengan Aspose.Words, Anda dapat mentransformasi dokumen secara programatis dari format Word, seperti DOC atau DOCX, ke PDF tanpa menggunakan Microsoft Office. Artikel ini menjelaskan cara melakukan konversi ini.

{{% alert color="primary" %}}

Perhatikan bahwa jumlah halaman dalam dokumen mempengaruhi waktu konversi.

{{% /alert %}}

### Mengkonversi DOCX atau DOC ke PDF

Mengubah dari format dokumen DOC atau DOCX ke format PDF di Aspose.Words sangat mudah dan dapat dicapai hanya dengan dua baris kode yang:

1. Muat dokumen Anda ke dalam objek [Document](https://reference.aspose.com/words/net/aspose.words/document/) menggunakan salah satu konstruktornya dengan menentukan nama dokumen beserta ekstensi formatnya.
1. Panggil salah satu metode [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) pada objek **Document** dan tentukan format output yang diinginkan sebagai PDF dengan memasukkan nama file dengan ekstensi ".PDF".

Contoh kode berikut menunjukkan cara mengkonversi dokumen dari DOCX ke PDF menggunakan metode [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Anda dapat mengunduh file template contoh ini dari [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Terkadang perlu untuk menentukan opsi tambahan yang dapat mempengaruhi hasil penyimpanan dokumen sebagai PDF. Opsi ini dapat ditentukan dengan menggunakan kelas [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), yang berisi properti yang menentukan bagaimana output PDF akan ditampilkan.

Perhatikan bahwa dengan teknik yang sama, Anda dapat mentransformasi dokumen format flow-layout apa pun ke format PDF.

{{% /alert %}}

### Mengubah ke berbagai standar PDF

Aspose.Words menyediakan enumerasi [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) untuk mendukung konversi DOC atau DOCX ke berbagai standar format PDF (seperti PDF 1.7, PDF 1.5, dll.).

Contoh kode berikut menunjukkan cara mengkonversi dokumen ke PDF 1.7 menggunakan [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) dengan kepatuhan terhadap PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Mengkonversi gambar ke PDF

Konversi ke PDF tidak terbatas pada format dokumen Microsoft Word. Format apa pun yang didukung oleh Aspose.Words, termasuk yang dibuat secara programatis, juga dapat diubah ke PDF. Misalnya, kita dapat mengkonversi gambar halaman tunggal, seperti JPEG, PNG, BMP, EMF, atau WMF, serta gambar multi-halaman, seperti TIFF dan GIF, ke PDF.

Contoh kode berikut menunjukkan cara mentransformasi gambar JPEG dan TIFF ke PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Agar kode ini berfungsi, Anda perlu menambahkan referensi ke Aspose.Words dan `System.Drawing` ke proyek Anda.

## Mengurangi ukuran output PDF

Saat menyimpan ke PDF, Anda dapat menentukan apakah Anda ingin mengoptimalkan output. Untuk melakukan ini, Anda perlu mengatur flag [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) ke true, dan kemudian kanvas bersarang yang berlebihan dan kosong akan dihapus, glyph yang berdekatan dengan format yang sama akan digabungkan.

Contoh kode berikut menunjukkan cara mengoptimalkan output:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Menggunakan properti **OptimizeOutput** dapat mempengaruhi akurasi tampilan konten.

{{% /alert %}}

## Lihat juga

- Artikel [Rendering](/words/id/net/rendering/) untuk informasi lebih lanjut tentang format halaman tetap dan flow-layout
- Artikel [Konversi ke format halaman tetap](/words/id/net/converting-to-fixed-page-format/#what-is-a-page-layout) untuk informasi lebih lanjut tentang tata letak halaman
- Artikel [Menentukan opsi rendering saat mengubah ke PDF](/words/id/net/specify-rendering-options-when-converting-to-pdf/) untuk informasi lebih lanjut tentang penggunaan kelas `PdfSaveOptions`
- Artikel [Pelajari fitur konversi ke PDF/A dan PDF/UA](/words/id/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) yang menjelaskan standar PDF mana dan ISO yang relevan untuk standar PDF yang didukung Aspose.Words
- Artikel [Standar PDF mana yang lebih baik untuk dipilih](/words/id/net/which-pdf-standard-is-better-to-choose/) untuk menentukan standar PDF mana yang masuk akal untuk kasus mana

- Artikel [Bekerja dengan PDF/A atau PDF/UA](/words/id/net/working-with-pdfa-or-pdfua/) menjelaskan persyaratan konten dokumen dalam format PDF/A dan PDF/UA – terutama persyaratan struktur dan font

- Artikel [Peringatan masalah aksesibilitas saat menyimpan ke PDF/A dan PDF/UA](/words/id/net/warnings-when-saving-to-pdfa-and-pdfua/) menjelaskan persyaratan aksesibilitas konten apa yang diberlakukan PDF/A dan PDF/UA
