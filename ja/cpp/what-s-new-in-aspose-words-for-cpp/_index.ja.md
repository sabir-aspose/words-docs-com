---
title: 新着情報
second_title: C++の場合Aspose.Words
articleTitle: What's new in C++の場合Aspose.Words
linktitle: What's new in C++の場合Aspose.Words
type: docs
description: "C++の場合Aspose.Words 毎日拡大し、強化します。 このページでは、製品の巨大で最も興味深い機能について学ぶことができます。"
weight: 2
url: /ja/cpp/what-s-new-in-aspose-words-for-cpp/
timestamp: 2025-01-14-17-38-46
---

このページでは、最近のリリースで導入された最も興味深い新しいAspose.Words機能について説明します。

## C++の場合Aspose.Words 24.9、24.10、24.11、24.12

Aspose.Words24.9はDocumentBuilderを介してgroup shape挿入とStructuredDocumentTag挿入を導入し、目盛りによる放射状チャートレンダリングを強化し、XAdES-EPESサポートによるデジタル署名を改善し、Markdown下線認識を追加し、脚注/文末脚注セパレータへのアクセスを提供します。

Aspose.Words24.10は、CommandButtonの作成、新しい形状の可視性コントロール、group shapesへの機能、テーブルの改善されたMarkdownエクスポート、PieとDoughnutチャートのチャートフォーマット、より良いBig5エンコーディング処理、古い台湾のフォントのサポートにより、ActiveXコントロールのサポートが強化されています。

Aspose.Words24.11では、AIを使用したドキュメントの要約、強化されたレンダリングオプション、ドキュメントプロパティへのアクセスの改善、ActiveXコントロー

Aspose.Words 24.12 では、カスタマイズ可能なデータ ラベルの配置、Google AI を活用したテキスト翻訳、強化された差し込み印刷のクリーンアップ オプション、新しい LowCode 処理クラスが導入されています。

### AI を活用した機能

#### OpenAI と Google を使用したドキュメント要約 <sup>24.11</sup>

**OpenAI**および**Google**生成言語モデルを使用した文書要約のサポートは、[Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/)名前空間とそのパブリックメンバーを追加することによって統合されています。

#### Google の生成言語モデルを使用したテキスト翻訳 <sup>24.12</sup>

Google の生成言語モデルを使用してテキストを翻訳する機能は、[Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) メソッドと [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) 列挙を [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) 名前空間に追加することで、Aspose.Words に実装されました。

### ローコード <sup>24.12</sup>

[Comparer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/comparer/)、[MailMerger](https://reference.aspose.com/words/cpp/aspose.words.lowcode/merger/)、[Replacer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/replacer/)、[Splitter](https://reference.aspose.com/words/cpp/aspose.words.lowcode/splitter/) などの新しいローコード クラスが導入され、ドキュメント処理のシンプルさと柔軟性の完璧なバランスを実現する一連のメソッドが提供されます。

### レンダリングと印刷

#### ラジアルチャート上の目盛り

放射状チャート上の目盛りのレンダリングが実装されています。

#### CommandButtonActiveXコントロール <sup>24.10</sup>

新しいパブリックメソッド[InsertForms2OleControl](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertforms2olecontrol/)と新しいパブリッククラス**Forms2OleControl**を追加することにより、CommandButtonActiveXコントロールを作成する機能が導入されました。

#### 形状の可視性を制御する <sup>24.10</sup>

図形の可視性を制御するために、新しいパブリックプロパティ[Hidden](https://reference.aspose.com/words/cpp/aspose.words.drawing/shapebase/get_hidden/)が追加されました。

#### PieチャートとDoughnutチャートの変更点 <sup>24.10</sup>

書式PieおよびDoughnutチャートにいくつかの新しいパブリックプロパティが追加されました。

#### PDF選択フォームフィールドの境界線のレンダリングを制御します <sup>24.11</sup>

新しいパブリックオプション[RenderChoiceFormFieldBorder](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/get_renderchoiceformfieldborder/)を追加することにより、PDF選択フォームフィールド境界のレンダリングを制御する新しいオプションが実装されました。

#### グラフデータの書式コードの取得と設定 <sup>24.11</sup>

チャートデータの書式コードを取得および設定する機能は、[ChartXValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartxvaluecollection/)、[ChartYValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartyvaluecollection/)、および[BubbleSizeCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/bubblesizecollection/)クラスに[FormatCode](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/bubblesizecollection/get_formatcode/)プロパティを実装することによって追加されました。

#### ビンとラベルを使用したヒストグラムチャートのレンダリング <sup>24.11</sup>

ヒストグラムチャートレンダリングは、指定された数のビンとラベルを使用できるようにすることで改善されました。

#### データ ラベルの配置をカスタマイズする <sup>24.12</sup>

[ChartDataLabel](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabel/) クラスと [ChartDataLabelCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabelcollection/) クラスに新しいプロパティを導入することで、データ ラベルの配置をカスタマイズする機能が追加されました。

### 文書の変換、読み込み、保存

#### Markdownファイルを読み込むときの書式設定に下線を引きます

新しいパブリックプロパティ**ImportUnderlineFormatting**を追加することにより、Markdown文書を読み込むときに下線の書式を認識するオプションが組み込まれました。

#### Markdownに保存するときにテーブルをHTMLとしてエクスポートする <sup>24.10</sup>

文書をMarkdown形式で保存するときにテーブルをHTMLとしてエクスポートするオプションは、新しいパブリックプロパティ[ExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_exportashtml/)と列挙[MarkdownExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownexportashtml/)を追加することによ

#### 更新された論理構造を使用してPDFをエクスポートする <sup>24.11</sup>

PDFエクスポートは、テーブルタイトルプロパティをPDF論理構造要素のタイトルとして含めることで拡張されました。

### 差し込み印刷とレポート

#### 差し込み印刷中に空のテーブルを削除 <sup>24.12</sup>

差し込み印刷の出力を改良するために、[MailMergeCleanupOptions](https://reference.aspose.com/words/cpp/aspose.words.mailmerging/mailmergecleanupoptions/) 列挙に新しい **RemoveEmptyTables** オプションが追加されました。

### デジタル署名

#### XAdES-EPESを使用して文書に署名する

新しいパブリックプロパティ**XmlDsigLevel**と新しいパブリック列挙**XmlDsigLevel**を追加することにより、XAdES-EPESレベルXML-DSig署名で文書に署名する機能が導入されました。

### その他

* 新しいパブリックメソッド[InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/)がgroup shapesに追加されました。
* ドキュメントに**StructuredDocumentTags**を挿入するための新しいパブリックメソッド[InsertStructuredDocumentTag](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertstructureddocumenttag/)が追加されました。
* 脚注/文末脚注の区切り文字へのパブリックアクセスは、いくつかのパブリッククラスとプロパティを追加することによって提供されています。
* [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/)メソッドを追加することにより、個々の図形group shapesをグループ化し、図形とgroup shapesの両方を直接グループ化する機能が導入されました。 <sup>24.10</sup>
* TrueTypecmapテーブルのbig5エンコード処理が改善されました。 <sup>24.10</sup>
* 古い台湾語フォントのサポートが強化されました。 <sup>24.10</sup>
* 拡張ドキュメントプロパティにアクセスするために、読み取り専用プロパティが[BuiltInDocumentProperties](https://reference.aspose.com/words/cpp/aspose.words.properties/builtindocumentproperties/)クラスに追加されました。 <sup>24.11</sup>
* ActiveXコントロールのキャプションの設定は、**Forms2OleControl.Caption**プロパティに新しいパブリックセッターを追加することで有効になりました。 <sup>24.11</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [C++の場合Aspose.Words 24.9リリースノート](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-9-release-notes/).

詳細については、こちらをご覧ください [C++の場合Aspose.Words 24.10リリースノート](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-10-release-notes/).

詳細については、こちらをご覧ください [C++の場合Aspose.Words 24.11リリースノート](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-11-release-notes/).

詳細については、こちらをご覧ください [C++の場合Aspose.Words 24.12リリースノート](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-12-release-notes/).

{{% /alert %}}

## C++の場合Aspose.Words 24.5, 24.6, 24.7

Aspose.Words24.5アセンブリのオプションを展開し、レンダリング機能を向上させ、その他のオプションを展開します。

Aspose.Words24.6レンダリングオプションが改善され、検索と比較機能が強化され、他のいくつかの機能が拡張されました。

Aspose.Words24.7ActiveXの操作方法を変更し、レンダリング機能を拡張し、MarkdownおよびXLSX形式にエクスポートします。

### サポートされている形式

バージョン24.7からは、障害を持つユーザーのアクセシビリティを確保するためにPDF/UA-2へのエクスポートがサポートされています。

### レンダリングと印刷

#### チャート、図形、描画の変更 <sup>24.5</sup>

- DrawingMLエフェクトSVGグラフィックス用のレンダリングが実装されており、これまでの機能は画像に限定されていました。
- コンボチャートを作成し、系列グループ内のギャップ幅、オーバーラップ、バブルスケールなどのプロパティを調整するためのサポートは、**ChartSeriesGroup**クラスと**ChartSeriesGroupCollection**クラスと**SeriesGroups**
- 図形のSoftEdge効果を操作する機能は、**SoftEdgeFormat**クラスを追加することによって実装されています。
- 図形の調整値を変更する機能は、**AdjustmentCollection**と**Adjustment**パブリッククラスと**Adjustments**プロパティを追加することによって実装されています。

#### チャート、図形、図面の変更 <sup>24.6</sup>

- グラフ作成機能が強化されました。 これで、次のようなさまざまなグラフを作成できます*Treemaps*, *Sunbursts*, *Histograms*, *Pareto* チャート、*Box & Whisker*チャート、*Waterfalls*、および*Funnels*。 これにより、より多様で有益な方法でデータを視覚化することができます。
- 影の書式設定のカラーコントロールが改善されました。 影の色にアクセスすることで、ドキュメントの外観をより正確に制御できます。
- バックグラウンドレンダリングのパフォーマンス向上が改善されました。 ネイティブのタイル技術のおかげで、小さな要素を含む背景のレンダリングを大幅に高速化できます。
- 形状のための現実的なグラデーションが追加されました。 非線形グラデーションを使用してDML図形を作成し、Microsoft Wordの視覚スタイルを模倣して、より洗練された外観にすることができます。

#### チャートデータラベルのカスタマイズ <sup>24.7</sup>

**Orientation**や**Rotation**などのチャートデータラベルをカスタマイズする機能が追加されました。

#### リストレベルのカスタム番号スタイル <sup>24.7</sup>

パブリックプロパティ[CustomNumberStyleFormat](https://reference.aspose.com/words/cpp/aspose.words.lists/listlevel/get_customnumberstyleformat/)のセッターが追加されました。 リストレベルのカスタム番号スタイルを定義できるようになりました。

#### ActiveXでの作業の変更点 <sup>24.7</sup>

- ActiveXオブジェクトのプロパティを変更できるようになり、その動作をより詳細に制御できるようになりました。
- 動的相互作用を有効にするために、ラジオボタンのActiveXコントロールの値を変更する機能が追加されました。
- ActiveXチェックボックスを"チェック済み"または"チェックされていない"に切り替える機能が追加されました。

### 文書の読み込みと保存

#### Markdown形式へのリンクのエクスポート <sup>24.7</sup>

[LinkExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_linkexportmode/)プロパティの実装により、Markdown形式のリンクのエクスポートを制御する機能が追加されました。

### 検索と比較

#### 高度な比較オプション <sup>24.6</sup>

改善された比較機能を備えたデータ分析ワークフローを合理化する機能が追加されました。 これには、新しい**IgnoreStoreItemId**オプションと、高度な比較のための再設計されたインターフェイスが含まれます。

### その他

- ドキュメントから空のページを削除する関数は、[RemoveBlankPages](https://reference.aspose.com/words/cpp/aspose.words/document/removeblankpages/)メソッドを追加することによって実装されています。 <sup>24.5</sup>
- ドキュメントをロードせずにVBAマクロの存在を確認する機能は、**HasMacros**プロパティを追加することによって提供されています。 <sup>24.5</sup>
- 新しい**DateTimeUtc**プロパティが追加されました–これにより、コメントのより正確なタイムスタンプが提供され、組織とトレーサビ <sup>24.6</sup>
- Xlsx形式へのシームレスなエクスポートのために、datetime形式が自動的に検出されるようになりました。 <sup>24.7</sup>
- Vbaプロジェクトが保護されているかどうかを確認できるパブリックプロパティ[IsProtected](https://reference.aspose.com/words/cpp/aspose.words.vba/vbaproject/get_isprotected/)が追加されました。 <sup>24.7</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [C++の場合Aspose.Words 24.5リリースノート](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-5-release-notes/).

詳細については、こちらをご覧ください [C++の場合Aspose.Words 24.6リリースノート](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-6-release-notes/).

詳細については、こちらをご覧ください [C++の場合Aspose.Words 24.7リリースノート](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-7-release-notes/).

{{% /alert %}}

## C++の場合Aspose.Words 24.1, 24.2, 24.3, 24.4

Aspose.Words24.1ストロークの色の管理に関する操作性が向上し、OLEオブジェクトが強化され、新しい参考文献ソースパブリックAPIが導入されました。

Aspose.Words24.2チャートAPIとスタイル管理を拡張しました。 このバージョンのAspose.Wordsでは、レンダリング中にSvgSaveOptionsを指定する機能、Markdownファイルを読み込む柔軟な制御、脚注と文末脚注の参照テキストを操作する機能も導入されました。

Aspose.Words24.3はWMFメタファイルのバイナリラスタ演算のエミュレーションを導入し、Charts APIも拡張し続けています。

Aspose.Words24.4いくつかのレンダリングオプションを強化し、デジタル署名の作業を改善します。

### レンダリングと印刷

#### ストロークカラーコントロール <sup>24.1</sup>

[Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/)クラスは、ストロークの色の管理に関連する一連の新しいパブリックプロパティ[ForeThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_forethemecolor/)と[BackThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backthemecolor/)、[ForeTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_foretintandshade/)と[BackTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backtintandshade/)で拡張されました。

#### DrawingMLチャートAPI拡張機能 <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API**は引き続き展開されます。

#### @font-faceルールで宣言された埋め込みフォント <sup>24.4</sup>

@font-faceルールで宣言されたフォントを結果のドキュメントのフォント定義に埋め込む機能を追加しました新しい[SupportFontFaceRules](https://reference.aspose.com/words/cpp/aspose.words.loading/htmlloadoptions/get_supportfontfacerules/)プロパティを追加することによ

#### グローとリフレクションの書式設定を使用する <sup>24.4</sup>

描画オブジェクトのグローとリフレクションの書式設定を操作する機能が実装されました。

### 文書の読み込みと保存

#### レンダリング中にSvgSaveOptionsを指定します <sup>24.2</sup>

レンダリング中に[SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/)を指定する機能が[ShapeRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/shaperenderer/)を使用して追加されました。[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/)と[OfficeMathRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/officemathrenderer/)。[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/)メソッド。

#### Markdownファイルの読み込み時に空行を保持する <sup>24.2</sup>

Markdownファイルの読み込み時に空行を保持する機能が追加されました。

### その他

- 新しい**TextBoxControl**クラスに新しい**Text**プロパティを追加することで、`TextBox`OLEコントロールのテキストを変更する機能が導入されました。 <sup>24.1</sup>
- Bibliography Sources public APIは、新しいクラスと列挙を含む新しい名前空間[Aspose.Words.Bibliography](https://reference.aspose.com/words/cpp/aspose.words.bibliography/)の追加と、新しい[Bibliography](https://reference.aspose.com/words/cpp/aspose.words/document/get_bibliography/)プロパティを[Document](https://reference.aspose.com/words/cpp/aspose.words/document/)クラスに追加することによって実装されました。 <sup>24.1</sup>
- スタイル管理を強化するための新しいパブリックプロパティ[Priority](https://reference.aspose.com/words/cpp/aspose.words/style/get_priority/)、[UnhideWhenUsed](https://reference.aspose.com/words/cpp/aspose.words/style/get_unhidewhenused/)、[SemiHidden](https://reference.aspose.com/words/cpp/aspose.words/style/get_semihidden/)が[Style](https://reference.aspose.com/words/cpp/aspose.words/style/)クラスに追加されました。 <sup>24.2</sup>
- 脚注と文末脚注の実際の参照マークテキストを取得する機能は、[ActualReferenceMark](https://reference.aspose.com/words/cpp/aspose.words.notes/footnote/get_actualreferencemark/)プロパティと[UpdateActualReferenceMarks](https://reference.aspose.com/words/cpp/aspose.words/document/updateactualreferencemarks/)メソッドで強化されました。 <sup>24.2</sup>
- WMFメタファイルのバイナリラスタ演算のエミュレーションが実装されています。 <sup>24.3</sup>
- **SaveOptions**内の文書の署名オプションを定義する機能は、新しいパブリックメンバーを持つ新しい**DigitalSignatureDetails**クラスを追加し、[OoxmlSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/ooxmlsaveoptions/)、[DocSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/docsaveoptions/)、[OdtSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/odtsaveoptions/)クラスに新しいプロパティを追加する <sup>24.4</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [C++の場合Aspose.Words 24.1リリースノート](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-1-release-notes/).

詳細については、こちらをご覧ください [C++の場合Aspose.Words 24.2リリースノート](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-2-release-notes/).

詳細については、こちらをご覧ください [C++の場合Aspose.Words 24.3リリースノート](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-3-release-notes/).

詳細については、こちらをご覧ください [C++の場合Aspose.Words 24.4リリースノート](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-4-release-notes/).

{{% /alert %}}

## C++の場合Aspose.Words 23.9, 23.10, 23.11, 23.12

Aspose.Words23.9レンダリングオプション、メタファイルレンダリングエミュレーション、およびmarkdown保存オプションを展開します。

Aspose.Words 23.10 はレンダリングを改善し、ドキュメントの読み込みと保存のオプションを拡張し、ユーザーが新しい方法でドキュメントを結合できるようにします。

Aspose.Words23.11は、追加オプションを使用して、チャートの凡例上のリビジョン、XLSX形式、フォントでの作業を強化します。

Aspose.Words23.12は、PDFおよびOXMLドキュメントを操作するための新しいプロパティと列挙、およびWebPイメージのサポートを導入します。

### レンダリングと印刷

#### Drawingmlチャートでの軸タイトルのカスタマイズ <sup>23.9</sup>

Drawingmlチャートの軸タイトルをカスタマイズする機能は、新しいpublic class**ChartAxisTitle**および[Title](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartaxis/get_title/)プロパティの実装によって導入されました。

#### 段落内のフォントの垂直位置の決定 <sup>23.9</sup>

新しいpublic[BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/paragraphformat/get_baselinealignment/)プロパティと新しい[BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/baselinealignment/)列挙体を使用して、段落内のフォントの垂直位置を定義できるようになりました。

#### 前景色制御 <sup>23.10</sup>

修飾子なしで前景色を取得する機能が**BaseForeColor**プロパティを介して[Fill](https://reference.aspose.com/words/cpp/aspose.words.drawing/fill/)クラスと[Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/)クラスに追加されました。

#### チャートの機能を拡張する <sup>23.10</sup>

[ChartDataPointCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatapointcollection/)、[ChartSeries](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartseries/)、[ChartFormat](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartformat/)クラスの機能は、新しいメソッドとプロパティで拡張されました。

#### 画像を自動的に調整して図形に合わせる <sup>23.10</sup>

新しい[FitImageToShape](https://reference.aspose.com/words/cpp/aspose.words.drawing/imagedata/fitimagetoshape/)メソッドを使用して、画像を特定の形状に自動的に調整して合わせる簡単な方法が提供されています。

#### Drawingmlグラフの凡例エントリの既定のフォント書式設定 <sup>23.11</sup>

Drawingmlチャートの凡例エントリのデフォルトのフォント書式を指定する機能が[Font](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartlegend/get_font/)プロパティを介して追加されました。 この機能により、グラフ要素のより合理化された一貫した外観が容易になり、文書全体の美しさが向上します。

#### ReaderでPDFを開くときのページレイアウトの指定 <sup>23.12</sup>

PDFリーダーで文書を開くときに使用するページレイアウトを指定する機能は、[PdfSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/)クラスに新しい**PageLayout**プロパティを導入し、新しい**PdfPageLayout**列挙体を導入することによ

### 文書の読み込みと保存

#### イメージURIsをMarkdownに構築するフォルダ名の指定 <sup>23.9</sup>

[MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/)クラスは[ImagesFolderAlias](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imagesfolderalias/)プロパティを含めることで拡張され、Markdown文書に書き込まれたイメージURIsを構築するために使用されるフォルダの名前を指定できます。

#### PDF出力サイズを減らす <sup>23.10</sup>

[OptimizeOutput](https://reference.aspose.com/words/cpp/aspose.words.saving/fixedpagesaveoptions/get_optimizeoutput/)設定を使用するときに出力サイズを小さくするためのさまざまなPDFレンダリング最適化が実装されています。

#### TXT文書を読み込むときにハイパーリンクを認識する <sup>23.10</sup>

TXT文書の読み込み時にハイパーリンクを認識する機能は、新しい[DetectHyperlinks](https://reference.aspose.com/words/cpp/aspose.words.loading/txtloadoptions/get_detecthyperlinks/)プロパティを追加することによって実装されています。

### その他

- ラスタライズサイズを決定するメタファイルレンダリングエミュレーションが、特にWMFペン幅とEMF化粧ペン幅のために実装されています。 これを実現するために、**ScaleWmfFontsToMetafileSize**プロパティは[EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpage/)プロパティに置き換えられ、[EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpageresolution/)プロパティが追加されました。 <sup>23.9</sup>
* 現在のカーソル位置にある文書を別の文書に挿入するための簡略化された方法が[InsertDocumentInline](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertdocumentinline/)メソッドを使用して導入されました。 <sup>23.10</sup>
* 新しい[Locked](https://reference.aspose.com/words/cpp/aspose.words/style/get_locked/)プロパティの導入により、スタイルプロパティにアクセスして変更する機能が追加されました。 <sup>23.10</sup>
* ジェネリック型パラメーターが[CompositeNode](https://reference.aspose.com/words/cpp/aspose.words/compositenode/)クラスのメソッドに追加されました。 <sup>23.10</sup>
* 特定のリビジョンを受け入れる/拒否するかどうかを制御する方法は、[Accept](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/accept/)メソッドと[Reject](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/reject/)メソッドを使用して実装されています。 この機能強化により、ユーザーは改訂プロセスをより細かく制御できます。 <sup>23.11</sup>
* 文書のすべてのセクションを同じXLSXワークシートに書き込む機能は、新しい[XlsxSectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsectionmode/)列挙型と新しい[SectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsaveoptions/get_sectionmode/)プロパティによって提供されています。 <sup>23.11</sup>
* OXMLドキュメントにZIP64形式拡張を使用する方法を制御する方法は、`OoxmlSaveOptions`クラスの新しいZip64Modeプロパティと新しいZip64Mode列挙体を使用して実装されてい <sup>23.12</sup>
* WebPイメージのサポートが導入されました。 この機能は以下のためにのみ利用可能ですのでご注意ください。NetStandartおよび.NET6+バージョン。 <sup>23.12</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [C++の場合Aspose.Words 23.9リリースノート](/words/cpp/aspose-words-for-cpp-23-9-release-notes/).
詳細については、こちらをご覧ください [C++の場合Aspose.Words 23.10リリースノート](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-10-release-notes/).
詳細については、こちらをご覧ください [C++の場合Aspose.Words 23.11リリースノート](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-11-release-notes/).
詳細については、こちらをご覧ください [C++の場合Aspose.Words 23.12リリースノート](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-12-release-notes/).

{{% /alert %}}

## また見て下さい

{{% alert color="primary" %}}

このページには、過去2年の最新リリースニュースが含まれています。 以前のリリースの詳細については、以下を参照してください [リリースノート'](/words/cpp/release-notes/) 関連するセクションのページ。

{{% /alert %}}
