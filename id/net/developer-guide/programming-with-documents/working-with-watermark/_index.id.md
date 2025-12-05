---
title: Bekerja dengan Tanda Air dalam C#
second_title: Aspose.Words untuk .NET
articleTitle: Bekerja dengan Tanda Air
linktitle: Bekerja dengan Tanda Air
description: "Manipulasi tanda air dokumen menggunakan C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /id/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Topik ini membahas cara bekerja secara terprogram dengan tanda air menggunakan Aspose.Words. Tanda air adalah gambar latar belakang yang ditampilkan di belakang teks dalam dokumen. Tanda air dapat berisi teks atau gambar yang diwakili oleh kelas [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Coba online**

Anda dapat mencoba fungsi ini dengan kami [Tanda air dokumen online gratis](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Menambahkan Tanda Air ke Dokumen

Di Microsoft Word, tanda air dapat dengan mudah disisipkan ke dalam dokumen menggunakan perintah Sisipkan Tanda Air. Aspose.Words menyediakan kelas [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) untuk menambah atau menghapus tanda air dalam dokumen. Aspose.Words menyediakan pencacahan [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)yang mendefinisikan tiga kemungkinan jenis tanda air (Teks, Gambar, dan Tidak Ada) untuk digunakan.

### Tambahkan Tanda Air Teks

Contoh kode berikut mendemonstrasikan cara menyisipkan tanda air teks dalam dokumen dengan mendefinisikan [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) menggunakan metode [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Tambahkan Tanda Air Gambar

Contoh kode berikut mendemonstrasikan cara menyisipkan tanda air gambar dalam dokumen dengan mendefinisikan [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) menggunakan metode [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Tanda air gambar dapat disisipkan sebagai gambar, string, atau aliran.

Tanda air juga dapat disisipkan menggunakan kelas bentuk juga. Sangat mudah untuk menyisipkan bentuk atau gambar apa pun ke dalam header atau footer dan dengan demikian membuat tanda air dari jenis apa pun yang dapat dibayangkan.

Contoh kode berikut menyisipkan tanda air ke dalam dokumen Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Anda dapat mengunduh file contoh contoh ini dari [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Hapus Tanda Air dari Dokumen

Kelas [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) menyediakan metode hapus untuk menghapus tanda air dari dokumen.

Contoh kode berikut menunjukkan cara menghapus tanda air dari dokumen:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Jika tanda air ditambahkan menggunakan objek kelas [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/), maka untuk menghapus tanda air dari dokumen, Anda hanya perlu menyetel nama bentuk tanda air selama penyisipan, lalu menghapus bentuk tanda air dengan nama yang ditetapkan.

Contoh kode berikut menunjukkan cara mengatur nama bentuk tanda air dan menghapusnya dari dokumen:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Tambahkan Tanda Air ke dalam Sel Tabel

Terkadang Anda perlu menyisipkan tanda air / gambar ke dalam sel tabel dan menampilkannya di luar tabel, Anda dapat menggunakan properti [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). Properti ini mendapatkan atau menetapkan tanda yang menunjukkan apakah bentuk ditampilkan di dalam tabel atau di luarnya. Perhatikan bahwa properti ini hanya berfungsi saat Anda mengoptimalkan dokumen untuk Microsoft Word 2010 menggunakan metode [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

Contoh kode berikut menunjukkan cara menggunakan properti ini:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
