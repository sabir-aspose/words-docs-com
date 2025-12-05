---
title: Apa yang baru
second_title: Aspose.Words untuk Java
articleTitle: Apa yang baru di Aspose.Words untuk Java
linktitle: Apa yang baru di Aspose.Words untuk Java
type: docs
description: "Aspose.Words untuk Java memperluas dan meningkatkan setiap hari. Di halaman ini, Anda dapat mempelajari tentang fitur produk yang sangat besar dan paling menarik."
weight: 2
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /id/java/what-s-new-in-aspose-words-for-java/
timestamp: 2025-06-23-21-02-49
---

Halaman ini menjelaskan fitur Aspose.Words baru yang paling menarik yang diperkenalkan dalam rilis terbaru.

## Aspose.Words untuk Java 25.5, 25.6

Aspose.Words 25.5 menyempurnakan penyesuaian bagan dengan opsi gaya baru dan meningkatkan ekspor Markdown dengan menawarkan kontrol atas penanganan paragraf kosong.

Aspose.Words 25.6 meningkatkan presisi rendering dan fitur visualisasi dengan memperkenalkan opsi ekspor gambar lanjutan, penanganan MathML yang ditingkatkan, dan representasi bagan yang lebih baik.

### Mengonversi, Memuat, dan Menyimpan Dokumen

#### Ekspor Paragraf Kosong ke Markdown <sup>25.5</sup>

Kemampuan untuk mengontrol bagaimana paragraf kosong diekspor ke Markdown telah diperkenalkan dengan menambahkan enumerasi [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownemptyparagraphexportmode/) dan properti [EmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getEmptyParagraphExportMode).

#### Ekspor Dokumen Multi-halaman ke Format Gambar Raster <sup>25.6</sup>

Kemampuan untuk mengekspor dokumen multi-halaman ke format gambar raster (seperti PNG dan JPEG) dengan [customizable layouts](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) - Horizontal, Vertikal, atau Kisi-telah diperkenalkan dengan memperluas fungsionalitas ekspor gambar.

### Rendering

#### Mengatur Gaya Bagan <sup>25.5</sup>

Kemampuan untuk mengatur gaya bagan telah diperkenalkan dengan menambahkan enumerasi [ChartStyle](https://reference.aspose.com/words/java/com.aspose.words/chartstyle/) dan properti [Style](https://reference.aspose.com/words/java/com.aspose.words/chart/#getStyle).

#### Merender Baris Konektor dalam Ekspresi MathML  <sup>25.6</sup>

Rendering garis penghubung dalam ekspresi MathML telah diterapkan untuk memastikan tampilan rumus matematika yang lebih akurat dan konsisten secara visual.

#### Merender Legenda untuk Bagan Air Terjun <sup>25.6</sup>

Rendering legenda untuk ["Waterfall" charts](https://reference.aspose.com/words/java/com.aspose.words/chartseriestype/) telah diperkenalkan, meningkatkan transparansi data, dan meningkatkan interpretabilitas bagan ini.

### Lainnya

* Kemampuan untuk membungkus rumus matematika yang berisi beberapa garis miring telah ditingkatkan, meningkatkan kejelasan tata letak dan keterbacaan rumus. <sup>25.6</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 25.5 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-5-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 25.6 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words untuk Java 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 memperkenalkan pemeriksaan tata bahasa bertenaga AI dan menyempurnakan penyimpanan dokumen dengan opsi lanjutan untuk format HTML, SVG, dan Markdown.

Aspose.Words 25.2 memperkenalkan peringkasan teks dengan model Anthropic AI, menambahkan dukungan format MsWorks, meningkatkan kontrol tipografi, dan meningkatkan struktur PDF dan penanganan daftar.

Aspose.Words 25.3 menyempurnakan pemeriksa tata bahasa dan pemilihan font bertenaga AI dengan properti UpdateAmbiguousTextFont, serta meningkatkan ekspor lampiran PDF.

Aspose.Words 25.4 memperkenalkan dukungan untuk ukuran kertas baru, memungkinkan kontrol ekspor HTML tingkat lanjut, meningkatkan penanganan tanda air, dan meningkatkan kegunaan LowCode API.

### AI-Fitur bertenaga

#### Dokumen AI Pemeriksaan Tata Bahasa

* Kemampuan untuk memeriksa tata bahasa dokumen yang disediakan menggunakan model generatif OpenAI telah diperkenalkan dengan menambahkan metode [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) baru. <sup>25.1</sup>
* Fitur Pemeriksaan Tata Bahasa bertenaga AI telah diperbarui untuk mendukung semua model yang tersedia dalam pencacahan [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). <sup>25.3</sup>

#### Ringkasan Menggunakan Model Bahasa Generatif Anthropic <sup>25.2</sup>

Peringkasan teks menggunakan model bahasa generatif Anthropic telah diaktifkan dengan memperkenalkan kelas publik baru [AnthropicAiModel](https://reference.aspose.com/words/java/com.aspose.words/anthropicaimodel/).

### Low Code

#### Low Code API Kegunaan <sup>25.4</sup>

Peningkatan signifikan pada kegunaan **LowCode API** telah diperkenalkan, menyederhanakan pemrosesan dokumen dan mengurangi kebutuhan akan kode yang berulang.

### Format yang Didukung <sup>25.2</sup>

Mulai dari versi 25.2, kompatibilitas dengan format pemuatan MsWorks baru untuk dokumen Karya Microsoft telah ditambahkan.

### Mengonversi, Memuat, dan Menyimpan Dokumen

#### Peningkatan Penyimpanan ke Format HTML dan SVG <sup>25.1</sup>

Menyimpan ke format HTML dan SVG telah ditingkatkan dengan menambahkan properti **IdPrefix** dan **RemoveJavaScriptFromLinks** ke kelas [HtmlFixedSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlfixedsaveoptions/) dan [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/).

#### Setel Resolusi Gambar dan Mode Keluaran OfficeMath Saat Menyimpan ke Markdown <sup>25.1</sup>

* Opsi [ImageResolution](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImageResolution) baru telah ditambahkan ke kelas [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) untuk mengatur resolusi gambar.
* Opsi [OfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getOfficeMathExportMode) baru dan enumerasi [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownofficemathexportmode/) telah dan ditambahkan ke kelas [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) untuk menyetel mode keluaran OfficeMath.
* Kemampuan untuk menyetel tanda air gambar dari aliran telah diperkenalkan dengan menambahkan kelebihan beban baru ke metode [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.io.InputStream-com.aspose.words.ImageWatermarkOptions). <sup>25.4</sup>

### Rendering

#### Kontrol Tipografi yang Ditingkatkan <sup>25.2</sup>

Properti [NumberSpacing](https://reference.aspose.com/words/java/com.aspose.words/font/#getNumberSpacing) telah ditambahkan untuk kontrol tipografi yang lebih baik.

#### Mengontrol Pemilihan Font untuk Karakter Ambigu <sup>25.3</sup>

Properti publik baru [UpdateAmbiguousTextFont](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/#getUpdateAmbiguousTextFont) telah ditambahkan ke kelas [SaveOptions](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/) untuk mengontrol pemilihan font sesuai dengan kode karakter yang digunakan.

#### Opsi Ukuran Kertas <sup>25.4</sup>

Kemampuan untuk menggunakan ukuran kertas JIS B4 dan JIS B5 telah diperkenalkan dengan menambahkan nilai baru ke enumerasi [PaperSize](https://reference.aspose.com/words/java/com.aspose.words/papersize/).

#### HTML Kontrol Keluaran <sup>25.4</sup>

Kemampuan untuk menghapus JavaScript dari hyperlink URLs selama ekspor HTML telah diperkenalkan dengan menambahkan properti [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/#getRemoveJavaScriptFromLinks).

### Lainnya

* PDF struktur logika telah ditingkatkan dengan dukungan untuk bidang TOA, BIBLIOGRAPHY, dan INDEX. <sup>25.2</sup>
* Metode [AddSingleLevelList](https://reference.aspose.com/words/java/com.aspose.words/listcollection/#addSingleLevelList-int) telah diperkenalkan untuk penanganan daftar yang lebih baik. <sup>25.2</sup>
* Properti baru [AttachmentsEmbeddingMode](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getAttachmentsEmbeddingMode) telah ditambahkan untuk menggantikan **EmbedAttachments** untuk meningkatkan ekspor lampiran PDF. Selain itu, nilai baru telah ditambahkan ke enumerasi [PdfCompliance](https://reference.aspose.com/words/java/com.aspose.words/pdfcompliance/) untuk mendukung lampiran versi PDF/A. Selain itu, lampiran sekarang didukung dengan enkripsi. <sup>25.3</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 25.1 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-1-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 25.2 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-2-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 25.3 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-3-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 25.4 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words untuk Java 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 memperkenalkan penyisipan group shape dan penyisipan StructuredDocumentTag melalui DocumentBuilder, menyempurnakan rendering bagan radial dengan gradasi, meningkatkan tanda tangan digital dengan dukungan XAdES-EPES, menambahkan pengenalan garis bawah Markdown, dan menyediakan akses ke pemisah catatan kaki / catatan akhir.

Aspose.Words 24.10 memperkenalkan dukungan kontrol ActiveX yang ditingkatkan dengan pembuatan CommandButton, kontrol visibilitas bentuk baru, kemampuan untuk group shapes, peningkatan ekspor Markdown untuk tabel, pemformatan bagan untuk bagan Pie dan Doughnut, penanganan penyandian Big5 yang lebih baik, dan dukungan untuk font Taiwan yang sudah ketinggalan zaman.

Aspose.Words 24.11 memperkenalkan peringkasan dokumen bertenaga AI, opsi rendering yang ditingkatkan, peningkatan akses ke properti dokumen, dan teks kontrol ActiveX.

Aspose.Words 24.12 memperkenalkan penempatan label data yang dapat disesuaikan, terjemahan teks bertenaga Google AI, opsi pembersihan Mail Merge yang disempurnakan, dan kelas pemrosesan LowCode baru.

### AI-Fitur bertenaga

#### Ringkasan Dokumen Menggunakan OpenAI dan Google <sup>24.11</sup>

Dukungan untuk peringkasan dokumen menggunakan model bahasa generatif **OpenAI** dan **Google** telah terintegrasi.

#### Terjemahan teks menggunakan model bahasa generatif Google <sup>24.12</sup>

Kemampuan untuk menerjemahkan teks menggunakan model bahasa generatif Google telah diterapkan di Aspose.Words dengan menambahkan metode [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) dan pencacahan [Language](https://reference.aspose.com/words/java/com.aspose.words/language/).

### Low Code <sup>24.12</sup>

Kelas LowCode baru seperti [Comparer](https://reference.aspose.com/words/java/com.aspose.words/comparer/), [MailMerger](https://reference.aspose.com/words/java/com.aspose.words/mailmerger/), [Replacer](https://reference.aspose.com/words/java/com.aspose.words/replacer/), [Splitter](https://reference.aspose.com/words/java/com.aspose.words/splitter/) dll. telah diperkenalkan, menawarkan serangkaian metode yang memberikan keseimbangan sempurna antara kesederhanaan dan fleksibilitas untuk pemrosesan dokumen.

### Rendering dan Pencetakan

#### Kelulusan pada Grafik Radial <sup>24.9</sup>

Rendering gradasi pada grafik radial telah diterapkan.

#### CommandButton ActiveX Kontrol <sup>24.10</sup>

Kemampuan untuk membuat kontrol CommandButton ActiveX telah diperkenalkan dengan menambahkan metode publik baru [InsertForms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertForms2OleControl-com.aspose.words.Forms2OleControl) dan kelas publik baru [Forms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/).

#### Kontrol Visibilitas Bentuk <sup>24.10</sup>

Properti publik baru [Hidden](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#getHidden) telah ditambahkan untuk mengontrol visibilitas bentuk.

#### Perubahan pada Bagan Pie dan Doughnut <sup>24.10</sup>

Beberapa properti publik baru telah ditambahkan ke bagan format Pie dan Doughnut.

#### Kontrol Rendering Batas Bidang Formulir Pilihan PDF <sup>24.11</sup>

Opsi baru untuk mengontrol rendering batas bidang formulir pilihan PDF telah diterapkan dengan menambahkan opsi publik baru [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getRenderChoiceFormFieldBorder).

#### Dapatkan dan Atur Kode Format untuk Data Bagan <sup>24.11</sup>

Kemampuan untuk mendapatkan dan mengatur kode format untuk data bagan telah ditambahkan dengan menerapkan properti [FormatCode](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/#getFormatCode) di kelas [ChartXValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartyvaluecollection/), dan [BubbleSizeCollection](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/).

#### Render Bagan Histogram dengan Tempat Sampah dan Label <sup>24.11</sup>

Rendering grafik histogram telah ditingkatkan dengan memungkinkan sejumlah tempat sampah dan label tertentu.

### Mengonversi, Memuat, dan Menyimpan Dokumen

#### Garis Bawahi Pemformatan saat Memuat File Markdown <sup>24.9</sup>

Opsi untuk mengenali pemformatan garis bawah saat memuat dokumen Markdown telah digabungkan dengan menambahkan properti publik baru [ImportUnderlineFormatting](https://reference.aspose.com/words/java/com.aspose.words/markdownloadoptions/#getImportUnderlineFormatting).

#### Mengekspor tabel sebagai HTML saat menyimpan ke Markdown <sup>24.10</sup>

Opsi untuk mengekspor tabel sebagai HTML saat menyimpan dokumen ke format Markdown telah diterapkan dengan menambahkan properti publik baru [ExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getExportAsHtml) dan enumerasi [MarkdownExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownexportashtml/).

#### Ekspor PDF dengan Struktur Logika yang Diperbarui <sup>24.11</sup>

Ekspor PDF telah ditingkatkan dengan menyertakan properti judul tabel sebagai judul elemen struktur logis PDF.

### Mail Merge dan Pelaporan

#### Hapus Tabel Kosong selama Mail Merge <sup>24.12</sup>

Opsi **RemoveEmptyTables** baru telah ditambahkan ke enumerasi [MailMergeCleanupOptions](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/) untuk menyempurnakan keluaran Mail Merge.

### Tanda Tangan Digital

#### Tanda tangani Dokumen dengan XAdES-EPES <sup>24.9</sup>

Kemampuan untuk menandatangani dokumen dengan tanda tangan XAdES-EPES level XML-DSig telah diperkenalkan dengan menambahkan properti publik baru [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/signoptions/#getXmlDsigLevel) dan pencacahan publik baru [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/xmldsiglevel/)

### Lainnya

* Metode publik baru [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-com.aspose.words.Shape...) telah ditambahkan ke group shapes. <sup>24.9</sup>
* Metode publik baru [InsertStructuredDocumentTag](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertStructuredDocumentTag-int) telah ditambahkan untuk menyisipkan **StructuredDocumentTags** ke dalam dokumen. <sup>24.9</sup>
* Akses publik ke pemisah catatan kaki / catatan akhir telah disediakan dengan menambahkan beberapa kelas dan properti publik. <sup>24.9</sup>
* Kemampuan untuk mengelompokkan masing-masing bentuk, group shapes bersama-sama, dan langsung mengelompokkan kedua bentuk dan group shapes telah diperkenalkan dengan menambahkan metode [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-double-double-double-double-com.aspose.words.ShapeBase...). <sup>24.10</sup>
* Penanganan penyandian Big5 untuk tabel cmap TrueType telah ditingkatkan. <sup>24.10</sup>
* Dukungan untuk font Taiwan yang sudah ketinggalan zaman telah ditingkatkan. <sup>24.10</sup>
* Untuk mengakses properti dokumen yang diperluas, properti hanya-baca telah ditambahkan ke kelas [BuiltInDocumentProperties](https://reference.aspose.com/words/java/com.aspose.words/builtindocumentproperties/). <sup>24.11</sup>
* Menyetel teks untuk kontrol ActiveX telah diaktifkan dengan menambahkan penyetel publik baru ke properti [Forms2OleControl.Caption](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/#getCaption). <sup>24.11</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.9 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-9-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.10 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-10-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.11 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-11-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.12 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words untuk Java 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 memperluas opsi untuk rakitan, meningkatkan kemampuan rendering, dan memperluas beberapa opsi lainnya.

Aspose.Words 24.6 meningkatkan opsi rendering, meningkatkan fungsionalitas penelusuran dan perbandingan, dan memperluas beberapa fitur lainnya.

Aspose.Words 24.7 mengubah cara Anda bekerja dengan ActiveX, memperluas kemampuan rendering, serta mengekspor ke format Markdown dan XLSX.

Aspose.Words 24.8 meningkatkan penyesuaian bagan dengan kontrol presisi atas label sumbu, memperluas manajemen font, meningkatkan penanganan struktur dokumen, dan menambahkan kemampuan baru untuk ekspor HTML / XAML, fungsionalitas PDF, konversi dokumen, dan tanda tangan digital.

### Format yang Didukung

Mulai dari versi 24.7, ekspor ke PDF/UA-2 didukung untuk memastikan aksesibilitas bagi pengguna penyandang disabilitas.

### Rendering dan Pencetakan

#### Perubahan Bagan, Bentuk, dan DrawingML <sup>24.5</sup>

- DrawingML rendering efek untuk grafik SVG, memperluas fungsionalitas sebelumnya yang terbatas pada gambar, telah diterapkan.
- Dukungan untuk membuat bagan kombo dan menyesuaikan properti seperti lebar celah, tumpang tindih, dan skala gelembung dalam grup deret telah diperkenalkan dengan menambahkan kelas [ChartSeriesGroup](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroup/) dan [ChartSeriesGroupCollection](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroupcollection/) dan properti [SeriesGroups](https://reference.aspose.com/words/java/com.aspose.words/chart/#getSeriesGroups).
- Fungsionalitas untuk memanipulasi efek SoftEdge dari bentuk telah diimplementasikan dengan menambahkan kelas [SoftEdgeFormat](https://reference.aspose.com/words/java/com.aspose.words/softedgeformat/).
- Kemampuan untuk memodifikasi nilai adjust dari bentuk telah diimplementasikan dengan menambahkan kelas publik [AdjustmentCollection](https://reference.aspose.com/words/java/com.aspose.words/adjustmentcollection/) dan [Adjustment](https://reference.aspose.com/words/java/com.aspose.words/adjustment/) dan properti [Adjustments](https://reference.aspose.com/words/java/com.aspose.words/shape/#getAdjustments).

#### Perubahan Bagan, Bentuk, dan Gambar <sup>24.6</sup>

- Kemampuan pembuatan bagan telah ditingkatkan. Anda sekarang dapat membuat variasi bagan yang lebih luas, termasuk *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* bagan, bagan *Box & Whisker*, *Waterfalls*, dan *Funnels*. Ini memungkinkan Anda untuk memvisualisasikan data Anda dengan cara yang lebih beragam dan informatif.
- Kontrol warna untuk pemformatan bayangan telah ditingkatkan. Anda dapat memperoleh kontrol yang lebih tepat atas tampilan dokumen Anda dengan mengakses warna bayangan.
- Peningkatan kinerja untuk rendering latar belakang telah ditingkatkan. Anda dapat mempercepat rendering latar belakang yang berisi elemen kecil secara signifikan berkat teknologi ubin asli.
- Gradien realistis untuk bentuk telah ditambahkan. Anda sekarang dapat membuat bentuk DML dengan gradien non-linier, meniru gaya visual Microsoft Word untuk tampilan yang lebih halus.

#### Kustomisasi Label Data Bagan <sup>24.7</sup>

Kemampuan untuk menyesuaikan label data bagan seperti **Orientation** dan **Rotation** telah ditambahkan.

#### Gaya Nomor Khusus untuk Level Daftar <sup>24.7</sup>

Penyetel untuk properti publik [CustomNumberStyleFormat](https://reference.aspose.com/words/java/com.aspose.words/listlevel/#getCustomNumberStyleFormat) telah ditambahkan. Anda sekarang dapat menentukan gaya angka khusus untuk level daftar.

#### Perubahan dalam bekerja dengan ActiveX <sup>24.7</sup>

* Properti objek ActiveX sekarang dapat dimodifikasi, memberi Anda kontrol lebih besar atas perilakunya.
* Kemampuan untuk mengubah nilai kontrol tombol radio ActiveX untuk mengaktifkan interaksi dinamis telah ditambahkan.
* Kemampuan untuk mengubah ActiveX checkbox menjadi "dicentang " atau" tidak dicentang " telah ditambahkan.

#### Kontrol Atas Sumbu Bagan Centang Label Orientasi dan Rotasi <sup>24.8</sup>

Kontrol yang tepat atas orientasi dan rotasi label centang sumbu bagan telah ditambahkan untuk penyesuaian bagan yang lebih nyaman-kelas [AxisTickLabels](https://reference.aspose.com/words/java/com.aspose.words/axisticklabels/) telah diperluas dengan properti **Orientation** dan **Rotation** yang baru.

#### Mengganti Garis Miring Terbalik dengan Tanda Yen <sup>24.8</sup>

Ekspor HTML dan XAML yang kompatibel ke belakang untuk mengganti karakter garis miring terbalik dengan tanda Yen telah ditingkatkan. Untuk mencapai hal ini, properti **ReplaceBackslashWithYenSign** telah ditambahkan ke kelas [HtmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/) dan [XamlFlowSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/).

#### Menggunakan Tag SDT sebagai Nama Bidang Formulir saat Mengekspor ke PDF <sup>24.8</sup>

Ekspor PDF dengan dukungan untuk menggunakan tag SDT sebagai nama bidang formulir telah ditingkatkan dengan menambahkan properti **UseSdtTagAsFormFieldName** baru ke kelas [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/).

### Mengonversi, Memuat, dan Menyimpan Dokumen

#### Mengekspor Tautan ke Format Markdown <sup>24.7</sup>

Kemampuan untuk mengontrol ekspor tautan dalam format Markdown telah ditambahkan melalui penerapan properti [LinkExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getLinkExportMode).

#### LowCode 24.8 <sup>24.8</sup>

Kelas **LowCode.Converter** baru, yang dirancang untuk menyediakan serangkaian metode untuk mengonversi berbagai jenis dokumen dengan satu baris kode, telah diperkenalkan.

### Cari dan Bandingkan

#### Opsi Perbandingan Lanjutan <sup>24.6</sup>

Kemampuan untuk merampingkan alur kerja analisis data dengan fungsionalitas perbandingan yang ditingkatkan telah ditambahkan. Ini termasuk opsi [IgnoreStoreItemId](https://reference.aspose.com/words/java/com.aspose.words/advancedcompareoptions/#getIgnoreStoreItemId) baru dan antarmuka yang didesain ulang untuk perbandingan lanjutan.

### Lainnya

* Fungsi untuk menghilangkan halaman kosong dari dokumen telah diimplementasikan dengan menambahkan metode [RemoveBlankPages](https://reference.aspose.com/words/java/com.aspose.words/document/#removeBlankPages). <sup>24.5</sup>
* Kemampuan untuk memeriksa keberadaan makro VBA tanpa memuat dokumen telah disediakan dengan menambahkan properti [HasMacros](https://reference.aspose.com/words/java/com.aspose.words/fileformatinfo/#hasMacros). <sup>24.5</sup>
* Mempertahankan penomoran sumber saat menyisipkan dokumen menggunakan Mesin Pelaporan LINQ sekarang didukung. <sup>24.5</sup>
* Properti [DateTimeUtc](https://reference.aspose.com/words/java/com.aspose.words/comment/#getDateTimeUtc) baru telah ditambahkan – ini memberikan stempel waktu yang lebih tepat untuk komentar, meningkatkan organisasi, dan keterlacakan. <sup>24.6</sup>
* Mesin Pelaporan LINQ telah ditingkatkan. Penghapusan selektif paragraf kosong dan definisi pesan khusus untuk anggota objek yang hilang telah dibuat, menghasilkan laporan yang lebih bersih dan informatif. <sup>24.6</sup>
* Format datetime sekarang secara otomatis terdeteksi untuk ekspor tanpa batas ke format XLSX. <sup>24.7</sup>
* Properti publik [IsProtected](https://reference.aspose.com/words/java/com.aspose.words/vbaproject/#isProtected), yang memungkinkan Anda memverifikasi apakah proyek VBA dilindungi, telah ditambahkan. <sup>24.7</sup>
* Informasi font telah diperluas dengan properti **EmbeddingLicensingRights** ditambahkan ke kelas [FontInfo](https://reference.aspose.com/words/java/com.aspose.words/fontinfo/) dan [PhysicalFontInfo](https://reference.aspose.com/words/java/com.aspose.words/physicalfontinfo/). <sup>24.8</sup>
* Cara untuk menghapus header dan footer bagian secara efisien sambil mempertahankan tanda air telah ditambahkan untuk bekerja lebih akurat dengan struktur dokumen. Untuk menghapus header dan footer bagian, gunakan metode publik baru **ClearHeadersFooters**. <sup>24.8</sup>
* Penandatanganan digital dokumen XPS menggunakan [XpsSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xpssaveoptions/) telah diaktifkan-properti baru **DigitalSignatureDetails** telah ditambahkan untuk tujuan ini. <sup>24.8</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.5 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-5-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.6 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-6-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.7 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-7-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.8 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words untuk Java 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 meningkatkan pengalaman seputar pengelolaan warna guratan, menyempurnakan objek OLE dan pelaporan LINQ, serta memperkenalkan Sumber Bibliografi baru publik API.

Aspose.Words 24.2 Bagan yang diperluas API, manajemen gaya, dan opsi LINQ. Versi Aspose.Words ini juga memperkenalkan kemampuan untuk menentukan SvgSaveOptions selama rendering, kontrol yang lebih fleksibel saat memuat file Markdown, dan bekerja dengan teks referensi untuk catatan kaki dan catatan akhir.

Aspose.Words 24.3 memperkenalkan Pembaca/Penulis TIFF baru dan Meniru operasi raster biner untuk WMF metafile. Aspose.Words 24.3 juga terus memperluas Bagan API.

Aspose.Words 24.4 meningkatkan format penyimpanan, beberapa opsi rendering, serta meningkatkan pekerjaan dengan tanda tangan digital.

### Format yang Didukung <sup>24.4</sup>

Format gambar **WebP** modern sekarang didukung dalam Aspose.Words. Anda sekarang dapat membaca dan menyisipkan gambar WebP ke dalam dokumen, serta menyimpan gambar dalam format WebP.

### Rendering dan Pencetakan

#### Kontrol Warna Goresan <sup>24.1</sup>

Kelas [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) telah diperluas dengan sekumpulan properti publik baru yang terkait dengan pengelolaan warna guratan: [ForeThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeThemeColor) dan [BackThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackThemeColor), [ForeTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeTintAndShade) dan [BackTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackTintAndShade).

#### DrawingML Bagan API Ekstensi <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** terus diperluas.

#### Sematkan Font yang Dideklarasikan dalam Aturan @font-face <sup>24.4</sup>

Menambahkan kemampuan untuk menyematkan font yang dideklarasikan dalam aturan @font-face ke dalam definisi font dokumen yang dihasilkan telah diperkenalkan dengan menambahkan properti [SupportFontFaceRules](https://reference.aspose.com/words/java/com.aspose.words/htmlloadoptions/#getSupportFontFaceRules) baru.

#### Bekerja dengan Pemformatan Cahaya dan Refleksi <sup>24.4</sup>

Kemampuan untuk bekerja dengan pemformatan cahaya dan refleksi untuk objek gambar telah diterapkan.

### Memuat dan Menyimpan Dokumen

#### Tentukan SvgSaveOptions Selama Rendering <sup>24.2</sup>

Kemampuan untuk menentukan [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/) selama rendering telah ditambahkan menggunakan [ShapeRenderer](https://reference.aspose.com/words/java/com.aspose.words/shaperenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) dan [OfficeMathRenderer](https://reference.aspose.com/words/java/com.aspose.words/officemathrenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) metode.

#### Pertahankan Baris Kosong saat Memuat file Markdown <sup>24.2</sup>

Kemampuan untuk mempertahankan baris kosong saat memuat file Markdown telah ditambahkan.

#### Pembaca/Penulis TIFF Baru <sup>24.3</sup>

Pembaca/penulis TIFF baru untuk Aspose.Words untuk .NET Standard, .NET 6 dan yang lebih baru telah dikembangkan. Aspose.Words untuk .NET 24.3 menambahkan dukungan untuk membaca gambar TIFF dengan tipe kompresi JPEG dan JPEG Lama, dan juga meningkatkan kualitas operasi baca dan tulis secara signifikan.

### Lainnya

* Kemampuan untuk memodifikasi teks dari kontrol `TextBox` OLE telah diperkenalkan dengan menambahkan properti [Text](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/#getText) baru ke kelas [TextBoxControl](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/) yang baru. 24.1 <sup>24.1</sup>
* Sumber Bibliografi publik API diimplementasikan dengan menambahkan beberapa sumber baru [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/bibliography/), [Source](https://reference.aspose.com/words/java/com.aspose.words/source/), [ContributorCollection](https://reference.aspose.com/words/java/com.aspose.words/contributorcollection/), [Contributor](https://reference.aspose.com/words/java/com.aspose.words/contributor/), [Corporate](https://reference.aspose.com/words/java/com.aspose.words/corporate/), [PersonCollection](https://reference.aspose.com/words/java/com.aspose.words/personcollection/) dan kelas [Person](https://reference.aspose.com/words/java/com.aspose.words/person/) dan pencacahan [SourceType](https://reference.aspose.com/words/java/com.aspose.words/sourcetype/), serta dengan menambahkan properti [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/document/#getBibliography) baru ke kelas [Document](https://reference.aspose.com/words/java/com.aspose.words/document/). <sup>24.1</sup>
* Sebuah API untuk membatasi akses ke anggota tipe menggunakan sintaks templat untuk Mesin Pelaporan LINQ telah disediakan. <sup>24.1</sup>
* Properti publik baru [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/), dan [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) untuk manajemen gaya yang disempurnakan telah ditambahkan ke kelas [Style](https://reference.aspose.com/words/net/aspose.words/style/). <sup>24.2</sup>
* Fungsionalitas untuk mengambil teks tanda referensi aktual untuk catatan kaki dan catatan akhir telah ditingkatkan dengan properti [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) dan metode [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* Kompatibilitas dengan bagan `Word 2016` untuk `LINQ Reporting Engine` telah diaktifkan. <sup>24.2</sup>
* Emulasi operasi raster biner untuk WMF metafile telah diterapkan. <sup>24.3</sup>
* Kemampuan untuk menentukan opsi tanda tangan untuk dokumen dalam **SaveOptions** telah diaktifkan dengan menambahkan kelas [DigitalSignatureDetails](https://reference.aspose.com/words/java/com.aspose.words/digitalsignaturedetails/) baru dengan anggota publik baru, serta menambahkan properti baru ke kelas [OoxmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/docsaveoptions/), dan [OdtSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.1 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-1-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.2 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-2-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.3 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-3-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 24.4 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words untuk Java 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 memperluas opsi rendering, emulasi rendering metafile, dan opsi penyimpanan markdown.

Aspose.Words 23.10 meningkatkan rendering, memperluas opsi untuk memuat dan menyimpan dokumen, dan memungkinkan pengguna menggabungkan dokumen dengan cara baru.

Aspose.Words 23.11 menyempurnakan pekerjaan dengan revisi, format XLSX, dan font pada legenda bagan dengan opsi tambahan.

Aspose.Words 23.12 memperkenalkan properti dan pencacahan baru untuk bekerja dengan dokumen PDF, dukungan untuk gambar WebP, dan pustaka Bouncy Castle yang diperbarui.

### Rendering dan Pencetakan

#### Menyesuaikan Judul Sumbu dalam Bagan DrawingML <sup>23.9</sup>

Kemampuan untuk menyesuaikan judul sumbu dalam bagan DrawingML telah diperkenalkan dengan penerapan properti kelas publik baru [ChartAxisTitle](https://reference.aspose.com/words/java/com.aspose.words/chartaxistitle/) dan [Title](https://reference.aspose.com/words/java/com.aspose.words/chartaxis/#getTitle).

#### Menentukan Posisi Vertikal Font dalam sebuah Paragraf <sup>23.9</sup>

Sekarang dimungkinkan untuk menentukan posisi vertikal font dalam paragraf menggunakan properti public [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getBaselineAlignment) baru dan enumerasi [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/baselinealignment/) baru.

#### Kontrol Warna Latar Depan <sup>23.10</sup>

Kemampuan untuk mengambil warna latar depan tanpa pengubah telah ditambahkan ke kelas [Fill](https://reference.aspose.com/words/java/com.aspose.words/fill/) dan [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) melalui properti **BaseForeColor**.

#### Memperluas Fungsionalitas Bagan <sup>23.10</sup>

Fungsionalitas kelas [ChartDataPointCollection](https://reference.aspose.com/words/java/com.aspose.words/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/java/com.aspose.words/chartseries/), dan [ChartFormat](https://reference.aspose.com/words/java/com.aspose.words/chartformat/) telah diperluas dengan metode dan properti baru.

#### Secara Otomatis Menyesuaikan dan Menyesuaikan Gambar menjadi Bentuk <sup>23.10</sup>

Cara sederhana untuk menyesuaikan dan menyesuaikan gambar secara otomatis dalam bentuk tertentu telah disediakan melalui metode [FitImageToShape](https://reference.aspose.com/words/java/com.aspose.words/imagedata/#fitImageToShape) yang baru.

#### Pemformatan Font Default untuk Entri Legenda Bagan DrawingML <sup>23.11</sup>

Kemampuan untuk menentukan pemformatan font default untuk entri legenda bagan DrawingML telah ditambahkan melalui properti **Font**. Fitur ini memfasilitasi tampilan yang lebih ramping dan konsisten untuk elemen bagan, meningkatkan estetika dokumen secara keseluruhan.

#### Tentukan Tata Letak Halaman saat Membuka PDF di Pembaca <sup>23.12</sup>

Kemampuan untuk menentukan tata letak halaman yang akan digunakan saat membuka dokumen di pembaca PDF telah ditambahkan melalui pengenalan properti [PageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getPageLayout) baru ke kelas [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/) dan pengenalan pencacahan [PdfPageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfpagelayout/) baru.

### Memuat dan Menyimpan Dokumen

#### Menentukan Nama Folder untuk Membuat Image URIs dalam Markdown <sup>23.9</sup>

Kelas [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) telah diperluas dengan menyertakan properti [ImagesFolderAlias](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImagesFolderAlias), yang memungkinkan untuk menentukan nama folder yang digunakan untuk membuat gambar URIs yang ditulis ke dalam dokumen Markdown.

#### Kurangi Ukuran Keluaran PDF <sup>23.10</sup>

Berbagai pengoptimalan rendering PDF untuk mengurangi ukuran keluaran saat menggunakan pengaturan [OptimizeOutput](https://reference.aspose.com/words/java/com.aspose.words/fixedpagesaveoptions/#getOptimizeOutput) telah diterapkan.

#### Mengenali Hyperlink saat Memuat Dokumen TXT <sup>23.10</sup>

Fitur untuk mengenali hyperlink saat memuat dokumen TXT telah diterapkan dengan menambahkan properti [DetectHyperlinks](https://reference.aspose.com/words/java/com.aspose.words/txtloadoptions/#getDetectHyperlinks) baru.

### Lainnya

- Emulasi rendering metafile untuk menentukan ukuran rasterisasi telah diterapkan, khususnya untuk lebar pena WMF dan lebar pena kosmetik EMF. Untuk mencapai hal ini, properti **ScaleWmfFontsToMetafileSize** diganti dengan properti [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPage) dan properti [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPageResolution) ditambahkan. <sup>23.9</sup>
- Metode yang disederhanakan untuk menyisipkan satu dokumen ke dokumen lain pada posisi kursor saat ini telah diperkenalkan menggunakan metode [InsertDocumentInline](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertDocumentInline-com.aspose.words.Document-int-com.aspose.words.ImportFormatOptions). <sup>23.10</sup>
- Kemampuan untuk mengakses dan memodifikasi properti gaya telah ditambahkan melalui pengenalan properti [Locked](https://reference.aspose.com/words/java/com.aspose.words/style/#getLocked) yang baru. <sup>23.10</sup>
- Parameter tipe generik telah ditambahkan ke metode kelas [CompositeNode](https://reference.aspose.com/words/java/com.aspose.words/compositenode/). <sup>23.10</sup>
- Cara untuk mengontrol kapan revisi tertentu harus diterima / ditolak atau tidak telah diterapkan dengan menggunakan metode [Accept](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#accept-com.aspose.words.IRevisionCriteria) dan [Reject](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#reject-com.aspose.words.IRevisionCriteria). Peningkatan ini memberi pengguna kontrol yang lebih baik atas proses revisi. <sup>23.11</sup>
- Kemampuan untuk menulis semua bagian dokumen ke lembar kerja XLSX yang sama telah disediakan melalui tipe enumerasi [XlsxSectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsectionmode/) yang baru dan properti [SectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/#getSectionMode) yang baru. <sup>23.11</sup>
- Dukungan untuk gambar WebP telah diperkenalkan. Harap dicatat bahwa fitur ini hanya tersedia untuk .versi NetStandart dan .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 23.9 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-9-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 23.10 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-10-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 23.11 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-11-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Java 23.12 Catatan Rilis](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-12-release-notes/).

{{% /alert %}}

## Lihat Juga

{{% alert color="primary" %}}

Halaman ini berisi berita rilis terbaru selama 2 tahun terakhir. Untuk detail tentang rilis sebelumnya, lihat [Catatan Rilis'](https://releases.aspose.com/words/java/release-notes/) halaman di bagian yang relevan.

{{% /alert %}}
