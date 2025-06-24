---
title: Apa yang baru
second_title: Aspose.Words untuk C++
articleTitle: Apa yang baru di Aspose.Words untuk C++
linktitle: Apa yang baru di Aspose.Words untuk C++
type: docs
description: "Aspose.Words untuk C++ memperluas dan meningkatkan setiap hari. Di halaman ini, Anda dapat mempelajari tentang fitur produk yang sangat besar dan paling menarik."
weight: 2
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /id/cpp/what-s-new-in-aspose-words-for-cpp/
timestamp: 2025-06-23-19-12-25
---

Halaman ini menjelaskan fitur Aspose.Words baru yang paling menarik yang diperkenalkan dalam rilis terbaru.

## Aspose.Words untuk C++ 25.5

Aspose.Words 25.5 menyempurnakan penyesuaian bagan dengan opsi gaya baru dan meningkatkan ekspor Markdown dengan menawarkan kontrol atas penanganan paragraf kosong.

### Mengonversi, Memuat, dan Menyimpan Dokumen

#### Ekspor Paragraf Kosong ke Markdown <sup>25.5</sup>

Kemampuan untuk mengontrol bagaimana paragraf kosong diekspor ke Markdown telah diperkenalkan dengan menambahkan enumerasi [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownemptyparagraphexportmode/) dan properti [EmptyParagraphExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_emptyparagraphexportmode/).

### Rendering

#### Mengatur Gaya Bagan <sup>25.5</sup>

Kemampuan untuk mengatur gaya bagan telah diperkenalkan dengan menambahkan enumerasi [ChartStyle](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartstyle/) dan properti [Style](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chart/get_style/).

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 25.5 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-5-release-notes/).

{{% /alert %}}

## Aspose.Words untuk C++ 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 memperkenalkan pemeriksaan tata bahasa bertenaga AI dan menyempurnakan penyimpanan dokumen dengan opsi lanjutan untuk format HTML, SVG, dan Markdown.

Aspose.Words 25.2 memperkenalkan peringkasan teks dengan model Anthropic AI, menambahkan dukungan format MsWorks, meningkatkan kontrol tipografi, dan meningkatkan struktur PDF dan penanganan daftar.

Aspose.Words 25.3 menyempurnakan pemeriksa tata bahasa dan pemilihan font bertenaga AI dengan properti UpdateAmbiguousTextFont, serta meningkatkan ekspor lampiran PDF.

Aspose.Words 25.4 memperkenalkan dukungan untuk ukuran kertas baru, memungkinkan kontrol ekspor HTML tingkat lanjut, meningkatkan penanganan tanda air, dan meningkatkan kegunaan LowCode API.

### AI-Fitur bertenaga

#### Dokumen AI Pemeriksaan Tata Bahasa

* Kemampuan untuk memeriksa tata bahasa dokumen yang disediakan menggunakan model generatif OpenAI telah diperkenalkan dengan menambahkan metode [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/) baru. <sup>25.1</sup>
* Fitur Pemeriksaan Tata Bahasa bertenaga AI telah diperbarui untuk mendukung semua model yang tersedia dalam pencacahan [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Ringkasan Menggunakan Model Bahasa Generatif Anthropic <sup>25.2</sup>

Peringkasan teks menggunakan model bahasa generatif Anthropic telah diaktifkan dengan memperkenalkan kelas publik baru [AnthropicAiModel](https://reference.aspose.com/words/cpp/aspose.words.ai/).

### Low Code

#### Low Code API Kegunaan <sup>25.4</sup>

Peningkatan signifikan pada kegunaan **LowCode API** telah diperkenalkan, menyederhanakan pemrosesan dokumen dan mengurangi kebutuhan akan kode yang berulang.

### Format yang Didukung <sup>25.2</sup>

Mulai dari versi 25.2, kompatibilitas dengan format pemuatan MsWorks baru untuk dokumen Karya Microsoft telah ditambahkan.

### Mengonversi, Memuat, dan Menyimpan Dokumen

#### Peningkatan Penyimpanan ke Format HTML dan SVG <sup>25.1</sup>

Menyimpan ke format HTML dan SVG telah ditingkatkan dengan menambahkan properti **IdPrefix** dan **RemoveJavaScriptFromLinks** ke kelas [HtmlFixedSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlfixedsaveoptions/) dan [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/).

#### Setel Resolusi Gambar dan Mode Keluaran OfficeMath Saat Menyimpan ke Markdown <sup>25.1</sup>

- Opsi [ImageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imageresolution/) baru telah ditambahkan ke kelas [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) untuk mengatur resolusi gambar.
- Opsi [OfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_officemathexportmode/) baru dan enumerasi [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownofficemathexportmode/) telah dan ditambahkan ke kelas [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) untuk menyetel mode keluaran OfficeMath.
- Kemampuan untuk menyetel tanda air gambar dari aliran telah diperkenalkan dengan menambahkan kelebihan beban baru ke metode [SetImage](https://reference.aspose.com/words/cpp/aspose.words/watermark/setimage/#watermarksetimageconst-systemsharedptrsystemiostream-const-systemsharedptrasposewordsimagewatermarkoptions-method). <sup>25.4</sup>

### Rendering

#### Kontrol Tipografi yang Ditingkatkan <sup>25.2</sup>

Properti [NumberSpacing](https://reference.aspose.com/words/cpp/aspose.words/font/get_numberspacing/) telah ditambahkan untuk kontrol tipografi yang lebih baik.

#### Mengontrol Pemilihan Font untuk Karakter Ambigu <sup>25.3</sup>

Properti publik baru [UpdateAmbiguousTextFont](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/get_updateambiguoustextfont/) telah ditambahkan ke kelas [SaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/) untuk mengontrol pemilihan font sesuai dengan kode karakter yang digunakan.

#### Opsi Ukuran Kertas <sup>25.4</sup>

Kemampuan untuk menggunakan ukuran kertas JIS B4 dan JIS B5 telah diperkenalkan dengan menambahkan nilai baru ke enumerasi [PaperSize](https://reference.aspose.com/words/cpp/aspose.words/papersize/).

#### HTML Kontrol Keluaran <sup>25.4</sup>

Kemampuan untuk menghapus JavaScript dari hyperlink URLs selama ekspor HTML telah diperkenalkan dengan menambahkan properti [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlsaveoptions/get_removejavascriptfromlinks/).

### Lainnya

* PDF struktur logika telah ditingkatkan dengan dukungan untuk bidang TOA, BIBLIOGRAPHY, dan INDEX. <sup>25.2</sup>
* Metode [AddSingleLevelList](https://reference.aspose.com/words/cpp/aspose.words.lists/listcollection/addsinglelevellist/) telah diperkenalkan untuk penanganan daftar yang lebih baik. <sup>25.2</sup>
* Properti baru [AttachmentsEmbeddingMode](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/get_attachmentsembeddingmode/) telah ditambahkan untuk menggantikan **EmbedAttachments** untuk meningkatkan ekspor lampiran PDF. Selain itu, nilai baru telah ditambahkan ke enumerasi [PdfCompliance](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfcompliance/) untuk mendukung lampiran versi PDF/A. Selain itu, lampiran sekarang didukung dengan enkripsi. <sup>25.3</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 25.1 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-1-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 25.2 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-2-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 25.3 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-3-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 25.4 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words untuk C++ 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 memperkenalkan penyisipan group shape dan penyisipan StructuredDocumentTag melalui DocumentBuilder, menyempurnakan rendering bagan radial dengan gradasi, meningkatkan tanda tangan digital dengan dukungan XAdES-EPES, menambahkan pengenalan garis bawah Markdown, dan menyediakan akses ke pemisah catatan kaki / catatan akhir.

Aspose.Words 24.10 memperkenalkan dukungan kontrol ActiveX yang ditingkatkan dengan pembuatan CommandButton, kontrol visibilitas bentuk baru, kemampuan untuk group shapes, peningkatan ekspor Markdown untuk tabel, pemformatan bagan untuk bagan Pie dan Doughnut, penanganan penyandian Big5 yang lebih baik, dan dukungan untuk font Taiwan yang sudah ketinggalan zaman.

Aspose.Words 24.11 memperkenalkan peringkasan dokumen bertenaga AI, opsi rendering yang ditingkatkan, peningkatan akses ke properti dokumen, dan teks kontrol ActiveX.

Aspose.Words 24.12 memperkenalkan penempatan label data yang dapat disesuaikan, terjemahan teks bertenaga Google AI, opsi pembersihan Mail Merge yang disempurnakan, dan kelas pemrosesan LowCode baru.

### AI-Fitur bertenaga

#### Ringkasan Dokumen Menggunakan OpenAI dan Google <sup>24.11</sup>

Dukungan untuk peringkasan dokumen menggunakan model bahasa generatif **OpenAI** dan **Google** telah terintegrasi.

#### Terjemahan teks menggunakan model bahasa generatif Google <sup>24.12</sup>

Kemampuan untuk menerjemahkan teks menggunakan model bahasa generatif Google telah diterapkan di Aspose.Words dengan menambahkan metode [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) dan pencacahan [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) ke namespace [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Kelas LowCode baru seperti [Comparer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/cpp/aspose.words.lowcode/merger/), [Replacer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/cpp/aspose.words.lowcode/splitter/) dll. telah diperkenalkan, menawarkan serangkaian metode yang memberikan keseimbangan sempurna antara kesederhanaan dan fleksibilitas untuk pemrosesan dokumen.

### Rendering dan Pencetakan

#### Kelulusan pada Grafik Radial <sup>24.9</sup>

Rendering gradasi pada grafik radial telah diterapkan.

#### CommandButton ActiveX Kontrol <sup>24.10</sup>

Kemampuan untuk membuat kontrol CommandButton ActiveX telah diperkenalkan dengan menambahkan metode publik baru [InsertForms2OleControl](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertforms2olecontrol/) dan kelas publik baru **Forms2OleControl**.

#### Kontrol Visibilitas Bentuk <sup>24.10</sup>

Properti publik baru [Hidden](https://reference.aspose.com/words/cpp/aspose.words.drawing/shapebase/get_hidden/) telah ditambahkan untuk mengontrol visibilitas bentuk.

#### Perubahan pada Bagan Pie dan Doughnut <sup>24.10</sup>

Beberapa properti publik baru telah ditambahkan ke bagan format Pie dan Doughnut.

#### Kontrol Rendering Batas Bidang Formulir Pilihan PDF <sup>24.11</sup>

Opsi baru untuk mengontrol rendering batas bidang formulir pilihan PDF telah diterapkan dengan menambahkan opsi publik baru **RenderChoiceFormFieldBorder**.

#### Dapatkan dan Atur Kode Format untuk Data Bagan <sup>24.11</sup>

Kemampuan untuk mendapatkan dan mengatur kode format untuk data bagan telah ditambahkan dengan menerapkan properti **FormatCode** di kelas [ChartXValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartyvaluecollection/), dan [BubbleSizeCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/bubblesizecollection/).

#### Render Bagan Histogram dengan Tempat Sampah dan Label <sup>24.11</sup>

Rendering grafik histogram telah ditingkatkan dengan memungkinkan sejumlah tempat sampah dan label tertentu.

#### Sesuaikan Penempatan Label Data <sup>24.12</sup>

Kemampuan untuk menyesuaikan penempatan label data telah ditambahkan dengan memperkenalkan properti baru ke kelas [ChartDataLabel](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabel/) dan [ChartDataLabelCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabelcollection/).

### Mengonversi, Memuat, dan Menyimpan Dokumen

#### Garis Bawahi Pemformatan saat Memuat File Markdown <sup>24.9</sup>

Opsi untuk mengenali pemformatan garis bawah saat memuat dokumen Markdown telah digabungkan dengan menambahkan properti publik baru **ImportUnderlineFormatting**.

#### Mengekspor tabel sebagai HTML saat menyimpan ke Markdown <sup>24.10</sup>

Opsi untuk mengekspor tabel sebagai HTML saat menyimpan dokumen ke format Markdown telah diterapkan dengan menambahkan properti publik baru [ExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_exportashtml/) dan enumerasi [MarkdownExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownexportashtml/).

#### Ekspor PDF dengan Struktur Logika yang Diperbarui <sup>24.11</sup>

Ekspor PDF telah ditingkatkan dengan menyertakan properti judul tabel sebagai judul elemen struktur logis PDF.

### Mail Merge dan Pelaporan

#### Hapus Tabel Kosong selama Mail Merge <sup>24.12</sup>

Opsi **RemoveEmptyTables** baru telah ditambahkan ke enumerasi [MailMergeCleanupOptions](https://reference.aspose.com/words/cpp/aspose.words.mailmerging/mailmergecleanupoptions/) untuk menyempurnakan keluaran Mail Merge.

### Tanda Tangan Digital

#### Tanda tangani Dokumen dengan XAdES-EPES <sup>24.9</sup>

Kemampuan untuk menandatangani dokumen dengan tanda tangan XAdES-EPES level XML-DSig telah diperkenalkan dengan menambahkan properti publik baru **XmlDsigLevel** dan pencacahan publik baru **XmlDsigLevel**.

### Lainnya

* Metode publik baru [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/) telah ditambahkan ke group shapes. <sup>24.9</sup>
* Metode publik baru [InsertStructuredDocumentTag](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertstructureddocumenttag/) telah ditambahkan untuk menyisipkan **StructuredDocumentTags** ke dalam dokumen. <sup>24.9</sup>
* Akses publik ke pemisah catatan kaki / catatan akhir telah disediakan dengan menambahkan beberapa kelas dan properti publik. <sup>24.9</sup>
* Kemampuan untuk mengelompokkan masing-masing bentuk, group shapes bersama-sama, dan langsung mengelompokkan kedua bentuk dan group shapes telah diperkenalkan dengan menambahkan metode [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/). <sup>24.10</sup>
* Penanganan penyandian Big5 untuk tabel cmap TrueType telah ditingkatkan. <sup>24.10</sup>
* Dukungan untuk font Taiwan yang sudah ketinggalan zaman telah ditingkatkan. <sup>24.10</sup>
* Untuk mengakses properti dokumen yang diperluas, properti hanya-baca telah ditambahkan ke kelas **BuiltInDocumentProperties**. <sup>24.11</sup>
* Menyetel teks untuk kontrol ActiveX telah diaktifkan dengan menambahkan penyetel publik baru ke properti **Forms2OleControl.Caption**. <sup>24.11</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 24.9 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-9-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 24.10 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-10-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 24.11 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-11-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 24.12 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words untuk C++ 24.5, 24.6, 24.7

Aspose.Words 24.5 memperluas opsi untuk rakitan, meningkatkan kemampuan rendering, dan memperluas beberapa opsi lainnya.

Aspose.Words 24.6 meningkatkan opsi rendering, meningkatkan fungsionalitas penelusuran dan perbandingan, dan memperluas beberapa fitur lainnya.

Aspose.Words 24.7 mengubah cara Anda bekerja dengan ActiveX, memperluas kemampuan rendering, serta mengekspor ke format Markdown dan XLSX.

### Format yang Didukung

Mulai dari versi 24.7, ekspor ke PDF/UA-2 didukung untuk memastikan aksesibilitas bagi pengguna penyandang disabilitas.

### Rendering dan Pencetakan

#### Perubahan Bagan, Bentuk, dan DrawingML <sup>24.5</sup>

- DrawingML rendering efek untuk grafik SVG, memperluas fungsionalitas sebelumnya yang terbatas pada gambar, telah diterapkan.
- Dukungan untuk membuat bagan kombo dan menyesuaikan properti seperti lebar celah, tumpang tindih, dan skala gelembung dalam grup deret telah diperkenalkan dengan menambahkan kelas **ChartSeriesGroup** dan **ChartSeriesGroupCollection** serta properti **SeriesGroups**.
- Fungsionalitas untuk memanipulasi efek SoftEdge dari bentuk telah diimplementasikan dengan menambahkan kelas **SoftEdgeFormat**.
- Kemampuan untuk memodifikasi nilai adjust dari bentuk telah diimplementasikan dengan menambahkan kelas publik **AdjustmentCollection** dan **Adjustment** dan properti **Adjustments**.

#### Perubahan Bagan, Bentuk, dan Gambar <sup>24.6</sup>

- Kemampuan pembuatan bagan telah ditingkatkan. Anda sekarang dapat membuat variasi bagan yang lebih luas, termasuk *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* bagan, bagan *Box & Whisker*, *Waterfalls*, dan *Funnels*. Ini memungkinkan Anda untuk memvisualisasikan data Anda dengan cara yang lebih beragam dan informatif.
- Kontrol warna untuk pemformatan bayangan telah ditingkatkan. Anda dapat memperoleh kontrol yang lebih tepat atas tampilan dokumen Anda dengan mengakses warna bayangan.
- Peningkatan kinerja untuk rendering latar belakang telah ditingkatkan. Anda dapat mempercepat rendering latar belakang yang berisi elemen kecil secara signifikan berkat teknologi ubin asli.
- Gradien realistis untuk bentuk telah ditambahkan. Anda sekarang dapat membuat bentuk DML dengan gradien non-linier, meniru gaya visual Microsoft Word untuk tampilan yang lebih halus.

#### Kustomisasi Label Data Bagan <sup>24.7</sup>

Kemampuan untuk menyesuaikan label data bagan seperti **Orientation** dan **Rotation** telah ditambahkan.

#### Gaya Nomor Khusus untuk Level Daftar <sup>24.7</sup>

Penyetel untuk properti publik [CustomNumberStyleFormat](https://reference.aspose.com/words/cpp/aspose.words.lists/listlevel/get_customnumberstyleformat/) telah ditambahkan. Anda sekarang dapat menentukan gaya angka khusus untuk level daftar.

#### Perubahan dalam bekerja dengan ActiveX <sup>24.7</sup>

- Properti objek ActiveX sekarang dapat dimodifikasi, memberi Anda kontrol lebih besar atas perilakunya.
- Kemampuan untuk mengubah nilai kontrol tombol radio ActiveX untuk mengaktifkan interaksi dinamis telah ditambahkan.
- Kemampuan untuk mengubah ActiveX checkbox menjadi "dicentang " atau" tidak dicentang " telah ditambahkan.

### Memuat dan Menyimpan Dokumen

#### Mengekspor Tautan ke Format Markdown <sup>24.7</sup>

Kemampuan untuk mengontrol ekspor tautan dalam format Markdown telah ditambahkan melalui penerapan properti [LinkExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_linkexportmode/).

### Cari dan Bandingkan

#### Opsi Perbandingan Lanjutan <sup>24.6</sup>

Kemampuan untuk merampingkan alur kerja analisis data dengan fungsionalitas perbandingan yang ditingkatkan telah ditambahkan. Ini termasuk opsi **IgnoreStoreItemId** baru dan antarmuka yang didesain ulang untuk perbandingan lanjutan.

### Lainnya

- Fungsi untuk menghilangkan halaman kosong dari dokumen telah diimplementasikan dengan menambahkan metode [RemoveBlankPages](https://reference.aspose.com/words/cpp/aspose.words/document/removeblankpages/). <sup>24.5</sup>
- Kemampuan untuk memeriksa keberadaan makro VBA tanpa memuat dokumen telah disediakan dengan menambahkan properti **HasMacros**. <sup>24.5</sup>
- Properti **DateTimeUtc** baru telah ditambahkan – ini memberikan stempel waktu yang lebih tepat untuk komentar, meningkatkan organisasi, dan keterlacakan. <sup>24.6</sup>
- Format datetime sekarang secara otomatis terdeteksi untuk ekspor tanpa batas ke format XLSX. <sup>24.7</sup>
- Properti publik [IsProtected](https://reference.aspose.com/words/cpp/aspose.words.vba/vbaproject/get_isprotected/), yang memungkinkan Anda memverifikasi apakah proyek VBA dilindungi, telah ditambahkan. <sup>24.7</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 24.5 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-5-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 24.6 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-6-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 24.7 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-7-release-notes/).

{{% /alert %}}

## Aspose.Words untuk C++ 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 meningkatkan pengalaman seputar pengelolaan warna guratan, menyempurnakan objek OLE, serta memperkenalkan Sumber Bibliografi baru publik API.

Aspose.Words 24.2 Bagan yang diperluas API dan manajemen gaya. Versi Aspose.Words ini juga memperkenalkan kemampuan untuk menentukan SvgSaveOptions selama rendering, kontrol yang lebih fleksibel saat memuat file Markdown, dan bekerja dengan teks referensi untuk catatan kaki dan catatan akhir.

Aspose.Words 24.3 memperkenalkan Emulasi operasi raster biner untuk WMF metafile dan juga terus memperluas Bagan API.

Aspose.Words 24.4 menyempurnakan beberapa opsi rendering, serta meningkatkan pekerjaan dengan tanda tangan digital.

### Rendering dan Pencetakan

#### Kontrol Warna Goresan <sup>24.1</sup>

Kelas [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) telah diperluas dengan sekumpulan properti publik baru yang terkait dengan pengelolaan warna guratan: [ForeThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_forethemecolor/) dan [BackThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_foretintandshade/) dan [BackTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backtintandshade/).

#### DrawingML Bagan API Ekstensi <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** terus diperluas.

#### Sematkan Font yang Dideklarasikan dalam Aturan @font-face <sup>24.4</sup>

Menambahkan kemampuan untuk menyematkan font yang dideklarasikan dalam aturan @font-face ke dalam definisi font dokumen yang dihasilkan telah diperkenalkan dengan menambahkan properti [SupportFontFaceRules](https://reference.aspose.com/words/cpp/aspose.words.loading/htmlloadoptions/get_supportfontfacerules/) baru.

#### Bekerja dengan Pemformatan Cahaya dan Refleksi <sup>24.4</sup>

Kemampuan untuk bekerja dengan pemformatan cahaya dan refleksi untuk objek gambar telah diterapkan.

### Memuat dan Menyimpan Dokumen

#### Tentukan SvgSaveOptions Selama Rendering <sup>24.2</sup>

Kemampuan untuk menentukan [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/) selama rendering telah ditambahkan menggunakan [ShapeRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) dan [OfficeMathRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) metode.

#### Pertahankan Baris Kosong saat Memuat file Markdown <sup>24.2</sup>

Kemampuan untuk mempertahankan baris kosong saat memuat file Markdown telah ditambahkan.

### Lainnya

- Kemampuan untuk memodifikasi teks dari kontrol `TextBox` OLE telah diperkenalkan dengan menambahkan properti **Text** baru ke kelas **TextBoxControl** yang baru. <sup>24.1</sup>
- Bibliography Sources public API diimplementasikan melalui penambahan namespace baru [Aspose.Words.Bibliography](https://reference.aspose.com/words/cpp/aspose.words.bibliography/) dengan kelas dan enumerasi barunya, dan melalui penambahan properti [Bibliography](https://reference.aspose.com/words/cpp/aspose.words/document/get_bibliography/) baru ke kelas [Document](https://reference.aspose.com/words/cpp/aspose.words/document/). <sup>24.1</sup>
- Properti publik baru [Priority](https://reference.aspose.com/words/cpp/aspose.words/style/get_priority/), [UnhideWhenUsed](https://reference.aspose.com/words/cpp/aspose.words/style/get_unhidewhenused/), dan [SemiHidden](https://reference.aspose.com/words/cpp/aspose.words/style/get_semihidden/) untuk manajemen gaya yang disempurnakan telah ditambahkan ke kelas [Style](https://reference.aspose.com/words/cpp/aspose.words/style/). <sup>24.2</sup>
- Fungsionalitas untuk mengambil teks tanda referensi aktual untuk catatan kaki dan catatan akhir telah ditingkatkan dengan properti [ActualReferenceMark](https://reference.aspose.com/words/cpp/aspose.words.notes/footnote/get_actualreferencemark/) dan metode [UpdateActualReferenceMarks](https://reference.aspose.com/words/cpp/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
- Emulasi operasi raster biner untuk WMF metafile telah diterapkan. <sup>24.3</sup>
- Kemampuan untuk menentukan opsi tanda tangan untuk dokumen dalam **SaveOptions** telah diaktifkan dengan menambahkan kelas **DigitalSignatureDetails** baru dengan anggota publik baru, serta menambahkan properti baru ke kelas [OoxmlSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/docsaveoptions/), dan [OdtSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 24.1 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-1-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 24.2 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-2-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 24.3 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-3-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 24.4 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words untuk C++ 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 memperluas opsi rendering, emulasi rendering metafile, dan opsi penyimpanan markdown.

Aspose.Words 23.10 meningkatkan rendering, memperluas opsi untuk memuat dan menyimpan dokumen, dan memungkinkan pengguna menggabungkan dokumen dengan cara baru.

Aspose.Words 23.11 menyempurnakan pekerjaan dengan revisi, format XLSX, dan font pada legenda bagan dengan opsi tambahan.

Aspose.Words 23.12 memperkenalkan properti dan pencacahan baru untuk bekerja dengan dokumen PDF dan OOXML, serta dukungan untuk gambar WebP.

### Rendering dan Pencetakan

#### Menyesuaikan Judul Sumbu dalam Bagan DrawingML <sup>23.9</sup>

Kemampuan untuk menyesuaikan judul sumbu dalam bagan DrawingML telah diperkenalkan dengan penerapan properti kelas publik baru **ChartAxisTitle** dan [Title](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartaxis/get_title/).

#### Menentukan Posisi Vertikal Font dalam sebuah Paragraf <sup>23.9</sup>

Sekarang dimungkinkan untuk menentukan posisi vertikal font dalam paragraf menggunakan properti public [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/paragraphformat/get_baselinealignment/) baru dan enumerasi [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/baselinealignment/) baru.

#### Kontrol Warna Latar Depan <sup>23.10</sup>

Kemampuan untuk mengambil warna latar depan tanpa pengubah telah ditambahkan ke kelas [Fill](https://reference.aspose.com/words/cpp/aspose.words.drawing/fill/) dan [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) melalui properti **BaseForeColor**.

#### Memperluas Fungsionalitas Bagan <sup>23.10</sup>

Fungsionalitas kelas [ChartDataPointCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartseries/), dan [ChartFormat](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartformat/) telah diperluas dengan metode dan properti baru.

#### Secara Otomatis Menyesuaikan dan Menyesuaikan Gambar menjadi Bentuk <sup>23.10</sup>

Cara sederhana untuk menyesuaikan dan menyesuaikan gambar secara otomatis dalam bentuk tertentu telah disediakan melalui metode [FitImageToShape](https://reference.aspose.com/words/cpp/aspose.words.drawing/imagedata/fitimagetoshape/) yang baru.

#### Pemformatan Font Default untuk Entri Legenda Bagan DrawingML <sup>23.11</sup>

Kemampuan untuk menentukan pemformatan font default untuk entri legenda bagan DrawingML telah ditambahkan melalui properti [Font](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartlegend/get_font/). Fitur ini memfasilitasi tampilan yang lebih ramping dan konsisten untuk elemen bagan, meningkatkan estetika dokumen secara keseluruhan.

#### Tentukan Tata Letak Halaman saat Membuka PDF di Pembaca <sup>23.12</sup>

Kemampuan untuk menentukan tata letak halaman yang akan digunakan saat membuka dokumen di pembaca PDF telah ditambahkan melalui pengenalan properti **PageLayout** baru ke kelas [PdfSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/) dan pengenalan pencacahan **PdfPageLayout** baru.

### Memuat dan Menyimpan Dokumen

#### Menentukan Nama Folder untuk Membuat Image URIs dalam Markdown <sup>23.9</sup>

Kelas [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) telah diperluas dengan menyertakan properti [ImagesFolderAlias](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imagesfolderalias/), yang memungkinkan untuk menentukan nama folder yang digunakan untuk membuat gambar URIs yang ditulis ke dalam dokumen Markdown.

#### Kurangi Ukuran Keluaran PDF <sup>23.10</sup>

Berbagai pengoptimalan rendering PDF untuk mengurangi ukuran keluaran saat menggunakan pengaturan [OptimizeOutput](https://reference.aspose.com/words/cpp/aspose.words.saving/fixedpagesaveoptions/get_optimizeoutput/) telah diterapkan.

#### Mengenali Hyperlink saat Memuat Dokumen TXT <sup>23.10</sup>

Fitur untuk mengenali hyperlink saat memuat dokumen TXT telah diterapkan dengan menambahkan properti [DetectHyperlinks](https://reference.aspose.com/words/cpp/aspose.words.loading/txtloadoptions/get_detecthyperlinks/) baru.

### Lainnya

- Emulasi rendering metafile untuk menentukan ukuran rasterisasi telah diterapkan, khususnya untuk lebar pena WMF dan lebar pena kosmetik EMF. Untuk mencapai hal ini, properti **ScaleWmfFontsToMetafileSize** diganti dengan properti [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpage/) dan properti [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpageresolution/) ditambahkan. <sup>23.9</sup>
* Metode yang disederhanakan untuk menyisipkan satu dokumen ke dokumen lain pada posisi kursor saat ini telah diperkenalkan menggunakan metode [InsertDocumentInline](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertdocumentinline/). <sup>23.10</sup>
* Kemampuan untuk mengakses dan memodifikasi properti gaya telah ditambahkan melalui pengenalan properti [Locked](https://reference.aspose.com/words/cpp/aspose.words/style/get_locked/) yang baru. <sup>23.10</sup>
* Parameter tipe generik telah ditambahkan ke metode kelas [CompositeNode](https://reference.aspose.com/words/cpp/aspose.words/compositenode/). <sup>23.10</sup>
* Cara untuk mengontrol kapan revisi tertentu harus diterima / ditolak atau tidak telah diterapkan dengan menggunakan metode [Accept](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/accept/) dan [Reject](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/reject/). Peningkatan ini memberi pengguna kontrol yang lebih baik atas proses revisi. <sup>23.11</sup>
* Kemampuan untuk menulis semua bagian dokumen ke lembar kerja XLSX yang sama telah disediakan melalui tipe enumerasi [XlsxSectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsectionmode/) yang baru dan properti [SectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsaveoptions/get_sectionmode/) yang baru. <sup>23.11</sup>
* Cara untuk mengontrol bagaimana ekstensi format ZIP64 akan digunakan untuk dokumen OOXML telah diterapkan melalui properti Zip64Mode baru dari kelas `OoxmlSaveOptions` dan pencacahan Zip64Mode baru. <sup>23.12</sup>
* Dukungan untuk gambar WebP telah diperkenalkan. Harap dicatat bahwa fitur ini hanya tersedia untuk .versi NetStandart dan .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 23.9 Catatan Rilis](/words/cpp/aspose-words-for-cpp-23-9-release-notes/).
Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 23.10 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-10-release-notes/).
Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 23.11 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-11-release-notes/).
Pelajari lebih lanjut tentang [Aspose.Words untuk C++ 23.12 Catatan Rilis](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-12-release-notes/).

{{% /alert %}}

## Lihat Juga

{{% alert color="primary" %}}

Halaman ini berisi berita rilis terbaru selama 2 tahun terakhir. Untuk detail tentang rilis sebelumnya, lihat [Catatan Rilis'](/words/cpp/release-notes/) halaman di bagian yang relevan.

{{% /alert %}}
