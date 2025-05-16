---
title: 新着情報
second_title: Aspose.Wordsのための.NET
articleTitle: What's new in Aspose.Wordsのための.NET
linktitle: What's new in Aspose.Wordsのための.NET
type: docs
description: "Aspose.Wordsのための.NET 毎日拡大し、強化します。 このページでは、製品の巨大で最も興味深い機能について学ぶことができます。"
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ja/net/what-s-new-in-aspose-words-for-net/
timestamp: 2025-04-16-07-02-05
---

このページでは、最近のリリースで導入された最も興味深い新しいAspose.Words機能について説明します。

## Aspose.Wordsのための.NET 25.1, 25.2, 25.3, 25.4

Aspose.Words25.1はAIを使用した文法チェックを導入し、HTML、SVG、Markdown形式の高度なオプションを使用して文書の保存を強化します。

Aspose.Words25.2はAnthropicAIモデルによるテキスト要約を導入し、MsWorks形式のサポートを追加し、タイポグラフィ制御を強化し、PDF構造とリストの処理を改善します。

Aspose.Words25.3AIを使用した文法チェッカーとフォントの選択をUpdateAmbiguousTextFontプロパティで強化し、PDF添付ファイルのエクスポートを改善しました。

Aspose.Words25.4は新しい用紙サイズのサポートを導入し、高度なHTML輸出管理を可能にし、透かしの処理を改善し、LowCodeAPIの使いやすさを向上させます。

### AI搭載の機能

#### 文書AI文法チェック

* OpenAI生成モデルを使用して提供された文書の文法をチェックする機能は、新しい[CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/)メソッドを追加することによって導入されました。 <sup>25.1</sup>
* AIを使用した文法チェック機能が更新され、[AiModelType](https://reference.aspose.com/words/net/aspose.words.ai/aimodeltype/)列挙体で使用可能なすべてのモデルがサポートされました。 <sup>25.3</sup>

#### Anthropic生成言語モデルを使用した要約 <sup>25.2</sup>

新しいパブリッククラス[AnthropicAiModel](https://reference.aspose.com/words/net/aspose.words.ai/anthropicaimodel/)を導入することにより、Anthropic生成言語モデルを使用したテキスト要約が可能になりました。

### Low Code

#### Low CodeAPIユーザビリティ <sup>25.4</sup>

**LowCode API**の使いやすさが大幅に改善され、文書処理が簡素化され、反復的なコードの必要性が軽減されました。

### サポートされている形式 <sup>25.2</sup>

バージョン25.2から、MicrosoftWorksドキュメントの新しいMsWorksロード形式との互換性が追加されました。

### ドキュメントの変換、読み込み、保存

#### HTML形式とSVG形式への保存を改善しました <sup>25.1</sup>

[HtmlFixedSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlfixedsaveoptions/)クラスと[SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/)クラスの両方に**IdPrefix**プロパティと**RemoveJavaScriptFromLinks**プロパティを追加することで、HTML形式とSVG形式への保存が強化されました。

#### 保存時の画像解像度とOfficeMath出力モードをMarkdownに設定します <sup>25.1</sup>

* 画像の解像度を設定するための新しい[ImageResolution](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imageresolution/)オプションが[MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/)クラスに追加されました。
* 新しい[OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/officemathexportmode/)オプションと[MarkdownOfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownofficemathexportmode/)列挙体が[MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/)クラスに追加され、OfficeMath出力モードを設定しました。
* ストリームから画像の透かしを設定する機能は、[SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage_2)メソッドに新しいオーバーロードを追加することによって導入されました。 <sup>25.4</sup>

### レンダリング

#### 改善されたタイポグラフィ制御 <sup>25.2</sup>

[NumberSpacing](https://reference.aspose.com/words/net/aspose.words/font/numberspacing/)プロパティは、タイポグラフィ制御を改善するために追加されました。

#### あいまいな文字のフォント選択の制御 <sup>25.3</sup>

新しいパブリックプロパティ[UpdateAmbiguousTextFont](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/updateambiguoustextfont/)が[SaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/)クラスに追加され、使用される文字コードに従ってフォントの選択を制御します。

#### 用紙サイズオプション <sup>25.4</sup>

JISB4とJISB5用紙サイズを使用する機能は、[PaperSize](https://reference.aspose.com/words/net/aspose.words/papersize/)列挙体に新しい値を追加することによって導入されました。

#### HTML出力制御 <sup>25.4</sup>

HTMLエクスポート中にJavaScriptをハイパーリンクURLsから削除する機能は、[RemoveJavaScriptFromLinks](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/removejavascriptfromlinks/)プロパティを追加することによって導入されました。

### その他

* PDF論理構造が改善され、TOA、BIBLIOGRAPHY、INDEXフィールドがサポートされました。 <sup>25.2</sup>
* リストの処理を改善するために[AddSingleLevelList](https://reference.aspose.com/words/net/aspose.words.lists/listcollection/addsinglelevellist/)メソッドが導入されました。 <sup>25.2</sup>
* PDF添付ファイルのエクスポートを改善するために**EmbedAttachments**を置き換える新しいプロパティ[AttachmentsEmbeddingMode](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/attachmentsembeddingmode/)が追加されました。 また、PDF/Aバージョンの添付ファイルをサポートするために、[PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/)列挙体に新しい値が追加されました。 さらに、添付ファイルは暗号化でサポートされるようになりました。 <sup>25.3</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 25.1 リリースノート](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-1-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 25.2 リリースノート](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-2-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 25.3 リリースノート](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-3-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 25.4 リリースノート](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-4-release-notes/).

{{% /alert %}}

## Aspose.Wordsのための.NET 24.9, 24.10, 24.11, 24.12

Aspose.Words24.9はDocumentBuilderを介してgroup shape挿入とStructuredDocumentTag挿入を導入し、目盛りによる放射状チャートレンダリングを強化し、XAdES-EPESサポートによるデジタル署名を改善し、Markdown下線認識を追加し、脚注/文末脚注セパレータへのアクセスを提供します。

Aspose.Words24.10はCommandButton作成による強化されたActiveXコントロールサポート、新しい形状の可視性コントロール、group shapesへの機能、テーブルの改善されたMarkdownエクスポート、PieとDoughnutチャートのチャー

Aspose.Words24.11はAIを活用した文書の要約、強化されたレンダリングオプション、文書のプロパティへのアクセスの改善、ActiveXコントロールキャプションを導入します。Aspose.Words24.11はAI

Aspose.Words24.12では、カスタマイズ可能なデータラベルの配置、GoogleAIによるテキスト翻訳、強化されたMail Mergeクリーンアップオプション、新しいLowCode処理クラスが導入されま

### AI搭載の機能

#### OpenAIとGoogleを使用した文書の要約 <sup>24.11</sup>

**OpenAI**および**Google**生成言語モデルを使用した文書要約のサポートは、[Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)名前空間とそのパブリックメンバーを追加することによって統合されています。

#### Googleの生成言語モデルを使用したテキスト翻訳 <sup>24.12</sup>

Googleの生成言語モデルを使用してテキストを翻訳する機能は、Aspose.Wordsに[Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/)メソッドと[Language](https://reference.aspose.com/words/net/aspose.words.ai/language/)列挙体を[Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)名前空間に追加することによって実装されています。

### Low Code <sup>24.12</sup>

新しいLowCodeクラスのような[Comparer](https://reference.aspose.com/words/net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/net/aspose.words.lowcode/splitter/) など。 文書処理のための簡易性と柔軟性間の完全なバランスを打つ一組の方法を提供する導入された。

### レンダリングと印刷

#### ラジアルチャート上の目盛り <sup>24.9</sup>

放射状チャート上の目盛りのレンダリングが実装されています。

#### CommandButtonActiveXコントロール <sup>24.10</sup>

CommandButtonActiveXコントロールを作成する機能は、新しいパブリックメソッド[InsertForms2OleControl](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertforms2olecontrol/)と新しいパブリッククラス[Forms2OleControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/)を追加することによって導入されました。

#### 形状の可視性を制御する <sup>24.10</sup>

図形の可視性を制御するために、新しいパブリックプロパティ[Hidden](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/hidden/)が追加されました。

#### PieチャートとDoughnutチャートの変更点 <sup>24.10</sup>

書式PieおよびDoughnutチャートにいくつかの新しいパブリックプロパティが追加されました。

#### PDF選択フォームフィールドの境界線のレンダリングを制御します <sup>24.11</sup>

新しいパブリックオプション[RenderChoiceFormFieldBorder](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/renderchoiceformfieldborder/)を追加することにより、PDF選択フォームフィールド境界のレンダリングを制御する新しいオプションが実装されました。

#### グラフデータの書式コードの取得と設定 <sup>24.11</sup>

チャートデータの書式コードを取得および設定する機能は、[ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/)、[ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/)、および[BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/)クラスに[FormatCode](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/formatcode/)プロパティを実装することによって追加されました。

#### ビンとラベルを使用したヒストグラムチャートのレンダリング <sup>24.11</sup>

ヒストグラムチャートレンダリングは、指定された数のビンとラベルを使用できるようにすることで改善されました。

#### データラベルの配置をカスタマイズする <sup>24.12</sup>

[ChartDataLabel](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabel/)クラスと[ChartDataLabelCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/)クラスに新しいプロパティを導入することで、データラベルの配置をカスタマイズする機能が追加されました。

### 文書の変換、読み込み、保存

#### Markdownファイルを読み込むときの書式設定に下線を引きます <sup>24.9</sup>

新しいパブリックプロパティ[ImportUnderlineFormatting](https://reference.aspose.com/words/net/aspose.words.loading/markdownloadoptions/importunderlineformatting/)を追加することにより、Markdown文書を読み込むときに下線の書式を認識するオプションが組み込まれました。

#### Markdownに保存するときにテーブルをHTMLとしてエクスポートする <sup>24.10</sup>

文書をMarkdown形式で保存するときにテーブルをHTMLとしてエクスポートするオプションは、新しいパブリックプロパティ[ExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/exportashtml/)と列挙[MarkdownExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownexportashtml/)を追加することによ

#### 更新された論理構造を使用してPDFをエクスポートする <sup>24.11</sup>

PDFエクスポートは、テーブルタイトルプロパティをPDF論理構造要素のタイトルとして含めることで拡張されました。

### Mail Mergeと報告

#### Mail Merge中に空のテーブルを削除する <sup>24.12</sup>

新しい**RemoveEmptyTables**オプションが[MailMergeCleanupOptions](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmergecleanupoptions/)列挙体に追加され、Mail Merge出力を調整しました。

### デジタル署名

#### XAdES-EPESで文書に署名する <sup>24.9</sup>

新しいパブリックプロパティ[XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/signoptions/xmldsiglevel/)と新しいパブリック列挙[XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/xmldsiglevel/)を追加することにより、XAdES-EPESレベルXML-DSig署名で文書に署名する機能が導入されました。

### その他

* 新しいパブリックメソッド[InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/)がgroup shapesに追加されました。 <sup>24.9</sup>
* ドキュメントに**StructuredDocumentTags**を挿入するための新しいパブリックメソッド[InsertStructuredDocumentTag](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertstructureddocumenttag/)が追加されました。 <sup>24.9</sup>
* 脚注/文末脚注の区切り文字へのパブリックアクセスは、いくつかのパブリッククラスとプロパティを追加することによって提供されています。 <sup>24.9</sup>
* [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/#insertgroupshape_1)メソッドを追加することにより、個々の図形group shapesをグループ化し、図形とgroup shapesの両方を直接グループ化する機能が導入されました。 <sup>24.10</sup>
* TrueTypecmapテーブルのbig5エンコード処理が改善されました。 <sup>24.10</sup>
* 古い台湾語フォントのサポートが強化されました。 <sup>24.10</sup>
* 拡張ドキュメントプロパティにアクセスするために、読み取り専用プロパティが[BuiltInDocumentProperties](https://reference.aspose.com/words/net/aspose.words.properties/builtindocumentproperties/)クラスに追加されました。 <sup>24.11</sup>
* ActiveXコントロールのキャプションの設定は、[Forms2OleControl.Caption](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/caption/)プロパティに新しいpublicセッターを追加することで有効になりました。 <sup>24.11</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.9 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-9-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.10 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-10-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.11 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-11-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.12 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-12-release-notes/).

{{% /alert %}}

## Aspose.Wordsのための.NET 24.5, 24.6, 24.7, 24.8

Aspose.Words24.5アセンブリのオプションを展開し、レンダリング機能を向上させ、その他のオプションを展開します。

Aspose.Words24.6レンダリングオプションが改善され、検索と比較機能が強化され、他のいくつかの機能が拡張されました。

Aspose.Words24.7はActiveXの操作方法を変更し、レンダリング機能を拡張し、Markdown形式とXLSX形式にエクスポートします。

Aspose.Words24.8軸ラベルを正確に制御してグラフのカスタマイズを強化し、フォント管理を拡張し、文書構造の処理を改善し、HTML/XAMLエクスポート、PDF機能、文書変換、デジタ

### サポートされている形式

バージョン24.7からは、障害を持つユーザーのアクセシビリティを確保するためにPDF/UA-2へのエクスポートがサポートされています。

### プラットフォーム <sup>24.5</sup>

.NET 7.0/8.0アセンブリはAspose.WordsNuGetパッケージに含まれています。

### レンダリングと印刷

#### チャート、図形、およびDrawingMLの変更 <sup>24.5</sup>

* DrawingMLエフェクトSVGグラフィックスのレンダリングが実装されており、これまでの機能は画像に限定されていました。
* コンボチャートを作成し、系列グループ内のギャップ幅、オーバーラップ、バブルスケールなどのプロパティを調整するためのサポートは、[ChartSeriesGroup](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroup/)クラスと[ChartSeriesGroupCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroupcollection/)クラスと[SeriesGroups](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/seriesgroups/)
* 図形のSoftEdge効果を操作する機能は、[SoftEdgeFormat](https://reference.aspose.com/words/net/aspose.words.drawing/softedgeformat/)クラスを追加することによって実装されています。
* 図形の調整値を変更する機能は、[AdjustmentCollection](https://reference.aspose.com/words/net/aspose.words.drawing/adjustmentcollection/)と[Adjustment](https://reference.aspose.com/words/net/aspose.words.drawing/adjustment/)パブリッククラスと[Adjustments](https://reference.aspose.com/words/net/aspose.words.drawing/shape/adjustments/)プロパティを追加することによって実装されています。

#### チャート、図形、図面の変更 <sup>24.6</sup>

* グラフ作成機能が強化されました。 これで、次のようなさまざまなグラフを作成できます*Treemaps*, *Sunbursts*, *Histograms*, *Pareto* チャート、*Box & Whisker*チャート、*Waterfalls*、および*Funnels*。 これにより、より多様で有益な方法でデータを視覚化することができます。
* 影の書式設定のカラーコントロールが改善されました。 影の色にアクセスすることで、ドキュメントの外観をより正確に制御できます。
* バックグラウンドレンダリングのパフォーマンス向上が改善されました。 ネイティブのタイル技術のおかげで、小さな要素を含む背景のレンダリングを大幅に高速化できます。
* 形状のための現実的なグラデーションが追加されました。 非線形グラデーションを持つDML図形を作成し、Microsoft Wordの視覚スタイルを模倣して、より洗練された外観にすることができます。

#### チャートデータラベルのカスタマイズ <sup>24.7</sup>

**Orientation**や**Rotation**などのチャートデータラベルをカスタマイズする機能が追加されました。

#### リストレベルのカスタム番号スタイル <sup>24.7</sup>

パブリックプロパティ[CustomNumberStyleFormat](https://reference.aspose.com/words/net/aspose.words.lists/listlevel/customnumberstyleformat/)のセッターが追加されました。 リストレベルのカスタム番号スタイルを定義できるようになりました。

#### ActiveXでの作業の変更点 <sup>24.7</sup>

* ActiveXオブジェクトのプロパティを変更できるようになり、その動作をより詳細に制御できるようになりました。
* ラジオボタンActiveXコントロールの値を変更して動的相互作用を有効にする機能が追加されました。
* ActiveXcheckboxを"checked"または"unchecked"に切り替える機能が追加されました。

#### チャート軸の目盛りラベルの向きと回転の制御 <sup>24.8</sup>

グラフのカスタマイズをより便利にするために、グラフ軸の目盛りラベルの向きと回転を正確に制御できるようになりました。[AxisTickLabels](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/)クラスは新しい[Orientation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/orientation/)と[Rotation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/rotation/)プロパティで拡張されました。

#### 円記号を円記号に置き換える <sup>24.8</sup>

バックスラッシュ文字を円記号に置き換えるための後方互換性のあるHTMLとXAMLエクスポートが改善されました。 これを実現するために、**ReplaceBackslashWithYenSign**プロパティが[HtmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/)クラスと[XamlFlowSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xamlflowsaveoptions/)クラスに追加されました。

#### PDFにエクスポートするときにSDTタグをフォームフィールド名として使用する <sup>24.8</sup>

[PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)クラスに新しい[UseSdtTagAsFormFieldName](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/usesdttagasformfieldname/)プロパティを追加することで、SDTタグをフォームフィールド名として使用することをサポートしたPDFエクスポートが強化されました。[PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)クラスに新しい[UseSdtTagAsFormFieldName](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/usesdttagasformfieldname/)プロパティを追加しました。

### 文書の変換、読み込み、保存

#### Markdown形式へのリンクのエクスポート <sup>24.7</sup>

[LinkExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/linkexportmode/)プロパティの実装により、Markdown形式のリンクのエクスポートを制御する機能が追加されました。

#### LowCode 24.8 <sup>24.8</sup>

さまざまなドキュメントタイプを1行のコードで変換するための一連のメソッドを提供するように設計された新しい[LowCode.Converter](https://reference.aspose.com/words/net/aspose.words.lowcode/converter/)クラスが導入されました。

### 検索と比較

#### 高度な比較オプション <sup>24.6</sup>
改善された比較機能を備えたデータ分析ワークフローを合理化する機能が追加されました。 これには、新しい[IgnoreStoreItemId](https://reference.aspose.com/words/net/aspose.words.comparing/advancedcompareoptions/ignorestoreitemid/)オプションと、高度な比較のための再設計されたインターフェイスが含まれます。

### その他

* ドキュメントから空のページを削除する関数は、[RemoveBlankPages](https://reference.aspose.com/words/net/aspose.words/document/removeblankpages/)メソッドを追加することによって実装されています。 <sup>24.5</sup>
* ドキュメントをロードせずにVBAマクロの存在をチェックする機能は、[HasMacros](https://reference.aspose.com/words/net/aspose.words/fileformatinfo/hasmacros/)プロパティを追加することによって提供されています。 <sup>24.5</sup>
* LINQレポートエンジンを使用して文書を挿入する際にソース番号を保持することがサポートされるようになりました。 <sup>24.5</sup>
* 新しい[DateTimeUtc](https://reference.aspose.com/words/net/aspose.words/comment/datetimeutc/)プロパティが追加されました–これにより、コメントのより正確なタイムスタンプが提供され、組織とトレーサビ <sup>24.6</sup>
* LINQレポートエンジンが改善されました。 空の段落を選択的に削除し、欠落しているオブジェクトメンバーのカスタムメッセージを定義することで、よりクリーンで有益なレポートが作成されました。 <sup>24.6</sup>
* XLSX形式へのシームレスなエクスポートのために、datetime形式が自動的に検出されるようになりました。 <sup>24.7</sup>
* VBAプロジェクトが保護されているかどうかを確認できるパブリックプロパティ[IsProtected](https://reference.aspose.com/words/net/aspose.words.vba/vbaproject/isprotected/)が追加されました。 <sup>24.7</sup>
* フォント情報は、[FontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/fontinfo/)クラスと[PhysicalFontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/physicalfontinfo/)クラスに**EmbeddingLicensingRights**プロパティが追加されて拡張されました。 <sup>24.8</sup>
* 透かしを保持しながら、効率的にセクションのヘッダーとフッターをクリアする方法は、より正確に文書構造を操作するために追加されました。 セクションヘッダーとフッターをクリアするには、新しいpublicメソッド[ClearHeadersFooters](https://reference.aspose.com/words/net/aspose.words/section/clearheadersfooters/)を使用します。 <sup>24.8</sup>
* [XpsSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/)を使用したXPS文書のデジタル署名が有効になりました–この目的のために新しいプロパティ[DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/digitalsignaturedetails/)が追加されました。 <sup>24.8</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.5 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-5-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.6 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-6-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.7 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-7-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.8 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-8-release-notes/).

{{% /alert %}}

## Aspose.Wordsのための.NET 24.1, 24.2, 24.3, 24.4

Aspose.Words24.1ストロークカラーの管理に関する経験が向上し、OLEオブジェクトとLINQレポートが強化され、新しい`Bibliography Sources`パブリックAPIが導入されました。

Aspose.Words24.2展開されたグラフAPI、スタイル管理、およびLINQオプション。 このバージョンのAspose.Wordsでは、レンダリング中にSvgSaveOptionsを指定する機能、Markdownファイルを読み込む柔軟な制御、脚注と文末脚注の参照テキストを操作する機能も導入されました。

Aspose.Words24.3は新しいTIFFリーダー/ライターを導入し、WMFメタファイルのバイナリラスタ演算のエミュレーションを導入しました。 Aspose.Words24.3もチャートAPIを拡大し続けます。

Aspose.Words24.4保存形式、いくつかのレンダリングオプションを強化し、デジタル署名の作業を改善します。

### サポートされている形式 <sup>24.4</sup>

最新の**WebP**画像形式がサポートされるようになりました Aspose.Wordsのための.NET Framework 4.6.2 そしてより高い。 WebP画像を読み込んで文書に挿入したり、WebP形式で画像を保存したりできるようになりました。

WebPは現在.NET Standardと.NET Frameworkv4.6.2以上でのみ利用可能です。

### レンダリングと印刷

#### ストロークカラーコントロール <sup>24.1</sup>

[Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/)クラスは、ストロークの色の管理に関連する一連の新しいパブリックプロパティ[ForeThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/forethemecolor/)と[BackThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backthemecolor/)、[ForeTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/foretintandshade/)と[BackTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backtintandshade/)で拡張されました。

#### DrawingMLチャートAPI拡張 <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API**は引き続き展開されます。

#### @font-faceルールで宣言された埋め込みフォント <sup>24.4</sup>

新しい[SupportFontFaceRules](https://reference.aspose.com/words/net/aspose.words.loading/htmlloadoptions/supportfontfacerules/)プロパティを追加することで、@font-faceルールで宣言されたフォントを結果のドキュメントのフォント定義に埋め込む機能が導入されました。

#### グローとリフレクションの書式設定を使用する <sup>24.4</sup>

描画オブジェクトのグローとリフレクションの書式設定を操作する機能が実装されました。

### 文書の読み込みと保存

#### レンダリング中にSvgSaveOptionsを指定します <sup>24.2</sup>

レンダリング中に[SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/)を指定する機能が[ShapeRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/shaperenderer/)を使用して追加されました。[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/)と[OfficeMathRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/officemathrenderer/)。[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/)メソッド。

#### Markdownファイルの読み込み時に空の行を保持する <sup>24.2</sup>

Markdownファイルの読み込み時に空行を保持する機能が追加されました。

#### 新しいTIFFリーダー/ライター <sup>24.3</sup>

.NET Standard、.NET6以降のAspose.Words用の新しいTIFFリーダ/ライタが開発されました。 Aspose.Wordsのための.NET 24.3 JPEGおよび古いJPEG圧縮タイプのTIFF画像の読み取りのサポートが追加され、読み取りおよび書き込み操作の品質も大幅に改善されました。

### その他

* `TextBox`OLEコントロールのテキストを変更する機能は、新しい[Text](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/text/)プロパティを新しい[TextBoxControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/)クラスに追加することによって導入されました。 <sup>24.1</sup>
* 参考文献ソースpublicAPIは、新しいクラスと列挙を含む新しい名前空間[Aspose.Words.Bibliography](https://reference.aspose.com/words/net/aspose.words.bibliography/)の追加と、新しい[Bibliography](https://reference.aspose.com/words/net/aspose.words/document/bibliography/)プロパティを[Document](https://reference.aspose.com/words/net/aspose.words/document/)クラスに追加することによって実装されました。 <sup>24.1</sup>
* `LINQ Reporting Engine`のテンプレート構文を使用して型メンバーへのアクセスを制限するAPIが提供されています。 <sup>24.1</sup>
* スタイル管理を強化するための新しいパブリックプロパティ[Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/)、[UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/)、[SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/)が[Style](https://reference.aspose.com/words/net/aspose.words/style/)クラスに追加されました。 <sup>24.2</sup>
* 脚注と文末脚注の実際の参照マークテキストを取得する機能は、[ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/)プロパティと[UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/)メソッドで強化されました。 <sup>24.2</sup>
* `LINQ Reporting Engine`の`Word 2016`チャートとの互換性が有効になりました。 <sup>24.2</sup>
* WMFメタファイルのバイナリラスタ演算のエミュレーションが実装されました。 <sup>24.3</sup>
* **SaveOptions**内の文書の署名オプションを定義する機能は、新しいパブリックメンバーを持つ新しい[DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/digitalsignaturedetails/)クラスを追加することと、[OoxmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/ooxmlsaveoptions/)、[DocSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/docsaveoptions/)、[OdtSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/odtsaveoptions/)クラスに新しいプロパテ <sup>24.4</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.1 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-1-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.2 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-2-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.3 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-3-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 24.4 リリースノート](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-4-release-notes/).

{{% /alert %}}

## Aspose.Wordsのための.NET 23.9, 23.10, 23.11, 23.12

Aspose.Words23.9レンダリングオプション、メタファイルレンダリングエミュレーション、およびmarkdown保存オプションを展開します。

Aspose.Words23.10レンダリングが改善され、文書の読み込みと保存のオプションが拡張され、ユーザーが新しい方法で文書をマージできるようになりました。Aspose.Words23.10

Aspose.Words23.11は、追加オプションを使用して、チャート凡例のリビジョン、XLSX形式、フォントを使用して作業を強化します。

Aspose.Words23.12は、PDFおよびOOXMLドキュメントを操作するための新しいプロパティと列挙、およびWebPイメージのサポートを導入します。

### レンダリングと印刷

#### DrawingMLチャートでの座標軸タイトルのカスタマイズ <sup>23.9</sup>

DrawingMLチャートの軸タイトルをカスタマイズする機能は、新しいパブリッククラス[ChartAxisTitle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxistitle/)および[Title](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxis/title/)プロパティの実装によって導入されました。

#### 段落内のフォントの垂直位置の決定 <sup>23.9</sup>

新しいpublic[BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/paragraphformat/baselinealignment/)プロパティと新しい[BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/baselinealignment/)列挙体を使用して、段落内のフォントの垂直位置を定義できるようになりました。

#### 前景色制御 <sup>23.10</sup>

修飾子なしで前景色を取得する機能が**BaseForeColor**プロパティを介して[Fill](https://reference.aspose.com/words/net/aspose.words.drawing/fill/)クラスと[Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/)クラスに追加されました。

#### チャートの機能を拡張する <sup>23.10</sup>

[ChartDataPointCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatapointcollection/)、[ChartSeries](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseries/)、[ChartFormat](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartformat/)クラスの機能は、新しいメソッドとプロパティで拡張されました。

#### 画像を自動的に調整して図形に合わせる <sup>23.10</sup>

新しい[FitImageToShape](https://reference.aspose.com/words/net/aspose.words.drawing/imagedata/fitimagetoshape/)メソッドを使用して、画像を特定の形状に自動的に調整して合わせる簡単な方法が提供されています。

#### DrawingMLグラフの凡例エントリの既定のフォント書式設定 <sup>23.11</sup>

DrawingMLチャートの凡例エントリのデフォルトのフォント書式を指定する機能が[Font](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartlegend/font/)プロパティを介して追加されました。 この機能により、グラフ要素のより合理化された一貫した外観が容易になり、文書全体の美しさが向上します。

#### ReaderでPDFを開くときのページレイアウトの指定 <sup>23.12</sup>

PDFリーダーで文書を開くときに使用するページレイアウトを指定する機能は、[PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)クラスに新しい[PageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/pagelayout/)プロパティを導入し、新しい[PdfPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfpagelayout/)列挙体を導入することによ

### 文書の読み込みと保存

#### イメージURIsをMarkdownに構築するフォルダ名の指定 <sup>23.9</sup>

[MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/)クラスは[ImagesFolderAlias](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imagesfolderalias/)プロパティを含めることで拡張され、Markdown文書に書き込まれたイメージURIsを構築するために使用されるフォルダの名前を指定できます。

#### PDF出力サイズを減らす <sup>23.10</sup>

[OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/)設定を使用するときに出力サイズを小さくするためのさまざまなPDFレンダリング最適化が実装されています。

#### TXT文書を読み込むときにハイパーリンクを認識する <sup>23.10</sup>

TXT文書の読み込み時にハイパーリンクを認識する機能は、新しい[DetectHyperlinks](https://reference.aspose.com/words/net/aspose.words.loading/txtloadoptions/detecthyperlinks/)プロパティを追加することによって実装されています。

### その他

* ラスタライズサイズを決定するためのメタファイルレンダリングエミュレーションが実装されました,特にWMFペン幅とEMF化粧ペン幅のために. これを実現するために、**ScaleWmfFontsToMetafileSize**プロパティは[EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpage/)プロパティに置き換えられ、[EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpageresolution/)プロパティが追加されました。 <sup>23.9</sup>
* 現在のカーソル位置にある文書を別の文書に挿入するための簡略化された方法が[InsertDocumentInline](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertdocumentinline/)メソッドを使用して導入されました。 <sup>23.10</sup>
* 新しい[Locked](https://reference.aspose.com/words/net/aspose.words/style/locked/)プロパティの導入により、スタイルプロパティにアクセスして変更する機能が追加されました。 <sup>23.10</sup>
* ジェネリック型パラメーターが[CompositeNode](https://reference.aspose.com/words/net/aspose.words/compositenode/)クラスのメソッドに追加されました。 <sup>23.10</sup>
* 特定のリビジョンを受け入れる/拒否するかどうかを制御する方法は、[Accept](https://reference.aspose.com/words/net/aspose.words/revisioncollection/accept/)メソッドと[Reject](https://reference.aspose.com/words/net/aspose.words/revisioncollection/reject/)メソッドを使用して実装されています。 この機能強化により、ユーザーは改訂プロセスをより細かく制御できます。 <sup>23.11</sup>
* ドキュメントのすべてのセクションを同じXLSXワークシートに書き込む機能は、新しい[XlsxSectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsectionmode/)列挙型と新しい[SectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsaveoptions/sectionmode/)プロパティによって提供されています。 <sup>23.11</sup>
* ZIP64書式拡張がOOXML文書にどのように使用されるかを制御する方法は、`OoxmlSaveOptions`クラスの新しいZip64Modeプロパティと新しいZip64Mode列挙体を介して実装されています。 <sup>23.12</sup>
* WebPイメージのサポートが導入されました。 この機能は以下のためにのみ利用可能ですのでご注意ください。NetStandartおよび.NET6+バージョン。 <sup>23.12</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 23.9 リリースノート](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-9-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 23.10 リリースノート](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-10-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 23.11 リリースノート](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-11-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 23.12 リリースノート](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-12-release-notes/).

{{% /alert %}}

## Aspose.Wordsのための.NET 23.5, 23.6, 23.7, 23.8

Aspose.Words23.5は、グラフ系列データを操作する機能とODTドキュメントを操作する機能を強化し、ヘッダー/フッターとそのテキストの折り返しを改善します。Aspose.Words23.5は、グラフ系列データを操作する機能とODTドキュメントを操作する機能を強化します。

Aspose.Words23.6レンダリングオプションを展開し、新しいエクスポート形式を追加し、LINQレポートとLowCodeツールを改善します。

Aspose.Words23.7レポート機能が強化され、新しいエクスポート形式が追加され、テーブルとデジタル署名の操作に変更が加えられました。

Aspose.Words23.8は、さまざまな形式の機能を拡張し、レンダリングを改善し、フィールドを操作するための新しいオプションを追加します。

### サポートされている形式

* バージョン23.6以降では、文書をXLSX形式で保存することができます。 今、あなたはExcel形式に文書を変換することができます。 <sup>23.6</sup>
* バージョン23.7以降では、文書ページまたは図形をEPS形式で保存することができます。 <sup>23.7</sup>

### 新しいフォーマット機能

* MOBI文書の目次(TOC)を自動的に生成する機能が導入されました。 <sup>23.8</sup>
* [PdfEncryptionDetails](https://reference.aspose.com/words/net/aspose.words.saving/pdfencryptiondetails/pdfencryptiondetails/)コンストラクタは[PdfPermissions](https://reference.aspose.com/words/net/aspose.words.saving/pdfpermissions/)で展開されています。 <sup>23.8</sup>
* EMFメタファイルの垂直テキストの整形が実装されました。 <sup>23.8</sup>

### レンダリングと印刷

#### グラフ系列データの取得と変更 <sup>23.5</sup>

グラフ系列データを取得および変更する機能は、以下を追加することによって提供されました:

* 新しいクラス: [ChartXValue](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartmultilevelvalue/)
* 新しい列挙型:[ChartXValueType](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluetype/),[ChartYValueType](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluetype/)

#### 高度なタイポグラフィのサポート <sup>23.6</sup>

WMF、EMF、EMF+レンダリングにおける高度なタイポグラフィのサポートが追加されました。

#### ページ上の色付きのコンテンツ <sup>23.6</sup>

ページが色付けされているかどうかを示すパブリックプロパティ[PageInfo.Colored](https://reference.aspose.com/words/net/aspose.words.rendering/pageinfo/colored/)が追加されました。

#### チャートデータラベルの書式設定 <sup>23.6</sup>

チャートデータラベルの塗りつぶし、ストローク、および吹き出しの書式設定を設定する機能が実装されました。

### Mail Mergeと報告

#### LINQレポートエンジンの動的HTML挿入 <sup>23.6</sup>

LINQReporting Engineの動的HTML挿入の新しい方法が追加されました。

#### Mustacheタグのサポート <sup>23.7</sup>

Mustacheタグは[MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/getregionshierarchy/)メソッドと[MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/getfieldnamesforregion/#getfieldnamesforregion)メソッドでサポートされるようになりました。

#### LINQレポートエンジンテンプレート構文の更新 <sup>23.7</sup>

LINQReporting Engineテンプレート構文で、`ElementAt`およびElementAtOrDefault拡張メソッドがサポートされるようになりました。

#### レンダリングされた画像のサイズの指定 <sup>23.8</sup>

レンダリングされた画像のサイズをピクセル単位で指定するための新しいパブリックプロパティ[ImageSize](https://reference.aspose.com/words/net/aspose.words.saving/imagesaveoptions/imagesize/)が導入されました。

#### JSON文字列値の空白を保持する-LINQ <sup>23.8</sup>

LINQレポートエンジンに、JSON文字列値の空白を保持するオプションが追加されました。

### LowCode <sup>23.6</sup>

異なる種類の文書を単一の出力文書にマージするための新しいLowCodeメソッドが追加されました。

### その他

* ヘッダー/フッターでのテキスト折り返しのサポートが実装されました。 <sup>23.5</sup>
* ODT文書からデジタル署名を削除する機能が[RemoveAllSignatures](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignatureutil/removeallsignatures/)メソッドによって追加されました。 <sup>23.5</sup>
* 音声ガイド[Run](https://reference.aspose.com/words/net/aspose.words/run/)のベーステキストとルビテキストを取得するためのパブリックプロパティ[PhoneticGuide](https://reference.aspose.com/words/net/aspose.words/run/phoneticguide/)が追加されました。 <sup>23.5</sup>
* 新しい[SignatureValue](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignature/signaturevalue/)プロパティを導入することで、デジタル署名された文書からデジタル署名値をバイト配列として取得する機能が追加されました。 <sup>23.7</sup>
* [Row](https://reference.aspose.com/words/net/aspose.words.tables/row/)クラスと[Cell](https://reference.aspose.com/words/net/aspose.words.tables/cell/)クラスは新しいパブリックメンバーで拡張されました– [Row.NextRow](https://reference.aspose.com/words/net/aspose.words.tables/row/nextrow/), [Row.PreviousRow](https://reference.aspose.com/words/net/aspose.words.tables/row/previousrow/), [Cell.NextCell](https://reference.aspose.com/words/net/aspose.words.tables/cell/nextcell/), と[Cell.PreviousCell](https://reference.aspose.com/words/net/aspose.words.tables/cell/previouscell/)。 <sup>23.7</sup>
* CITATIONフィールドとBIBLIOGRAPHYフィールドのサポートが追加されました。 <sup>23.8</sup>

{{% alert color="primary" %}}

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 23.5 リリースノート](/words/net/aspose-words-for-net-23-5-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 23.6 リリースノート](/words/net/aspose-words-for-net-23-6-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 23.7 リリースノート](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-7-release-notes/).

詳細については、こちらをご覧ください [Aspose.Wordsのための.NET 23.8 リリースノート](/words/net/aspose-words-for-net-23-8-release-notes/).

{{% /alert %}}

## また見て下さい

{{% alert color="primary" %}}

このページには、過去2年間の最新リリースニュースが含まれています。 以前のリリースの詳細については、以下を参照してください [リリースノート'](https://releases.aspose.com/words/net/release-notes/) 関連するセクションのページ。

{{% /alert %}}
