---
title: 新着情報
second_title: Aspose.WordsのためのPython via .NET
articleTitle: What's new in Aspose.WordsのためのPython via .NET
linktitle: What's new in Aspose.WordsのためのPython via .NET
type: docs
description: "Aspose.WordsのためのPython via .NET 毎日拡大し、強化します。 このページでは、製品の巨大で最も興味深い機能について学ぶことができます。"
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ja/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-06-23-21-02-49
---

このページでは、最近のリリースで導入された最も興味深い新しいAspose.Words機能について説明します。

## Aspose.WordsはPython via .NET25.5,25.6の場合

Aspose.Words25.5新しいスタイルオプションでグラフのカスタマイズが強化され、空の段落の処理方法を制御できるようになりましたMarkdownエクスポー

Aspose.Words25.6高度な画像エクスポートオプション、改善されたMathML処理、およびより良いチャート表現を導入することにより、レンダリングの精度とビジュアライゼーションフィーチャーを強化します。

### ドキュメントの変換、読み込み、保存

#### 空の段落をMarkdownにエクスポートする <sup>25.5</sup>

空の段落をMarkdownにエクスポートする方法を制御する機能は、**MarkdownEmptyParagraphExportMode**列挙体と**empty_paragraph_export_mode**プロパティを追加することによって導入されました。

#### 複数ページのドキュメントをラスターイメージ形式にエクスポートする <sup>25.6</sup>

複数ページのドキュメントをPNGやJPEGなどのラスターイメージ形式に[customizable layouts](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/)-水平、垂直、またはグリッドでエクスポートする機能は、画像エクスポート機能を拡張して導入されました。

### レンダリング

#### グラフスタイルの設定 <sup>25.5</sup>

チャートスタイルを設定する機能は、**ChartStyle**列挙体と**style**プロパティを追加することによって導入されました。

#### MathML式でのコネクタ行のレンダリング <sup>25.6</sup>

MathML式でのコネクタ線のレンダリングは、数式のより正確で視覚的に一貫した表示を確実にするために実装されています。

#### ウォーターフォールチャートの凡例のレンダリング <sup>25.6</sup>

["Waterfall" charts](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriestype/)の凡例のレンダリングが導入され、データの透明性が向上し、これらのチャートの解釈性が向上しました。

### その他

* 複数のスラッシュを含む数式をラップする機能が強化され、レイアウトの明快さと数式の読みやすさが向上しました。 <sup>25.6</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.WordsforPython via .NET25.5リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-5-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsforPython via .NET25.6リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-6-release-notes/).

{{% /alert %}}

## .NET 経由の Python の Aspose.Words 25.1、25.2、25.3、25.4

Aspose.Words25.1はAIを使用した文法チェックを導入し、HTML、SVG、Markdown形式の高度なオプションを使用して文書の保存を強化します。

Aspose.Words25.2はAnthropicAIモデルによるテキスト要約を導入し、MsWorks形式のサポートを追加し、タイポグラフィ制御を強化し、PDF構造とリストの処理を改善します。

Aspose.Words25.3AIを使用した文法チェッカーとフォントの選択をUpdateAmbiguousTextFontプロパティで強化し、PDF添付ファイルのエクスポートを改善しました。

Aspose.Words25.4は新しい用紙サイズのサポートを導入し、高度なHTMLエクスポート制御を有効にし、透かしの処理を改善します。

### AI搭載の機能

#### 文書AI文法チェック

* OpenAI生成モデルを使用して提供された文書の文法をチェックする機能は、新しい[check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/)メソッドを追加することによって導入されました。 <sup>25.1</sup>
* AIを使用した文法チェック機能が更新され、[AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/)列挙体で使用可能なすべてのモデルがサポートされました。 <sup>25.3</sup>

#### Anthropic生成言語モデルを使用した要約 <sup>25.2</sup>

新しいパブリッククラス[AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/)を導入することにより、Anthropic生成言語モデルを使用したテキスト要約が可能になりました。

### サポートされている形式 <sup>25.2</sup>

バージョン25.2から、MicrosoftWorksドキュメントの新しいMsWorksロード形式との互換性が追加されました。

### ドキュメントの変換、読み込み、保存

#### HTML形式とSVG形式への保存を改善しました <sup>25.1</sup>

[HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/)クラスと[SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/)クラスの両方に**id_prefix**プロパティと**remove_java_script_from_links**プロパティを追加することで、HTML形式とSVG形式への保存が強化されました。

#### 保存時の画像解像度とOfficeMath出力モードをMarkdownに設定します <sup>25.1</sup>

* 画像の解像度を設定するための新しい[image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/)オプションが[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)クラスに追加されました。
* 新しい[office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/)オプションと[MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/)列挙体が[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)クラスに追加され、OfficeMath出力モードを設定しました。

### レンダリング

#### 改善されたタイポグラフィ制御 <sup>25.2</sup>

[number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/)プロパティは、タイポグラフィ制御を改善するために追加されました。

#### あいまいな文字のフォント選択の制御 <sup>25.3</sup>

新しいパブリックプロパティ[update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/)が[SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/)クラスに追加され、使用される文字コードに従ってフォントの選択を制御します。

#### 用紙サイズオプション <sup>25.4</sup>

JISB4とJISB5用紙サイズを使用する機能は、[PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/)列挙体に新しい値を追加することによって導入されました。

#### HTML出力制御 <sup>25.4</sup>

HTMLエクスポート中にJavaScriptをハイパーリンクURLsから削除する機能は、[RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/)プロパティを追加することによって導入されました。

### その他

* PDF論理構造が改善され、TOA、BIBLIOGRAPHY、INDEXフィールドがサポートされました。 <sup>25.2</sup>
* リストの処理を改善するために[add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate)メソッドが導入されました。 <sup>25.2</sup>
* PDF添付ファイルのエクスポートを改善するために**EmbedAttachments**を置き換える新しいプロパティ[attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/)が追加されました。 また、PDF/Aバージョンの添付ファイルをサポートするために、[PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/)列挙体に新しい値が追加されました。 さらに、添付ファイルは暗号化でサポートされるようになりました。 <sup>25.3</sup>
* ストリームから画像の透かしを設定する機能は、[SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions)メソッドに新しいオーバーロードを追加することによって導入されました。 <sup>25.4</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 25.1リリースノート](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 25.2リリースノート](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 25.3リリースノート](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 25.4リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## .NET 経由の Python の Aspose.Words 24.9、24.10、24.11、24.12

Aspose.Words24.9はDocumentBuilderを介してgroup shape挿入とStructuredDocumentTag挿入を導入し、目盛りによる放射状チャートレンダリングを強化し、XAdES-EPESサポートによるデジタル署名を改善し、Markdown下線認識を追加し、脚注/文末脚注セパレータへのアクセスを提供します。

Aspose.Words24.10はCommandButton作成による強化されたActiveXコントロールサポート、新しい形状の可視性コントロール、group shapesへの機能、テーブルの改善されたMarkdownエクスポート、PieとDoughnutチャートのチャー

Aspose.Words24.11はAIを活用した文書の要約、強化されたレンダリングオプション、文書のプロパティへのアクセスの改善、ActiveXコントロールキャプションを導入します。Aspose.Words24.11はAI

Aspose.Words24.12では、カスタマイズ可能なデータラベルの配置、GoogleAIによるテキスト翻訳、および強化された新しいLowCode処理クラスが導入されました。

### AI搭載の機能

#### OpenAIとGoogleを使用した文書の要約 <sup>24.11</sup>

**OpenAI**および**Google**生成言語モデルを使用した文書要約のサポートは、[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)名前空間とそのパブリックメンバーを追加することによって統合されています。

#### Googleの生成言語モデルを使用したテキスト翻訳 <sup>24.12</sup>

Googleの生成言語モデルを使用してテキストを翻訳する機能は、Aspose.Wordsに[translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/)メソッドと[Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/)列挙体を[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)名前空間に追加することによって実装されています。

### Low Code <sup>24.12</sup>

新しいLowCodeクラスのような[Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) など。 文書処理のための簡易性と柔軟性間の完全なバランスを打つ一組の方法を提供する導入された。

### レンダリングと印刷

#### ラジアルチャート上の目盛り <sup>24.9</sup>

放射状チャート上の目盛りのレンダリングが実装されています。

#### CommandButtonActiveXコントロール <sup>24.10</sup>

CommandButtonActiveXコントロールを作成する機能は、新しいパブリックメソッド[insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/)と新しいパブリッククラス[Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/)を追加することによって導入されました。

#### 形状の可視性を制御する <sup>24.10</sup>

図形の可視性を制御するために、新しいパブリックプロパティ[hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/)が追加されました。

#### PieチャートとDoughnutチャートの変更点 <sup>24.10</sup>

書式PieおよびDoughnutチャートにいくつかの新しいパブリックプロパティが追加されました。

#### PDF選択フォームフィールドの境界線のレンダリングを制御します <sup>24.11</sup>

新しいパブリックオプション[render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/)を追加することにより、PDF選択フォームフィールド境界のレンダリングを制御する新しいオプションが実装されました。

#### グラフデータの書式コードの取得と設定 <sup>24.11</sup>

チャートデータの書式コードを取得および設定する機能は、[ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/)、[ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/)、および[BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/)クラスに[format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/)プロパティを実装することによって追加されました。

#### ビンとラベルを使用したヒストグラムチャートのレンダリング <sup>24.11</sup>

ヒストグラムチャートレンダリングは、指定された数のビンとラベルを使用できるようにすることで改善されました。

#### データラベルの配置をカスタマイズする <sup>24.12</sup>

[ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/)クラスと[ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/)クラスに新しいプロパティを導入することで、データラベルの配置をカスタマイズする機能が追加されました。

### 文書の変換、読み込み、保存

#### Markdownファイルを読み込むときの書式設定に下線を引きます <sup>24.9</sup>

新しいパブリックプロパティ[import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/)を追加することにより、Markdown文書を読み込むときに下線の書式を認識するオプションが組み込まれました。

#### Markdownに保存するときにテーブルをHTMLとしてエクスポートする <sup>24.10</sup>

文書をMarkdown形式で保存するときにテーブルをHTMLとしてエクスポートするオプションは、新しいパブリックプロパティ[export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/)と列挙[MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/)を追加することによ

#### 更新された論理構造を使用してPDFをエクスポートする <sup>24.11</sup>

PDFエクスポートは、テーブルタイトルプロパティをPDF論理構造要素のタイトルとして含めることで拡張されました。

### デジタル署名

#### XAdES-EPESで文書に署名する <sup>24.9</sup>

新しいパブリックプロパティ[xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/)と新しいパブリック列挙[XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/)を追加することにより、XAdES-EPESレベルXML-DSig署名で文書に署名する機能が導入されました。

### その他

* 新しいパブリックメソッド[insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/)がgroup shapesに追加されました。 <sup>24.9</sup>
* ドキュメントに**StructuredDocumentTags**を挿入するための新しいパブリックメソッド[insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/)が追加されました。 <sup>24.9</sup>
* 脚注/文末脚注の区切り文字へのパブリックアクセスは、いくつかのパブリッククラスとプロパティを追加することによって提供されています。 <sup>24.9</sup>
* [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist)メソッドを追加することにより、個々の図形group shapesをグループ化し、図形とgroup shapesの両方を直接グループ化する機能が導入されました。 <sup>24.10</sup>
* TrueTypecmapテーブルのbig5エンコード処理が改善されました。 <sup>24.10</sup>
* 古い台湾語フォントのサポートが強化されました。 <sup>24.10</sup>
* 拡張ドキュメントプロパティにアクセスするために、読み取り専用プロパティが[BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/)クラスに追加されました。 <sup>24.11</sup>
* ActiveXコントロールのキャプションの設定は、[Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/)プロパティに新しいpublicセッターを追加することで有効になりました。 <sup>24.11</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.9リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.10リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.11リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.12リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## .NET 経由の Python の Aspose.Words 24.5、24.6、24.7、24.8

Aspose.Words24.5アセンブリのオプションを展開し、レンダリング機能を向上させ、その他のオプションを展開します。

Aspose.Words24.6レンダリングオプションが改善され、検索と比較機能が強化され、他のいくつかの機能が拡張されました。

Aspose.Words24.7はActiveXの操作方法を変更し、レンダリング機能を拡張し、Markdown形式とXLSX形式にエクスポートします。

Aspose.Words24.8軸ラベルを正確に制御してグラフのカスタマイズを強化し、フォント管理を拡張し、文書構造の処理を改善し、HTML/XAMLエクスポート、PDF機能、文書変換、デジタ

### サポートされている形式

バージョン24.7からは、障害を持つユーザーのアクセシビリティを確保するためにPDF/UA-2へのエクスポートがサポートされています。

### レンダリングと印刷

#### チャート、図形、およびDrawingMLの変更 <sup>24.5</sup>

* DrawingMLエフェクトSVGグラフィックスのレンダリングが実装されており、これまでの機能は画像に限定されていました。
* コンボチャートを作成し、系列グループ内のギャップ幅、オーバーラップ、バブルスケールなどのプロパティを調整するためのサポートは、[ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/)クラスと[ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/)クラスと[series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/)
* 図形のSoftEdge効果を操作する機能は、[SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/)クラスを追加することによって実装されています。
* 図形の調整値を変更する機能は、**AdjustmentCollection**と**Adjustment**パブリッククラスと[adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/)プロパティを追加することによって実装されています。

#### チャート、図形、図面の変更 <sup>24.6</sup>

- グラフ作成機能が強化されました。 これで、次のようなさまざまなグラフを作成できます*Treemaps*, *Sunbursts*, *Histograms*, *Pareto* チャート、*Box & Whisker*チャート、*Waterfalls*、および*Funnels*。 これにより、より多様で有益な方法でデータを視覚化することができます。
- 影の書式設定のカラーコントロールが改善されました。 影の色にアクセスすることで、ドキュメントの外観をより正確に制御できます。
- バックグラウンドレンダリングのパフォーマンス向上が改善されました。 ネイティブのタイル技術のおかげで、小さな要素を含む背景のレンダリングを大幅に高速化できます。
- 形状のための現実的なグラデーションが追加されました。 非線形グラデーションを持つDML図形を作成し、Microsoft Wordの視覚スタイルを模倣して、より洗練された外観にすることができます。

#### チャートデータラベルのカスタマイズ <sup>24.7</sup>

**Orientation**や**Rotation**などのチャートデータラベルをカスタマイズする機能が追加されました。

#### リストレベルのカスタム番号スタイル <sup>24.7</sup>

パブリックプロパティ[custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/)のセッターが追加されました。 リストレベルのカスタム番号スタイルを定義できるようになりました。

#### ActiveXでの作業の変更点 <sup>24.7</sup>

- ActiveXオブジェクトのプロパティを変更できるようになり、その動作をより詳細に制御できるようになりました。
- ラジオボタンActiveXコントロールの値を変更して動的相互作用を有効にする機能が追加されました。
- ActiveXcheckboxを"checked"または"unchecked"に切り替える機能が追加されました。

#### チャート軸の目盛りラベルの向きと回転の制御 <sup>24.8</sup>

グラフのカスタマイズをより便利にするために、グラフ軸の目盛りラベルの向きと回転を正確に制御できるようになりました。[AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/)クラスは新しい[orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/)と[rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/)プロパティで拡張されました。

#### 円記号を円記号に置き換える <sup>24.8</sup>

バックスラッシュ文字を円記号に置き換えるための後方互換性のあるHTMLとXAMLエクスポートが改善されました。 これを実現するために、**replace_backslash_with_yen_sign**プロパティが[HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/)クラスと[XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/)クラスに追加されました。

#### PDFにエクスポートするときにSDTタグをフォームフィールド名として使用する <sup>24.8</sup>

[PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/)クラスに新しい[use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/)プロパティを追加することで、SDTタグをフォームフィールド名として使用することをサポートしたPDFエクスポートが強化されました。[PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/)クラスに新しい[use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/)プロパティを追加しました。

### 文書の変換、読み込み、保存

#### Markdown形式へのリンクのエクスポート <sup>24.7</sup>

[link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/)プロパティの実装により、Markdown形式のリンクのエクスポートを制御する機能が追加されました。

#### LowCode 24.8 <sup>24.8</sup>

さまざまなドキュメントタイプを1行のコードで変換するための一連のメソッドを提供するように設計された新しい[LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/)クラスが導入されました。

### 検索と比較

#### 高度な比較オプション <sup>24.6</sup>

改善された比較機能を備えたデータ分析ワークフローを合理化する機能が追加されました。 これには、新しい[ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/)オプションと、高度な比較のための再設計されたインターフェイスが含まれます。

### その他

* ドキュメントから空のページを削除する関数は、[remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/)メソッドを追加することによって実装されています。 <sup>24.5</sup>
* ドキュメントをロードせずにVBAマクロの存在をチェックする機能は、[has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/)プロパティを追加することによって提供されています。 <sup>24.5</sup>
* LINQレポートエンジンを使用して文書を挿入する際にソース番号を保持することがサポートされるようになりました。 <sup>24.5</sup>
* 新しい[date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/)プロパティが追加されました–これにより、コメントのより正確なタイムスタンプが提供され、組織とトレーサビ <sup>24.6</sup>
* XLSX形式へのシームレスなエクスポートのために、datetime形式が自動的に検出されるようになりました。 <sup>24.7</sup>
* VBAプロジェクトが保護されているかどうかを確認できるパブリックプロパティ[is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/)が追加されました。 <sup>24.7</sup>
* フォント情報は、[FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/)クラスと[PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/)クラスに**embedding_licensing_rights**プロパティが追加されて拡張されました。 <sup>24.8</sup>
* 透かしを保持しながら、効率的にセクションのヘッダーとフッターをクリアする方法は、より正確に文書構造を操作するために追加されました。 セクションヘッダーとフッターをクリアするには、新しいpublicメソッド[clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default)を使用します。 <sup>24.8</sup>
* [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/)を使用したXPS文書のデジタル署名が有効になりました–この目的のために新しいプロパティ[digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/)が追加されました。 <sup>24.8</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.5リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.6リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.7リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.8リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## .NET 経由の Python の Aspose.Words 24.1、24.2、24.3、24.4

Aspose.Words24.1ストロークカラーの管理に関する経験が向上し、OLEオブジェクトが強化され、新しい`Bibliography Sources`パブリックAPIが導入されました。

Aspose.Words24.2拡張チャートAPIとスタイル管理。 このバージョンのAspose.Wordsでは、レンダリング中にSvgSaveOptionsを指定する機能、Markdownファイルを読み込む柔軟な制御、脚注と文末脚注の参照テキストを操作する機能も導入されました。

Aspose.Words24.3は新しいTIFFリーダー/ライターを導入し、WMFメタファイルのバイナリラスタ演算のエミュレーションを導入しました。 Aspose.Words24.3もチャートAPIを拡大し続けます。

Aspose.Words24.4保存形式、いくつかのレンダリングオプションを強化し、デジタル署名の作業を改善します。

### サポートされている形式 <sup>24.4</sup>

最新の**WebP**画像形式がサポートされるようになりました Aspose.Wordsのための.NET Framework 4.6.2 そしてより高い。 WebP画像を読み込んで文書に挿入したり、WebP形式で画像を保存したりできるようになりました。

WebPは現在.NET Standardと.NET Frameworkv4.6.2以上でのみ利用可能です。

### レンダリングと印刷

#### ストロークカラーコントロール <sup>24.1</sup>

[Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/)クラスは、ストロークの色の管理に関連する一連の新しいパブリックプロパティ[fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/)と[back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/)、[fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/)と[back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/)で拡張されました。

#### DrawingMLチャートAPI拡張 <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API**は引き続き展開されます。

#### @font-faceルールで宣言された埋め込みフォント <sup>24.4</sup>

新しい[support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/)プロパティを追加することで、@font-faceルールで宣言されたフォントを結果のドキュメントのフォント定義に埋め込む機能が導入されました。

#### グローとリフレクションの書式設定を使用する <sup>24.4</sup>

描画オブジェクトのグローとリフレクションの書式設定を操作する機能が実装されました。

### 文書の読み込みと保存

#### レンダリング中にSvgSaveOptionsを指定します <sup>24.2</sup>

レンダリング中に[SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/)を指定する機能が[ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/)を使用して追加されました。[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions)と[OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/)。[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions)メソッド。

#### Markdownファイルの読み込み時に空の行を保持する <sup>24.2</sup>

Markdownファイルの読み込み時に空行を保持する機能が追加されました。

#### 新しいTIFFリーダー/ライター <sup>24.3</sup>

Aspose.Words用の新しいTIFFリーダ/ライタが開発されました。 Aspose.Wordsのための.NET 24.3 JPEGおよび古いJPEG圧縮タイプのTIFF画像の読み取りのサポートが追加され、読み取りおよび書き込み操作の品質も大幅に改善されました。

### その他

* `TextBox`OLEコントロールのテキストを変更する機能は、新しい**Text**プロパティを新しい**TextBoxControl**クラスに追加することによって導入されました。 <sup>24.1</sup>
* 参考文献ソースpublicAPIは、新しいクラスと列挙を含む新しい名前空間[Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/)の追加と、新しい[bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/)プロパティを[Document](https://reference.aspose.com/words/python-net/aspose.words/document/)クラスに追加することによって実装されました。 <sup>24.1</sup>
* スタイル管理を強化するための新しいパブリックプロパティ[priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/)、[unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/)、[semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/)が[Style](https://reference.aspose.com/words/python-net/aspose.words/style/)クラスに追加されました。 <sup>24.2</sup>
* 脚注と文末脚注の実際の参照マークテキストを取得する機能は、[actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/)プロパティと[update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default)メソッドで強化されました。 <sup>24.2</sup>
* WMFメタファイルのバイナリラスタ演算のエミュレーションが実装されました。 <sup>24.3</sup>
* **SaveOptions**内の文書の署名オプションを定義する機能は、新しいパブリックメンバーを持つ新しい[DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/)クラスを追加することと、[OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/)、[DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/)、[OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/)クラスに新しいプロパテ <sup>24.4</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.1リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.2リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.3リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 24.4リリースノート](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## .NET 経由の Python の Aspose.Words 23.9、23.10、23.11、23.12

Aspose.Words23.9レンダリングオプション、メタファイルレンダリングエミュレーション、およびmarkdown保存オプションを展開します。

Aspose.Words23.10レンダリングが改善され、文書の読み込みと保存のオプションが拡張され、ユーザーが新しい方法で文書をマージできるようになりました。Aspose.Words23.10

Aspose.Words23.11は、追加オプションを使用して、チャート凡例のリビジョン、XLSX形式、フォントを使用して作業を強化します。

Aspose.Words23.12は、PDFおよびOOXMLドキュメントを操作するための新しいプロパティと列挙、およびWebPイメージのサポートを導入します。

### レンダリングと印刷

#### DrawingMLチャートでの座標軸タイトルのカスタマイズ <sup>23.9</sup>

DrawingMLチャートの軸タイトルをカスタマイズする機能は、新しいパブリッククラス[ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/)および[title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/)プロパティの実装によって導入されました。

####  段落内のフォントの垂直位置の決定 <sup>23.9</sup>

新しいpublic[baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/)プロパティと新しい[BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/)列挙体を使用して、段落内のフォントの垂直位置を定義できるようになりました。

#### 前景色制御 <sup>23.10</sup>

修飾子なしで前景色を取得する機能が**BaseForeColor**プロパティを介して[Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/)クラスと[Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/)クラスに追加されました。

#### チャートの機能を拡張する <sup>23.10</sup>

[ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/)、[ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/)、[ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/)クラスの機能は、新しいメソッドとプロパティで拡張されました。

#### 画像を自動的に調整して図形に合わせる <sup>23.10</sup>

新しい[fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default)メソッドを使用して、画像を特定の形状に自動的に調整して合わせる簡単な方法が提供されています。

#### DrawingMLグラフの凡例エントリの既定のフォント書式設定 <sup>23.11</sup>

DrawingMLチャートの凡例エントリのデフォルトのフォント書式を指定する機能が[font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/)プロパティを介して追加されました。 この機能により、グラフ要素のより合理化された一貫した外観が容易になり、文書全体の美しさが向上します。

#### ReaderでPDFを開くときのページレイアウトの指定 <sup>23.12</sup>

PDFリーダーで文書を開くときに使用するページレイアウトを指定する機能は、[PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/)クラスに新しい[page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/)プロパティを導入し、新しい[PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/)列挙体を導入することによ

### 文書の読み込みと保存

#### イメージURIsをMarkdownに構築するフォルダ名の指定 <sup>23.9</sup>

[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)クラスは[images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/)プロパティを含めることで拡張され、Markdown文書に書き込まれたイメージURIsを構築するために使用されるフォルダの名前を指定できます。

#### PDF出力サイズを減らす <sup>23.10</sup>

[optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/)設定を使用するときに出力サイズを小さくするためのさまざまなPDFレンダリング最適化が実装されています。

#### TXT文書を読み込むときにハイパーリンクを認識する <sup>23.10</sup>

TXT文書の読み込み時にハイパーリンクを認識する機能は、新しい[detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/)プロパティを追加することによって実装されています。

### その他

- ラスタライズサイズを決定するためのメタファイルレンダリングエミュレーションが実装されました,特にWMFペン幅とEMF化粧ペン幅のために. これを実現するために、**ScaleWmfFontsToMetafileSize**プロパティは[emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/)プロパティに置き換えられ、[emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/)プロパティが追加されました。 <sup>23.9</sup>
- 現在のカーソル位置にある文書を別の文書に挿入するための簡略化された方法が[insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions)メソッドを使用して導入されました。 <sup>23.10</sup>
- 新しい[locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/)プロパティの導入により、スタイルプロパティにアクセスして変更する機能が追加されました。 <sup>23.10</sup>
- ジェネリック型パラメーターが[CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/)クラスのメソッドに追加されました。 <sup>23.10</sup>
- ドキュメントのすべてのセクションを同じXLSXワークシートに書き込む機能は、新しい[XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/)列挙型と新しい[section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/)プロパティによって提供されています。 <sup>23.11</sup>
* ZIP64書式拡張がOOXML文書にどのように使用されるかを制御する方法は、`OoxmlSaveOptions`クラスの新しいZip64Modeプロパティと新しいZip64Mode列挙体を介して実装されています。 <sup>23.12</sup>
* WebPイメージのサポートが導入されました。 この機能は以下のためにのみ利用可能ですのでご注意ください。NetStandartおよび.NET6+バージョン。 <sup>23.12</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 23.9リリースノート](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 23.10リリースノート](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 23.11リリースノート](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 23.12 リリースノート](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## .NET 経由の Python の Aspose.Words 23.5、23.6、23.7、23.8

Aspose.Words23.5は、グラフ系列データを操作する機能とODTドキュメントを操作する機能を強化し、ヘッダー/フッターとそのテキストの折り返しを改善します。Aspose.Words23.5は、グラフ系列データを操作する機能とODTドキュメントを操作する機能を強化します。

Aspose.Words23.6レンダリングオプションを展開し、新しいエクスポート形式を追加し、LINQレポートとLowCodeツールを改善します。

Aspose.Words23.7レポート機能が強化され、新しいエクスポート形式が追加され、テーブルとデジタル署名の操作に変更が加えられました。

Aspose.Words23.8は、さまざまな形式の機能を拡張し、レンダリングを改善し、フィールドを操作するための新しいオプションを追加します。

### サポートされている形式

* バージョン23.6以降では、文書をXLSX形式で保存することができます。 今、あなたはExcel形式に文書を変換することができます。 <sup>23.6</sup>

* バージョン23.7以降では、文書ページまたは図形をEPS形式で保存することができます。 <sup>23.7</sup>

### 新しいフォーマット機能

- MOBI文書の目次(TOC)を自動的に生成する機能が導入されました。 <sup>23.8</sup>
- [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions)コンストラクタは[PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions)で展開されています。 <sup>23.8</sup>
- EMFメタファイルの垂直テキストの整形が実装されました。 <sup>23.8</sup>

### レンダリング

#### グラフ系列データの取得と変更 <sup>23.5</sup>

グラフ系列データを取得および変更する機能は、以下を追加することによって提供されました:

- 新しいクラス: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- 新しい列挙型:[ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/),[ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### 高度なタイポグラフィのサポート <sup>23.6</sup>

WMF、EMF、EMF+レンダリングにおける高度なタイポグラフィのサポートが追加されました。

#### ページ上の色付きのコンテンツ <sup>23.6</sup>

ページが色付けされているかどうかを示すパブリックプロパティ[PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/)が追加されました。

#### チャートデータラベルの書式設定 <sup>23.6</sup>

チャートデータラベルの塗りつぶし、ストローク、および吹き出しの書式設定を設定する機能が実装されました。

### Mail Mergeと報告

#### LINQレポートエンジンの動的HTML挿入 <sup>23.6</sup>

LINQReporting Engineの動的HTML挿入の新しい方法が追加されました。

#### Mustacheタグのサポート <sup>23.7</sup>

Mustacheタグは[MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/)メソッドと[MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/)メソッドでサポートされるようになりました。

#### レンダリングされた画像のサイズの指定 <sup>23.8</sup>

レンダリングされた画像のサイズをピクセル単位で指定するための新しいパブリックプロパティ[image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/)が導入されました。

#### JSON文字列値の空白を保持する-LINQ <sup>23.8</sup>

LINQレポートエンジンに、JSON文字列値の空白を保持するオプションが追加されました。

### LowCode <sup>23.6</sup>

異なる種類の文書を単一の出力文書にマージするための新しいLowCodeメソッドが追加されました。

### その他

- ヘッダー/フッターでのテキスト折り返しのサポートが実装されました。 <sup>23.5</sup>
- ODT文書からデジタル署名を削除する機能が[RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str)メソッドによって追加されました。 <sup>23.5</sup>
- 音声ガイド[Run](https://reference.aspose.com/words/python-net/aspose.words/run/)のベーステキストとルビテキストを取得するためのパブリックプロパティ[phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/)が追加されました。 <sup>23.5</sup>
- 新しい[signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/)プロパティを導入することで、デジタル署名された文書からデジタル署名値をバイト配列として取得する機能が追加されました。 <sup>23.7</sup>
- [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/)クラスと[Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/)クラスは新しいパブリックメンバーで拡張されました– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), と[Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/)。 <sup>23.7</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 23.5リリースノート](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-5-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 23.6リリースノート](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-6-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 23.7リリースノート](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

詳細については、こちらをご覧ください [Aspose.WordsのためのPython via .NET 23.8リリースノート](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## また見て下さい

{{% alert color="primary" %}}

このページには、過去2年間の最新リリースニュースが含まれています。 以前のリリースの詳細については、以下を参照してください [リリースノート'](https://releases.aspose.com/words/python/release-notes/) 関連するセクションのページ。

{{% /alert %}}
