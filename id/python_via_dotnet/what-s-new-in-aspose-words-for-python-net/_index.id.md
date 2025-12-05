---
title: Apa yang baru
second_title: Aspose.Words untuk Python via .NET
articleTitle: Apa yang baru di Aspose.Words untuk Python via .NET
linktitle: Apa yang baru di Aspose.Words untuk Python via .NET
type: docs
description: "Aspose.Words untuk Python via .NET memperluas dan meningkatkan setiap hari. Di halaman ini, Anda dapat mempelajari tentang fitur produk yang sangat besar dan paling menarik."
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /id/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-06-23-21-02-49
---

Halaman ini menjelaskan fitur Aspose.Words baru yang paling menarik yang diperkenalkan dalam rilis terbaru.

## Aspose.Words untuk Python via .NET 25.5, 25.6

Aspose.Words 25.5 menyempurnakan penyesuaian bagan dengan opsi gaya baru dan meningkatkan ekspor Markdown dengan menawarkan kontrol atas penanganan paragraf kosong.

Aspose.Words 25.6 meningkatkan presisi rendering dan fitur visualisasi dengan memperkenalkan opsi ekspor gambar lanjutan, penanganan MathML yang ditingkatkan, dan representasi bagan yang lebih baik.

### Mengonversi, Memuat, dan Menyimpan Dokumen

#### Ekspor Paragraf Kosong ke Markdown <sup>25.5</sup>

Kemampuan untuk mengontrol bagaimana paragraf kosong diekspor ke Markdown telah diperkenalkan dengan menambahkan enumerasi **MarkdownEmptyParagraphExportMode** dan properti **empty_paragraph_export_mode**.

#### Ekspor Dokumen Multi-halaman ke Format Gambar Raster <sup>25.6</sup>

Kemampuan untuk mengekspor dokumen multi-halaman ke format gambar raster (seperti PNG dan JPEG) dengan [customizable layouts](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) - Horizontal, Vertikal, atau Kisi-telah diperkenalkan dengan memperluas fungsionalitas ekspor gambar.

### Rendering

#### Mengatur Gaya Bagan <sup>25.5</sup>

Kemampuan untuk mengatur gaya bagan telah diperkenalkan dengan menambahkan enumerasi **ChartStyle** dan properti **style**.

#### Merender Baris Konektor dalam Ekspresi MathML  <sup>25.6</sup>

Rendering garis penghubung dalam ekspresi MathML telah diterapkan untuk memastikan tampilan rumus matematika yang lebih akurat dan konsisten secara visual.

#### Merender Legenda untuk Bagan Air Terjun <sup>25.6</sup>

Rendering legenda untuk ["Waterfall" charts](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriestype/) telah diperkenalkan, meningkatkan transparansi data, dan meningkatkan interpretabilitas bagan ini.

### Lainnya

* Kemampuan untuk membungkus rumus matematika yang berisi beberapa garis miring telah ditingkatkan, meningkatkan kejelasan tata letak dan keterbacaan rumus. <sup>25.6</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 25.5 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-5-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 25.6 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words untuk Python melalui .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 memperkenalkan pemeriksaan tata bahasa bertenaga AI dan menyempurnakan penyimpanan dokumen dengan opsi lanjutan untuk format HTML, SVG, dan Markdown.

Aspose.Words 25.2 memperkenalkan peringkasan teks dengan model Anthropic AI, menambahkan dukungan format MsWorks, meningkatkan kontrol tipografi, dan meningkatkan struktur PDF dan penanganan daftar.

Aspose.Words 25.3 menyempurnakan pemeriksa tata bahasa dan pemilihan font bertenaga AI dengan properti UpdateAmbiguousTextFont, serta meningkatkan ekspor lampiran PDF.

Aspose.Words 25.4 memperkenalkan dukungan untuk ukuran kertas baru, memungkinkan kontrol ekspor HTML tingkat lanjut, dan meningkatkan penanganan tanda air.

### AI-Fitur bertenaga

#### Dokumen AI Pemeriksaan Tata Bahasa

* Kemampuan untuk memeriksa tata bahasa dokumen yang disediakan menggunakan model generatif OpenAI telah diperkenalkan dengan menambahkan metode [check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/) baru. <sup>25.1</sup>
* Fitur Pemeriksaan Tata Bahasa bertenaga AI telah diperbarui untuk mendukung semua model yang tersedia dalam pencacahan [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Ringkasan Menggunakan Model Bahasa Generatif Anthropic <sup>25.2</sup>

Peringkasan teks menggunakan model bahasa generatif Anthropic telah diaktifkan dengan memperkenalkan kelas publik baru [AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/).

### Format yang Didukung <sup>25.2</sup>

Mulai dari versi 25.2, kompatibilitas dengan format pemuatan MsWorks baru untuk dokumen Karya Microsoft telah ditambahkan.

### Mengonversi, Memuat, dan Menyimpan Dokumen

#### Peningkatan Penyimpanan ke Format HTML dan SVG <sup>25.1</sup>

Menyimpan ke format HTML dan SVG telah ditingkatkan dengan menambahkan properti **id_prefix** dan **remove_java_script_from_links** ke kelas [HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/) dan [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/).

#### Setel Resolusi Gambar dan Mode Keluaran OfficeMath Saat Menyimpan ke Markdown <sup>25.1</sup>

* Opsi [image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/) baru telah ditambahkan ke kelas [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) untuk mengatur resolusi gambar.
* Opsi [office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/) baru dan enumerasi [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/) telah dan ditambahkan ke kelas [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) untuk menyetel mode keluaran OfficeMath.

### Rendering

#### Kontrol Tipografi yang Ditingkatkan <sup>25.2</sup>

Properti [number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/) telah ditambahkan untuk kontrol tipografi yang lebih baik.

#### Mengontrol Pemilihan Font untuk Karakter Ambigu <sup>25.3</sup>

Properti publik baru [update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/) telah ditambahkan ke kelas [SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/) untuk mengontrol pemilihan font sesuai dengan kode karakter yang digunakan.

#### Opsi Ukuran Kertas <sup>25.4</sup>

Kemampuan untuk menggunakan ukuran kertas JIS B4 dan JIS B5 telah diperkenalkan dengan menambahkan nilai baru ke enumerasi [PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/).

#### HTML Kontrol Keluaran <sup>25.4</sup>

Kemampuan untuk menghapus JavaScript dari hyperlink URLs selama ekspor HTML telah diperkenalkan dengan menambahkan properti [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/).

### Lainnya

* PDF struktur logika telah ditingkatkan dengan dukungan untuk bidang TOA, BIBLIOGRAPHY, dan INDEX. <sup>25.2</sup>
* Metode [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate) telah diperkenalkan untuk penanganan daftar yang lebih baik. <sup>25.2</sup>
* Properti baru [attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/) telah ditambahkan untuk menggantikan **EmbedAttachments** untuk meningkatkan ekspor lampiran PDF. Selain itu, nilai baru telah ditambahkan ke enumerasi [PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/) untuk mendukung lampiran versi PDF/A. Selain itu, lampiran sekarang didukung dengan enkripsi. <sup>25.3</sup>
* Kemampuan untuk menyetel tanda air gambar dari aliran telah diperkenalkan dengan menambahkan kelebihan beban baru ke metode [SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions). <sup>25.4</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 25.1 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 25.2 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 25.3 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 25.4 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words untuk Python melalui .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 memperkenalkan penyisipan group shape dan penyisipan StructuredDocumentTag melalui DocumentBuilder, menyempurnakan rendering bagan radial dengan gradasi, meningkatkan tanda tangan digital dengan dukungan XAdES-EPES, menambahkan pengenalan garis bawah Markdown, dan menyediakan akses ke pemisah catatan kaki / catatan akhir.

Aspose.Words 24.10 memperkenalkan dukungan kontrol ActiveX yang ditingkatkan dengan pembuatan CommandButton, kontrol visibilitas bentuk baru, kemampuan untuk group shapes, peningkatan ekspor Markdown untuk tabel, pemformatan bagan untuk bagan Pie dan Doughnut, penanganan penyandian Big5 yang lebih baik, dan dukungan untuk font Taiwan yang sudah ketinggalan zaman.

Aspose.Words 24.11 memperkenalkan peringkasan dokumen bertenaga AI, opsi rendering yang ditingkatkan, peningkatan akses ke properti dokumen, dan teks kontrol ActiveX.

Aspose.Words 24.12 memperkenalkan penempatan label data yang dapat disesuaikan, terjemahan teks bertenaga Google AI, dan kelas pemrosesan LowCode baru yang disempurnakan.

### AI-Fitur bertenaga

#### Ringkasan Dokumen Menggunakan OpenAI dan Google <sup>24.11</sup>

Dukungan untuk peringkasan dokumen menggunakan model bahasa generatif **OpenAI** dan **Google** telah diintegrasikan dengan menambahkan namespace [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) dengan anggota publiknya.

#### Terjemahan teks menggunakan model bahasa generatif Google <sup>24.12</sup>

Kemampuan untuk menerjemahkan teks menggunakan model bahasa generatif Google telah diterapkan di Aspose.Words dengan menambahkan metode [translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/) dan pencacahan [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) ke namespace [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Kelas LowCode baru seperti [Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) dll. telah diperkenalkan, menawarkan serangkaian metode yang memberikan keseimbangan sempurna antara kesederhanaan dan fleksibilitas untuk pemrosesan dokumen.

### Rendering dan Pencetakan

#### Kelulusan pada Grafik Radial <sup>24.9</sup>

Rendering gradasi pada grafik radial telah diterapkan.

#### CommandButton ActiveX Kontrol <sup>24.10</sup>

Kemampuan untuk membuat kontrol CommandButton ActiveX telah diperkenalkan dengan menambahkan metode publik baru [insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/) dan kelas publik baru [Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/).

#### Kontrol Visibilitas Bentuk <sup>24.10</sup>

Properti publik baru [hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/) telah ditambahkan untuk mengontrol visibilitas bentuk.

#### Perubahan pada Bagan Pie dan Doughnut <sup>24.10</sup>

Beberapa properti publik baru telah ditambahkan ke bagan format Pie dan Doughnut.

#### Kontrol Rendering Batas Bidang Formulir Pilihan PDF <sup>24.11</sup>

Opsi baru untuk mengontrol rendering batas bidang formulir pilihan PDF telah diterapkan dengan menambahkan opsi publik baru [render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/).

#### Dapatkan dan Atur Kode Format untuk Data Bagan <sup>24.11</sup>

Kemampuan untuk mendapatkan dan mengatur kode format untuk data bagan telah ditambahkan dengan menerapkan properti [format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/) di kelas [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), dan [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/).

#### Render Bagan Histogram dengan Tempat Sampah dan Label <sup>24.11</sup>

Rendering grafik histogram telah ditingkatkan dengan memungkinkan sejumlah tempat sampah dan label tertentu.

#### Sesuaikan Penempatan Label Data <sup>24.12</sup>

Kemampuan untuk menyesuaikan penempatan label data telah ditambahkan dengan memperkenalkan properti baru ke kelas th [ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/) dan [ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Mengonversi, Memuat, dan Menyimpan Dokumen

#### Garis Bawahi Pemformatan saat Memuat File Markdown <sup>24.9</sup>

Opsi untuk mengenali pemformatan garis bawah saat memuat dokumen Markdown telah digabungkan dengan menambahkan properti publik baru [import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/).

#### Mengekspor tabel sebagai HTML saat menyimpan ke Markdown <sup>24.10</sup>

Opsi untuk mengekspor tabel sebagai HTML saat menyimpan dokumen ke format Markdown telah diterapkan dengan menambahkan properti publik baru [export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/) dan enumerasi [MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/).

#### Ekspor PDF dengan Struktur Logika yang Diperbarui <sup>24.11</sup>

Ekspor PDF telah ditingkatkan dengan menyertakan properti judul tabel sebagai judul elemen struktur logis PDF.

### Tanda Tangan Digital

#### Tanda tangani Dokumen dengan XAdES-EPES <sup>24.9</sup>

Kemampuan untuk menandatangani dokumen dengan tanda tangan XAdES-EPES level XML-DSig telah diperkenalkan dengan menambahkan properti publik baru [xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/) dan pencacahan publik baru [XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/).

### Lainnya

* Metode publik baru [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/) telah ditambahkan ke group shapes. <sup>24.9</sup>
* Metode publik baru [insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/) telah ditambahkan untuk menyisipkan **StructuredDocumentTags** ke dalam dokumen. <sup>24.9</sup>
* Akses publik ke pemisah catatan kaki / catatan akhir telah disediakan dengan menambahkan beberapa kelas dan properti publik. <sup>24.9</sup>
* Kemampuan untuk mengelompokkan masing-masing bentuk, group shapes bersama-sama, dan langsung mengelompokkan kedua bentuk dan group shapes telah diperkenalkan dengan menambahkan metode [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist). <sup>24.10</sup>
* Penanganan penyandian Big5 untuk tabel cmap TrueType telah ditingkatkan. <sup>24.10</sup>
* Dukungan untuk font Taiwan yang sudah ketinggalan zaman telah ditingkatkan. <sup>24.10</sup>
* Untuk mengakses properti dokumen yang diperluas, properti hanya-baca telah ditambahkan ke kelas [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/). <sup>24.11</sup>
* Menyetel teks untuk kontrol ActiveX telah diaktifkan dengan menambahkan penyetel publik baru ke properti [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.9 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.10 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.11 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.12 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words untuk Python melalui .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 memperluas opsi untuk rakitan, meningkatkan kemampuan rendering, dan memperluas beberapa opsi lainnya.

Aspose.Words 24.6 meningkatkan opsi rendering, meningkatkan fungsionalitas penelusuran dan perbandingan, dan memperluas beberapa fitur lainnya.

Aspose.Words 24.7 mengubah cara Anda bekerja dengan ActiveX, memperluas kemampuan rendering, serta mengekspor ke format Markdown dan XLSX.

Aspose.Words 24.8 meningkatkan penyesuaian bagan dengan kontrol presisi atas label sumbu, memperluas manajemen font, meningkatkan penanganan struktur dokumen, dan menambahkan kemampuan baru untuk ekspor HTML / XAML, fungsionalitas PDF, konversi dokumen, dan tanda tangan digital.

### Format yang Didukung

Mulai dari versi 24.7, ekspor ke PDF/UA-2 didukung untuk memastikan aksesibilitas bagi pengguna penyandang disabilitas.

### Rendering dan Pencetakan

#### Perubahan Bagan, Bentuk, dan DrawingML <sup>24.5</sup>

* DrawingML rendering efek untuk grafik SVG, memperluas fungsionalitas sebelumnya yang terbatas pada gambar, telah diterapkan.
* Dukungan untuk membuat bagan kombo dan menyesuaikan properti seperti lebar celah, tumpang tindih, dan skala gelembung dalam grup deret telah diperkenalkan dengan menambahkan kelas [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/) dan [ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/) serta properti [series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/).
* Fungsionalitas untuk memanipulasi efek SoftEdge dari bentuk telah diimplementasikan dengan menambahkan kelas [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/).
* Kemampuan untuk memodifikasi nilai adjust dari bentuk telah diterapkan dengan menambahkan kelas publik **AdjustmentCollection** dan **Adjustment** dan properti [adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/).

#### Perubahan Bagan, Bentuk, dan Gambar <sup>24.6</sup>

- Kemampuan pembuatan bagan telah ditingkatkan. Anda sekarang dapat membuat variasi bagan yang lebih luas, termasuk *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* bagan, bagan *Box & Whisker*, *Waterfalls*, dan *Funnels*. Ini memungkinkan Anda untuk memvisualisasikan data Anda dengan cara yang lebih beragam dan informatif.
- Kontrol warna untuk pemformatan bayangan telah ditingkatkan. Anda dapat memperoleh kontrol yang lebih tepat atas tampilan dokumen Anda dengan mengakses warna bayangan.
- Peningkatan kinerja untuk rendering latar belakang telah ditingkatkan. Anda dapat mempercepat rendering latar belakang yang berisi elemen kecil secara signifikan berkat teknologi ubin asli.
- Gradien realistis untuk bentuk telah ditambahkan. Anda sekarang dapat membuat bentuk DML dengan gradien non-linier, meniru gaya visual Microsoft Word untuk tampilan yang lebih halus.

#### Kustomisasi Label Data Bagan <sup>24.7</sup>

Kemampuan untuk menyesuaikan label data bagan seperti **Orientation** dan **Rotation** telah ditambahkan.

#### Gaya Nomor Khusus untuk Level Daftar <sup>24.7</sup>

Penyetel untuk properti publik [custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/) telah ditambahkan. Anda sekarang dapat menentukan gaya angka khusus untuk level daftar.

#### Perubahan dalam bekerja dengan ActiveX <sup>24.7</sup>

- Properti objek ActiveX sekarang dapat dimodifikasi, memberi Anda kontrol lebih besar atas perilakunya.
- Kemampuan untuk mengubah nilai kontrol tombol radio ActiveX untuk mengaktifkan interaksi dinamis telah ditambahkan.
- Kemampuan untuk mengubah ActiveX checkbox menjadi "dicentang " atau" tidak dicentang " telah ditambahkan.

#### Kontrol Atas Sumbu Bagan Centang Label Orientasi dan Rotasi <sup>24.8</sup>

Kontrol yang tepat atas orientasi dan rotasi label centang sumbu bagan telah ditambahkan untuk penyesuaian bagan yang lebih nyaman-kelas [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) telah diperluas dengan properti [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) dan [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/) yang baru.

#### Mengganti Garis Miring Terbalik dengan Tanda Yen <sup>24.8</sup>

Ekspor HTML dan XAML yang kompatibel ke belakang untuk mengganti karakter garis miring terbalik dengan tanda Yen telah ditingkatkan. Untuk mencapai hal ini, properti **replace_backslash_with_yen_sign** telah ditambahkan ke kelas [HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/) dan [XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/).

#### Menggunakan Tag SDT sebagai Nama Bidang Formulir saat Mengekspor ke PDF <sup>24.8</sup>

Ekspor PDF dengan dukungan untuk menggunakan tag SDT sebagai nama bidang formulir telah ditingkatkan dengan menambahkan properti [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) baru ke kelas [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/).

### Mengonversi, Memuat, dan Menyimpan Dokumen

#### Mengekspor Tautan ke Format Markdown <sup>24.7</sup>

Kemampuan untuk mengontrol ekspor tautan dalam format Markdown telah ditambahkan melalui penerapan properti [link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/).

#### LowCode 24.8 <sup>24.8</sup>

Kelas [LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/) baru, yang dirancang untuk menyediakan serangkaian metode untuk mengonversi berbagai jenis dokumen dengan satu baris kode, telah diperkenalkan.

### Cari dan Bandingkan

#### Opsi Perbandingan Lanjutan <sup>24.6</sup>

Kemampuan untuk merampingkan alur kerja analisis data dengan fungsionalitas perbandingan yang ditingkatkan telah ditambahkan. Ini termasuk opsi [ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/) baru dan antarmuka yang didesain ulang untuk perbandingan lanjutan.

### Lainnya

* Fungsi untuk menghilangkan halaman kosong dari dokumen telah diimplementasikan dengan menambahkan metode [remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/). <sup>24.5</sup>
* Kemampuan untuk memeriksa keberadaan makro VBA tanpa memuat dokumen telah disediakan dengan menambahkan properti [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/). <sup>24.5</sup>
* Mempertahankan penomoran sumber saat menyisipkan dokumen menggunakan Mesin Pelaporan LINQ sekarang didukung. <sup>24.5</sup>
* Properti [date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/) baru telah ditambahkan – ini memberikan stempel waktu yang lebih tepat untuk komentar, meningkatkan organisasi, dan keterlacakan. <sup>24.6</sup>
* Format datetime sekarang secara otomatis terdeteksi untuk ekspor tanpa batas ke format XLSX. <sup>24.7</sup>
* Properti publik [is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/), yang memungkinkan Anda memverifikasi apakah proyek VBA dilindungi, telah ditambahkan. <sup>24.7</sup>
* Informasi font telah diperluas dengan properti **embedding_licensing_rights** ditambahkan ke kelas [FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/) dan [PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* Cara untuk menghapus header dan footer bagian secara efisien sambil mempertahankan tanda air telah ditambahkan untuk bekerja lebih akurat dengan struktur dokumen. Untuk menghapus header dan footer bagian, gunakan metode publik baru [clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default). <sup>24.8</sup>
* Penandatanganan digital dokumen XPS menggunakan [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/) telah diaktifkan-properti baru [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/) telah ditambahkan untuk tujuan ini. <sup>24.8</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.5 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.6 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.7 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.8 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words untuk Python melalui .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 meningkatkan pengalaman seputar pengelolaan warna guratan, menyempurnakan objek OLE, serta memperkenalkan publik `Bibliography Sources` baru API.

Aspose.Words 24.2 Bagan yang diperluas API dan manajemen gaya. Versi Aspose.Words ini juga memperkenalkan kemampuan untuk menentukan SvgSaveOptions selama rendering, kontrol yang lebih fleksibel saat memuat file Markdown, dan bekerja dengan teks referensi untuk catatan kaki dan catatan akhir.

Aspose.Words 24.3 memperkenalkan Pembaca/Penulis TIFF baru dan Meniru operasi raster biner untuk WMF metafile. Aspose.Words 24.3 juga terus memperluas Bagan API.

Aspose.Words 24.4 meningkatkan format penyimpanan, beberapa opsi rendering, serta meningkatkan pekerjaan dengan tanda tangan digital.

### Format yang Didukung <sup>24.4</sup>

Format gambar **WebP** modern sekarang didukung di Aspose.Words untuk .NET Framework 4.6.2 dan lebih tinggi. Anda sekarang dapat membaca dan menyisipkan gambar WebP ke dalam dokumen, serta menyimpan gambar dalam format WebP.

Harap perhatikan bahwa WebP saat ini hanya tersedia di .NET Standard dan .NET Framework v4.6.2 ke atas.

### Rendering dan Pencetakan

#### Kontrol Warna Goresan <sup>24.1</sup>

Kelas [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) telah diperluas dengan sekumpulan properti publik baru yang terkait dengan pengelolaan warna guratan: [fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/) dan [back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/), [fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/) dan [back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### DrawingML Bagan API Ekstensi <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** terus diperluas.

#### Sematkan Font yang Dideklarasikan dalam Aturan @font-face <sup>24.4</sup>

Menambahkan kemampuan untuk menyematkan font yang dideklarasikan dalam aturan @font-face ke dalam definisi font dokumen yang dihasilkan telah diperkenalkan dengan menambahkan properti [support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/) baru.

#### Bekerja dengan Pemformatan Cahaya dan Refleksi <sup>24.4</sup>

Kemampuan untuk bekerja dengan pemformatan cahaya dan refleksi untuk objek gambar telah diterapkan.

### Memuat dan Menyimpan Dokumen

#### Tentukan SvgSaveOptions Selama Rendering <sup>24.2</sup>

Kemampuan untuk menentukan [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) selama rendering telah ditambahkan menggunakan [ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) dan [OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) metode.

#### Pertahankan Baris Kosong saat Memuat file Markdown <sup>24.2</sup>

Kemampuan untuk mempertahankan baris kosong saat memuat file Markdown telah ditambahkan.

#### Pembaca/Penulis TIFF Baru <sup>24.3</sup>

Pembaca/penulis TIFF baru untuk Aspose.Words telah dikembangkan. Aspose.Words untuk .NET 24.3 menambahkan dukungan untuk membaca gambar TIFF dengan tipe kompresi JPEG dan JPEG Lama, dan juga meningkatkan kualitas operasi baca dan tulis secara signifikan.

### Lainnya

* Kemampuan untuk memodifikasi teks dari kontrol `TextBox` OLE telah diperkenalkan dengan menambahkan properti **Text** baru ke kelas **TextBoxControl** yang baru. <sup>24.1</sup>
* Bibliography Sources public API diimplementasikan melalui penambahan namespace baru [Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/) dengan kelas dan enumerasi barunya, dan melalui penambahan properti [bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/) baru ke kelas [Document](https://reference.aspose.com/words/python-net/aspose.words/document/). <sup>24.1</sup>
* Properti publik baru [priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/), [unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/), dan [semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/) untuk manajemen gaya yang disempurnakan telah ditambahkan ke kelas [Style](https://reference.aspose.com/words/python-net/aspose.words/style/). <sup>24.2</sup>
* Fungsionalitas untuk mengambil teks tanda referensi aktual untuk catatan kaki dan catatan akhir telah ditingkatkan dengan properti [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/) dan metode [update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default). <sup>24.2</sup>
* Emulasi operasi raster biner untuk WMF metafile telah diterapkan. <sup>24.3</sup>
* Kemampuan untuk menentukan opsi tanda tangan untuk dokumen dalam **SaveOptions** telah diaktifkan dengan menambahkan kelas [DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/) baru dengan anggota publik baru, serta menambahkan properti baru ke kelas [OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/), dan [OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.1 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.2 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.3 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 24.4 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words untuk Python melalui .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 memperluas opsi rendering, emulasi rendering metafile, dan opsi penyimpanan markdown.

Aspose.Words 23.10 meningkatkan rendering, memperluas opsi untuk memuat dan menyimpan dokumen, dan memungkinkan pengguna menggabungkan dokumen dengan cara baru.

Aspose.Words 23.11 menyempurnakan pekerjaan dengan revisi, format XLSX, dan font pada legenda bagan dengan opsi tambahan.

Aspose.Words 23.12 memperkenalkan properti dan pencacahan baru untuk bekerja dengan dokumen PDF dan OOXML, serta dukungan untuk gambar WebP.

### Rendering dan Pencetakan

#### Menyesuaikan Judul Sumbu dalam Bagan DrawingML <sup>23.9</sup>

Kemampuan untuk menyesuaikan judul sumbu dalam bagan DrawingML telah diperkenalkan dengan penerapan properti kelas publik baru [ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/) dan [title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/).

####  Menentukan Posisi Vertikal Font dalam sebuah Paragraf <sup>23.9</sup>

Sekarang dimungkinkan untuk menentukan posisi vertikal font dalam paragraf menggunakan properti public [baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/) baru dan enumerasi [BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/) baru.

#### Kontrol Warna Latar Depan <sup>23.10</sup>

Kemampuan untuk mengambil warna latar depan tanpa pengubah telah ditambahkan ke kelas [Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/) dan [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) melalui properti **BaseForeColor**.

#### Memperluas Fungsionalitas Bagan <sup>23.10</sup>

Fungsionalitas kelas [ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/), dan [ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/) telah diperluas dengan metode dan properti baru.

#### Secara Otomatis Menyesuaikan dan Menyesuaikan Gambar menjadi Bentuk <sup>23.10</sup>

Cara sederhana untuk menyesuaikan dan menyesuaikan gambar secara otomatis dalam bentuk tertentu telah disediakan melalui metode [fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default) yang baru.

#### Pemformatan Font Default untuk Entri Legenda Bagan DrawingML <sup>23.11</sup>

Kemampuan untuk menentukan pemformatan font default untuk entri legenda bagan DrawingML telah ditambahkan melalui properti [font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/). Fitur ini memfasilitasi tampilan yang lebih ramping dan konsisten untuk elemen bagan, meningkatkan estetika dokumen secara keseluruhan.

#### Tentukan Tata Letak Halaman saat Membuka PDF di Pembaca <sup>23.12</sup>

Kemampuan untuk menentukan tata letak halaman yang akan digunakan saat membuka dokumen di pembaca PDF telah ditambahkan melalui pengenalan properti [page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/) baru ke kelas [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) dan pengenalan pencacahan [PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/) baru.

### Memuat dan Menyimpan Dokumen

#### Menentukan Nama Folder untuk Membuat Image URIs dalam Markdown <sup>23.9</sup>

Kelas [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) telah diperluas dengan menyertakan properti [images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/), yang memungkinkan untuk menentukan nama folder yang digunakan untuk membuat gambar URIs yang ditulis ke dalam dokumen Markdown.

#### Kurangi Ukuran Keluaran PDF <sup>23.10</sup>

Berbagai pengoptimalan rendering PDF untuk mengurangi ukuran keluaran saat menggunakan pengaturan [optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/) telah diterapkan.

#### Mengenali Hyperlink saat Memuat Dokumen TXT <sup>23.10</sup>

Fitur untuk mengenali hyperlink saat memuat dokumen TXT telah diterapkan dengan menambahkan properti [detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/) baru.

### Lainnya

- Emulasi rendering metafile untuk menentukan ukuran rasterisasi telah diterapkan, khususnya untuk lebar pena WMF dan lebar pena kosmetik EMF. Untuk mencapai hal ini, properti **ScaleWmfFontsToMetafileSize** diganti dengan properti [emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/) dan properti [emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/) ditambahkan. <sup>23.9</sup>
- Metode yang disederhanakan untuk menyisipkan satu dokumen ke dokumen lain pada posisi kursor saat ini telah diperkenalkan menggunakan metode [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions). <sup>23.10</sup>
- Kemampuan untuk mengakses dan memodifikasi properti gaya telah ditambahkan melalui pengenalan properti [locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/) yang baru. <sup>23.10</sup>
- Parameter tipe generik telah ditambahkan ke metode kelas [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/). <sup>23.10</sup>
- Kemampuan untuk menulis semua bagian dokumen ke lembar kerja XLSX yang sama telah disediakan melalui tipe enumerasi [XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/) yang baru dan properti [section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/) yang baru. <sup>23.11</sup>
* Cara untuk mengontrol bagaimana ekstensi format ZIP64 akan digunakan untuk dokumen OOXML telah diterapkan melalui properti Zip64Mode baru dari kelas `OoxmlSaveOptions` dan pencacahan Zip64Mode baru. <sup>23.12</sup>
* Dukungan untuk gambar WebP telah diperkenalkan. Harap dicatat bahwa fitur ini hanya tersedia untuk .versi NetStandart dan .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 23.9 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 23.10 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 23.11 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk .NET 23.12 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words untuk Python melalui .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 meningkatkan kemampuan untuk bekerja dengan data deret bagan dan kemampuan untuk bekerja dengan dokumen ODT, serta meningkatkan header/footer dan pembungkusan teksnya.

Aspose.Words 23.6 memperluas opsi rendering, menambahkan format ekspor baru, meningkatkan pelaporan LINQ, dan alat LowCode.

Aspose.Words 23.7 meningkatkan kemampuan pelaporan, menambahkan format ekspor baru, dan memperkenalkan perubahan untuk bekerja dengan tabel dan tanda tangan digital.

Aspose.Words 23.8 memperluas kemampuan format yang berbeda, meningkatkan rendering, dan menambahkan opsi baru untuk bekerja dengan bidang.

### Format yang Didukung

* Dimulai dengan versi 23.6, dimungkinkan untuk menyimpan dokumen dalam format XLSX. Sekarang Anda dapat mengonversi dokumen Anda ke format Excel. <sup>23.6</sup>

* Dimulai dengan versi 23.7, dimungkinkan untuk menyimpan halaman atau bentuk dokumen dalam format EPS. <sup>23.7</sup>

### Fitur Format Baru

- Fungsionalitas untuk membuat Daftar Isi (TOC) secara otomatis untuk dokumen MOBI telah diperkenalkan. <sup>23.8</sup>
- Konstruktor [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) telah diperluas dengan [PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions). <sup>23.8</sup>
- Pembentukan teks vertikal untuk EMF metafile telah diterapkan. <sup>23.8</sup>

### Rendering

#### Dapatkan dan Modifikasi Data Deret Bagan <sup>23.5</sup>

Fitur untuk mendapatkan dan memodifikasi data deret bagan disediakan dengan menambahkan:

- kelas baru: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- tipe enum baru: [ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### Dukungan untuk Tipografi Tingkat Lanjut <sup>23.6</sup>

Dukungan untuk Tipografi Tingkat Lanjut dalam rendering WMF, EMF dan EMF+ telah ditambahkan.

#### Konten Berwarna pada Halaman <sup>23.6</sup>

Properti publik [PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/), yang menunjukkan apakah halaman diwarnai atau tidak, telah ditambahkan.

#### Pemformatan untuk Label Data Bagan <sup>23.6</sup>

Kemampuan untuk mengatur pemformatan isian, guratan, dan info untuk label data bagan telah diterapkan.

### Mail Merge dan Pelaporan

#### Penyisipan HTML Dinamis untuk Mesin Pelaporan LINQ <sup>23.6</sup>

Cara baru penyisipan HTML dinamis untuk Mesin Pelaporan LINQ telah ditambahkan.

#### Dukungan Tag Mustache <sup>23.7</sup>

Tag Mustache sekarang didukung dalam metode [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/) dan [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/).

#### Menentukan Ukuran Gambar yang Dirender <sup>23.8</sup>

Properti publik baru [image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/) untuk menentukan ukuran gambar yang dirender dalam piksel telah diperkenalkan.

#### Pertahankan Spasi Kosong untuk Nilai String JSON - LINQ <sup>23.8</sup>

Opsi telah ditambahkan ke Mesin Pelaporan LINQ untuk mempertahankan spasi kosong untuk nilai string JSON.

### LowCode <sup>23.6</sup>

Metode LowCode baru yang dimaksudkan untuk menggabungkan berbagai jenis dokumen menjadi satu dokumen keluaran telah ditambahkan.

### Lainnya

- Dukungan untuk pembungkusan teks di header / footer telah diterapkan. <sup>23.5</sup>
- Kemampuan untuk menghapus tanda tangan digital dari dokumen ODT telah ditambahkan melalui metode [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str). <sup>23.5</sup>
- Properti publik [phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/) untuk mendapatkan teks dasar dan rubi dari panduan fonetik [Run](https://reference.aspose.com/words/python-net/aspose.words/run/) telah ditambahkan. <sup>23.5</sup>
- Kemampuan untuk mengambil nilai tanda tangan digital dari dokumen yang ditandatangani secara digital sebagai larik byte telah ditambahkan dengan memperkenalkan properti [signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/) baru. <sup>23.7</sup>
- Kelas [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/) dan [Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/) telah diperpanjang dengan anggota publik baru– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), dan [Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/). <sup>23.7</sup>

{{% alert color="primary" %}}

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 23.5 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-5-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 23.6 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-6-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 23.7 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

Pelajari lebih lanjut tentang [Aspose.Words untuk Python via .NET 23.8 Catatan Rilis](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## Lihat Juga

{{% alert color="primary" %}}

Halaman ini berisi berita rilis terbaru selama 2 tahun terakhir. Untuk detail tentang rilis sebelumnya, lihat [Catatan Rilis'](https://releases.aspose.com/words/python/release-notes/) halaman di bagian yang relevan.

{{% /alert %}}
