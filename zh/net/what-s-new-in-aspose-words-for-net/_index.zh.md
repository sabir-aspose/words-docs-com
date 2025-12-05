---
title: 最新消息
second_title: Aspose.Words为.NET
articleTitle: 最新消息 Aspose.Words为.NET
linktitle: 最新消息 Aspose.Words为.NET
type: docs
description: "Aspose.Words为.NET 每天扩展和增强。 在这个页面上，您可以了解该产品的巨大和最有趣的功能。"
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /zh/net/what-s-new-in-aspose-words-for-net/
timestamp: 2025-06-23-21-02-49
---

本页介绍了最近版本中引入的最有趣的Aspose.Words新特性。

## Aspose.Words为.NET 25.5, 25.6

Aspose.Words25.5通过新的样式选项增强了图表自定义，并通过提供对空段落处理方式的控制来改进Markdown导出。

Aspose.Words25.6通过引入高级图像导出选项、改进的MathML处理和更好的图表表示，增强了渲染精度和可视化功能。

### 转换、加载和保存文档

#### 将空段落导出为Markdown <sup>25.5</sup>

通过添加[MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownemptyparagraphexportmode/)枚举和[EmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/emptyparagraphexportmode/)属性，引入了控制如何将空段落导出到Markdown的能力。

#### 将多页文档导出为光栅图像格式 <sup>25.6</sup>

通过扩展图像导出功能，可以使用[customizable layouts](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/)（水平、垂直或网格）将多页文档导出为栅格图像格式（如PNG和JPEG）。

### 渲染图

#### 设置图表样式 <sup>25.5</sup>

通过添加[ChartStyle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartstyle/)枚举和[Style](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/style/)属性，引入了设置图表样式的功能。

#### 在MathML表达式中呈现连接器行 <sup>25.6</sup>

在MathML表达式中实现了连接器线的渲染，以确保更准确和视觉上一致地显示数学公式。

#### 瀑布图的渲染图例 <sup>25.6</sup>

引入了["Waterfall" charts](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriestype/)的图例渲染，提高了数据透明度并提高了这些图表的可解释性。

### 其他

* 增强了包装包含多个斜线的数学公式的能力，提高了布局清晰度和公式易读性。 <sup>25.6</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为.NET 25.5发行说明](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-5-release-notes/).

了解更多关于 [Aspose.Words为.NET 25.6发行说明](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words为.NET 25.1, 25.2, 25.3, 25.4

Aspose.Words25.1引入了AI支持的语法检查，并通过HTML、SVG和Markdown格式的高级选项增强了文档保存。

Aspose.Words25.2引入了带有AnthropicAI模型的文本摘要，增加了MsWorks格式支持，增强了排版控制，并改进了PDF结构和列表处理。

Aspose.Words25.3使用UpdateAmbiguousTextFont属性增强了AI支持的语法检查器和字体选择，并改进了PDF附件导出。

Aspose.Words25.4引入对新纸张尺寸的支持，启用高级HTML导出控制，改进水印处理，并增强LowCodeAPI的可用性。

### AI功能

#### 文档AI语法检查

* 通过添加一个新的[CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/)方法，引入了使用OpenAI生成模型检查所提供文档语法的能力。 <sup>25.1</sup>
* 更新了AI支持的语法检查功能，以支持[AiModelType](https://reference.aspose.com/words/net/aspose.words.ai/aimodeltype/)枚举中可用的所有模型。 <sup>25.3</sup>

#### 使用Anthropic生成语言模型进行总结 <sup>25.2</sup>

通过引入一个新的公共类[AnthropicAiModel](https://reference.aspose.com/words/net/aspose.words.ai/anthropicaimodel/)，启用了使用Anthropic生成语言模型的文本摘要。

### Low Code

#### Low CodeAPI可用性 <sup>25.4</sup>

对**LowCode API**的可用性进行了重大改进，简化了文档处理并减少了对重复代码的需求。

### 支持的格式 <sup>25.2</sup>

从版本25.2开始，添加了与MicrosoftWorks文档的新MsWorks加载格式的兼容性。

### 转换、加载和保存文档

#### 改进保存为HTML和SVG格式 <sup>25.1</sup>

通过向[HtmlFixedSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlfixedsaveoptions/)和[SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/)类添加**IdPrefix**和**RemoveJavaScriptFromLinks**属性，已增强了保存为HTML和SVG格式的功能。

#### 保存为Markdown时设置图像分辨率和OfficeMath输出模式 <sup>25.1</sup>

* 在[MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/)类中添加了一个新的[ImageResolution](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imageresolution/)选项来设置图像分辨率。
* 一个新的[OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/officemathexportmode/)选项和[MarkdownOfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownofficemathexportmode/)枚举已添加到[MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/)类中以设置OfficeMath输出模式。
* 通过向[SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage_2)方法添加新的重载，引入了从流中设置图像水印的功能。 <sup>25.4</sup>

### 渲染图

#### 改进的排版控制 <sup>25.2</sup>

已添加[NumberSpacing](https://reference.aspose.com/words/net/aspose.words/font/numberspacing/)属性以改进排版控制。

#### 控制模糊字符的字体选择 <sup>25.3</sup>

在[SaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/)类中添加了一个新的公共属性[UpdateAmbiguousTextFont](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/updateambiguoustextfont/)，以根据使用的字符代码控制字体选择。

#### 纸张尺寸选项 <sup>25.4</sup>

通过向[PaperSize](https://reference.aspose.com/words/net/aspose.words/papersize/)枚举添加新值，引入了使用JISB4和JISB5纸张大小的功能。

#### HTML输出控制 <sup>25.4</sup>

通过添加[RemoveJavaScriptFromLinks](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/removejavascriptfromlinks/)属性，可以在HTML导出期间从超链接URLs中删除JavaScript。

### 其他

* PDF逻辑结构得到了改进，支持TOA、BIBLIOGRAPHY和INDEX字段。 <sup>25.2</sup>
* 为了改进列表处理，引入了[AddSingleLevelList](https://reference.aspose.com/words/net/aspose.words.lists/listcollection/addsinglelevellist/)方法。 <sup>25.2</sup>
* 添加了一个新属性[AttachmentsEmbeddingMode](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/attachmentsembeddingmode/)来替换**EmbedAttachments**以改进PDF附件的导出。 此外，新值已添加到[PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/)枚举以支持PDF/A版本附件。 此外，附件现在支持加密。 <sup>25.3</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为.NET 25.1 发行通知书](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-1-release-notes/).

了解更多关于 [Aspose.Words为.NET 25.2 发行通知书](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-2-release-notes/).

了解更多关于 [Aspose.Words为.NET 25.3 发行通知书](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-3-release-notes/).

了解更多关于 [Aspose.Words为.NET 25.4 发行通知书](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words为.NET 24.9, 24.10, 24.11, 24.12

Aspose.Words24.9通过DocumentBuilder引入group shape插入和StructuredDocumentTag插入，使用渐变增强径向图表呈现，使用XAdES-EPES支持改进数字签名，添加Markdown下划线识别，并提供对脚注/尾注分隔符的访问。

Aspose.Words24.10引入了增强的ActiveX控件支持CommandButton创建，新的形状可见性控制，group shapes的能力，改进的Markdown表格导出，Pie和Doughnut图表的图表格式，更好的Big5编码处理，以及对过时的台湾字体的支持。

Aspose.Words24.11引入了AI支持的文档摘要，增强的呈现选项，改进了对文档属性的访问和ActiveX控制字幕。

Aspose.Words24.12引入了可自定义的数据标签放置，GoogleAI支持的文本翻译，增强的Mail Merge清理选项和新的LowCode处理类。

### AI功能

#### 使用OpenAI和Google进行文档摘要 <sup>24.11</sup>

通过添加[Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)命名空间及其公共成员，集成了对使用**OpenAI**和**Google**生成语言模型的文档摘要的支持。

#### 使用Google生成语言模型进行文本翻译 <sup>24.12</sup>

通过将[Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/)方法和[Language](https://reference.aspose.com/words/net/aspose.words.ai/language/)枚举添加到[Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)命名空间，在Aspose.Words中实现了使用Google生成语言模型翻译文本的功能。

### Low Code <sup>24.12</sup>

新的LowCode类，如[Comparer](https://reference.aspose.com/words/net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/net/aspose.words.lowcode/splitter/) 等。 已经引入，提供了一组方法，在文档处理的简单性和灵活性之间取得完美的平衡。

### 渲染和打印

#### 径向图表上的毕业 <sup>24.9</sup>

已经实现了在径向图表上绘制毕业图。

#### CommandButton ActiveX 控件<sup>24.10</sup>

通过添加新的公共方法[InsertForms2OleControl](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertforms2olecontrol/)和新的公共类[Forms2OleControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/)，引入了创建CommandButtonActiveX控件的功能。

#### 控制形状可见性 <sup>24.10</sup>

添加了一个新的公共属性[Hidden](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/hidden/)来控制形状的可见性。

#### Pie和Doughnut图表的变化 <sup>24.10</sup>

为Pie和Doughnut图表的格式添加了几个新的公共属性。

#### 控制PDF选择表单字段边框的呈现 <sup>24.11</sup>

通过添加新的公共选项[RenderChoiceFormFieldBorder](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/renderchoiceformfieldborder/)，实现了控制PDF选择表单字段边框呈现的新选项。

#### 获取和设置图表数据的格式代码 <sup>24.11</sup>

通过在[ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/)、[ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/)和[BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/)类中实现[FormatCode](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/formatcode/)属性，添加了获取和设置图表数据格式代码的功能。

#### 使用箱和标签渲染直方图图表 <sup>24.11</sup>

通过允许指定数量的容器和标签，直方图图表的呈现得到了改进。

#### 自定义数据标签的放置 <sup>24.12</sup>

通过向[ChartDataLabel](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabel/)和[ChartDataLabelCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/)类引入新属性，添加了自定义数据标签放置的功能。

### 转换、加载和保存文档

#### 加载Markdown文件时的下划线格式 <sup>24.9</sup>

加载Markdown文档时识别下划线格式的选项已通过添加新的公共属性[ImportUnderlineFormatting](https://reference.aspose.com/words/net/aspose.words.loading/markdownloadoptions/importunderlineformatting/)合并。

#### 保存到Markdown时，将表导出为HTML <sup>24.10</sup>

通过添加新的公共属性[ExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/exportashtml/)和枚举[MarkdownExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownexportashtml/)，实现了在将文档保存为Markdown格式时将表导出为HTML的选项。

#### 使用更新的逻辑结构导出PDF <sup>24.11</sup>

通过将表标题属性包含为PDF逻辑结构元素标题，已增强了PDF导出。

### Mail Merge和报告

#### 在Mail Merge期间删除空表 <sup>24.12</sup>

一个新的**RemoveEmptyTables**选项已添加到[MailMergeCleanupOptions](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmergecleanupoptions/)枚举以细化Mail Merge输出。

### 数码签署

#### 用XAdES-EPES签署文件 <sup>24.9</sup>

通过添加新的公共属性[XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/signoptions/xmldsiglevel/)和新的公共枚举[XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/xmldsiglevel/)，可以使用XAdES-EPES级别XML-DSig签名对文档进行签名。

### 其他

* 一个新的公共方法[InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/)已添加到group shapes。 <sup>24.9</sup>
* 添加了一个新的公共方法[InsertStructuredDocumentTag](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertstructureddocumenttag/)以将**StructuredDocumentTags**插入到文档中。 <sup>24.9</sup>
* 通过添加一些公共类和属性，提供了对脚注/尾注分隔符的公共访问。 <sup>24.9</sup>
* 通过添加[InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/#insertgroupshape_1)方法，引入了将单个形状（group shapes组合在一起，以及直接将形状和group shapes组合在一起的功能。 <sup>24.10</sup>
* 改进了TrueTypecmap表的Big5编码处理。 <sup>24.10</sup>
* 增强了对过时的台湾字体的支持。 <sup>24.10</sup>
* 要访问扩展文档属性，已将只读属性添加到[BuiltInDocumentProperties](https://reference.aspose.com/words/net/aspose.words.properties/builtindocumentproperties/)类。 <sup>24.11</sup>
* 通过向[Forms2OleControl.Caption](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/caption/)属性添加一个新的公共setter，已启用ActiveX控件的标题设置。 <sup>24.11</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为.NET 24.9 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-9-release-notes/).

了解更多关于 [Aspose.Words为.NET 24.10 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-10-release-notes/).

了解更多关于 [Aspose.Words为.NET 24.11 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-11-release-notes/).

了解更多关于 [Aspose.Words为.NET 24.12 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words为.NET 24.5, 24.6, 24.7, 24.8

Aspose.Words24.5扩展了程序集的选项，改进了呈现功能，并扩展了一些其他选项。

Aspose.Words24.6改进了渲染选项，增强了搜索和比较功能，并扩展了其他几个功能。

Aspose.Words24.7更改ActiveX的工作方式，扩展渲染功能，以及导出为Markdown和XLSX格式。

Aspose.Words24.8通过对轴标签的精确控制来增强图表自定义，扩展字体管理，改进文档结构处理，并为HTML/XAML导出、PDF功能、文档转换和数字签名添加新功能。

### 支持的格式

从版本24.7开始，支持导出到PDF/UA-2，以确保残疾用户的可访问性。

### 平台 <sup>24.5</sup>

.NET 7.0/8.0程序集已包含在Aspose.WordsNuGet包中。

### 渲染和打印

#### 图表、形状和DrawingML的变化 <sup>24.5</sup>

* 已经实现了SVG图形的DrawingML效果渲染，扩展了以前仅限于图像的功能。
* 通过添加[ChartSeriesGroup](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroup/)和[ChartSeriesGroupCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroupcollection/)类以及[SeriesGroups](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/seriesgroups/)属性，支持在序列组中创建组合图和调整间隙宽度、重叠和气泡比例等属性。
* 通过添加[SoftEdgeFormat](https://reference.aspose.com/words/net/aspose.words.drawing/softedgeformat/)类实现了操作形状SoftEdge效果的功能。
* 通过添加[AdjustmentCollection](https://reference.aspose.com/words/net/aspose.words.drawing/adjustmentcollection/)和[Adjustment](https://reference.aspose.com/words/net/aspose.words.drawing/adjustment/)公共类以及[Adjustments](https://reference.aspose.com/words/net/aspose.words.drawing/shape/adjustments/)属性，实现了修改形状调整值的功能。

#### 图表、形状和绘图的变化 <sup>24.6</sup>

* 制图能力得到了增强。 您现在可以创建更多种类的图表，包括*Treemaps*, *Sunbursts*, *Histograms*, *Pareto* 图表，*Box & Whisker*图表，*Waterfalls*和*Funnels*。 这使您能够以更加多样化和信息丰富的方式可视化数据。
* 阴影格式的颜色控制已得到改进。 通过访问阴影颜色，您可以更精确地控制文档的外观。
* 改进了后台渲染的性能提升。 借助原生平铺技术，您可以显着加快包含小元素的背景的渲染速度。
* 已添加形状的逼真渐变。 您现在可以创建具有非线性渐变的DML形状，模仿Microsoft Word的视觉样式以获得更抛光的外观。

#### 图表数据标签定制 <sup>24.7</sup>

添加了自定义图表数据标签（如**Orientation**和**Rotation**）的功能。

#### 列表级别的自定义数字样式 <sup>24.7</sup>

已添加公共属性[CustomNumberStyleFormat](https://reference.aspose.com/words/net/aspose.words.lists/listlevel/customnumberstyleformat/)的setter。 您现在可以为列表级别定义自定义数字样式。

#### 使用ActiveX的更改 <sup>24.7</sup>

* 现在可以修改ActiveX对象的属性，使您可以更好地控制其行为。
* 添加了修改单选按钮ActiveX控件的值以启用动态交互的功能。
* 添加了将ActiveXcheckbox切换为"已选中"或"未选中"的功能。

#### 控制图表轴刻度标签的方向和旋转 <sup>24.8</sup>

添加了对图表轴刻度标签的方向和旋转的精确控制，以便于更方便的图表定制-[AxisTickLabels](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/)类已扩展为新的[Orientation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/orientation/)和[Rotation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/rotation/)属性。

#### 用日元符号替换反斜杠 <sup>24.8</sup>

改进了向后兼容的HTML和XAML导出，用于用日元符号替换反斜杠字符。 为此，**ReplaceBackslashWithYenSign**属性已添加到[HtmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/)和[XamlFlowSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xamlflowsaveoptions/)类中。

#### 导出到PDF时使用SDT标记作为表单字段名称 <sup>24.8</sup>

通过向[PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)类添加新的[UseSdtTagAsFormFieldName](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/usesdttagasformfieldname/)属性，增强了支持使用SDT标记作为表单字段名称的PDF导出。

### 转换、加载和保存文档

#### 将链接导出为Markdown格式 <sup>24.7</sup>

通过实现[LinkExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/linkexportmode/)属性，添加了控制Markdown格式链接导出的功能。

#### LowCode 24.8 <sup>24.8</sup>

引入了一个新的[LowCode.Converter](https://reference.aspose.com/words/net/aspose.words.lowcode/converter/)类，旨在提供一组用一行代码转换各种文档类型的方法。

### 搜索和比较

#### 高级比较选项 <sup>24.6</sup>
增加了通过改进的比较功能简化数据分析工作流的能力。 这包括一个新的[IgnoreStoreItemId](https://reference.aspose.com/words/net/aspose.words.comparing/advancedcompareoptions/ignorestoreitemid/)选项和一个重新设计的高级比较界面。

### 其他

* 通过添加[RemoveBlankPages](https://reference.aspose.com/words/net/aspose.words/document/removeblankpages/)方法实现了从文档中消除空页的功能。 <sup>24.5</sup>
* 通过添加[HasMacros](https://reference.aspose.com/words/net/aspose.words/fileformatinfo/hasmacros/)属性，可以在不加载文档的情况下检查VBA宏是否存在。 <sup>24.5</sup>
* 现在支持在使用LINQ报告引擎插入文档时保持源编号。 <sup>24.5</sup>
* 添加了一个新的[DateTimeUtc](https://reference.aspose.com/words/net/aspose.words/comment/datetimeutc/)属性-这为注释提供了更精确的时间戳，改善了组织和可追溯性。 <sup>24.6</sup>
* LINQ报告引擎已得到改进。 已经对空段落进行了选择性删除，并为缺少的对象成员定义了自定义消息，从而产生了更清洁和更具信息性的报告。 <sup>24.6</sup>
* 现在会自动检测datetime格式，以便无缝导出为XLSX格式。 <sup>24.7</sup>
* 已添加公共属性[IsProtected](https://reference.aspose.com/words/net/aspose.words.vba/vbaproject/isprotected/)，它允许您验证VBA项目是否受保护。 <sup>24.7</sup>
* 字体信息已扩展，**EmbeddingLicensingRights**属性添加到[FontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/fontinfo/)和[PhysicalFontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/physicalfontinfo/)类。 <sup>24.8</sup>
* 添加了一种在保留水印的同时有效清除部分页眉和页脚的方法，以更准确地使用文档结构。 要清除节页眉和页脚，请使用新的公共方法[ClearHeadersFooters](https://reference.aspose.com/words/net/aspose.words/section/clearheadersfooters/)。 <sup>24.8</sup>
* 已启用使用[XpsSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/)对XPS文档进行数字签名–为此添加了一个新属性[DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/digitalsignaturedetails/)。 <sup>24.8</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为.NET 24.5 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-5-release-notes/).

了解更多关于 [Aspose.Words为.NET 24.6 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-6-release-notes/).

了解更多关于 [Aspose.Words为.NET 24.7 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-7-release-notes/).

了解更多关于 [Aspose.Words为.NET 24.8 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words为.NET 24.1, 24.2, 24.3, 24.4

Aspose.Words24.1改进了管理笔划颜色的体验，增强了OLE对象和LINQ报告，并引入了新的`Bibliography Sources`publicAPI。

Aspose.Words24.2展开图表API、样式管理和LINQ选项。 此版本的Aspose.Words还引入了在渲染期间指定SvgSaveOptions的功能，更灵活地控制加载Markdown文件，以及处理脚注和尾注的参考文本。

Aspose.Words24.3为WMF元文件引入了一个新的TIFF读取器/写入器和二进制栅格操作的仿真。 Aspose.Words24.3也继续扩展图表API。

Aspose.Words24.4增强了保存格式，一些渲染选项，以及改进了数字签名的工作。

### 支持的格式 <sup>24.4</sup>

现代**WebP**图像格式现在在 Aspose.Words为.NET Framework 4.6.2 而且更高。 您现在可以读取WebP图像并将其插入到文档中，以及以WebP格式保存图像。

请注意，WebP目前仅在.NET Standard和.NET Frameworkv4.6.2及以上版本中提供。

### 渲染和打印

#### 笔画颜色控制 <sup>24.1</sup>

[Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/)类已扩展为一组与管理笔划颜色相关的新公共属性：[ForeThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/forethemecolor/)和[BackThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backthemecolor/)，[ForeTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/foretintandshade/)和[BackTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backtintandshade/)。

#### DrawingML图表API扩展 <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API**继续扩展。

#### 嵌入在@font-face规则中声明的字体 <sup>24.4</sup>

添加了将在@font-face规则中声明的字体嵌入到结果文档的字体定义中的功能，通过添加新的[SupportFontFaceRules](https://reference.aspose.com/words/net/aspose.words.loading/htmlloadoptions/supportfontfacerules/)属性引入。

#### 使用发光和反射格式 <sup>24.4</sup>

已经实现了使用绘图对象的发光和反射格式的能力。

### 加载和保存文档

#### 在渲染期间指定SvgSaveOptions <sup>24.2</sup>

使用[ShapeRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/shaperenderer/)添加了在渲染期间指定[SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/)的功能。[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/)和[OfficeMathRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/officemathrenderer/)。[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/)方法。

#### 加载Markdown文件时保留空行 <sup>24.2</sup>

添加了加载Markdown文件时保留空行的功能。

#### 一个新的TIFF读者/作家 <sup>24.3</sup>

一个新的TIFF读者/作家为Aspose.Words为.NET Standard，.NET6及以后已经开发。 Aspose.Words为.NET 24.3 增加了对使用JPEG和旧的JPEG压缩类型读取TIFF图像的支持，并且还显着提高了读写操作的质量。

### 其他

* 通过向新的[TextBoxControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/)类添加新的[Text](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/text/)属性，引入了修改`TextBox`OLE控件文本的功能。 <sup>24.1</sup>
* 参考书目源publicAPI是通过添加新的命名空间[Aspose.Words.Bibliography](https://reference.aspose.com/words/net/aspose.words.bibliography/)及其新的类和枚举以及向[Document](https://reference.aspose.com/words/net/aspose.words/document/)类添加新的[Bibliography](https://reference.aspose.com/words/net/aspose.words/document/bibliography/)属性来实现的。 <sup>24.1</sup>
* 提供了使用`LINQ Reporting Engine`的模板语法限制对类型成员的访问的API。 <sup>24.1</sup>
* 已将用于增强样式管理的新公共属性[Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/)、[UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/)和[SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/)添加到[Style](https://reference.aspose.com/words/net/aspose.words/style/)类中。 <sup>24.2</sup>
* 使用[ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/)属性和[UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/)方法增强了检索脚注和尾注的实际参考标记文本的功能。 <sup>24.2</sup>
* 已启用与`LINQ Reporting Engine`的`Word 2016`图表的兼容性。 <sup>24.2</sup>
* 已经实现了对WMF元文件的二进制栅格操作的仿真。 <sup>24.3</sup>
* 通过添加具有新公共成员的新[DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/digitalsignaturedetails/)类以及向[OoxmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/ooxmlsaveoptions/)、[DocSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/docsaveoptions/)和[OdtSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/odtsaveoptions/)类添加新属性，启用了为**SaveOptions**内文档定义签名选项的功能。 <sup>24.4</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为.NET 24.1 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-1-release-notes/).

了解更多关于 [Aspose.Words为.NET 24.2 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-2-release-notes/).

了解更多关于 [Aspose.Words为.NET 24.3 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-3-release-notes/).

了解更多关于 [Aspose.Words为.NET 24.4 发行通知书](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words为.NET 23.9, 23.10, 23.11, 23.12

Aspose.Words23.9扩展渲染选项、图元文件渲染仿真和markdown保存选项。

Aspose.Words23.10改进了渲染，扩展了加载和保存文档的选项，并允许用户以新的方式合并文档。

Aspose.Words23.11通过其他选项增强了图表图例上的修订、XLSX格式和字体的工作。

Aspose.Words23.12引入了用于处理PDF和OOXML文档的新属性和枚举，以及对WebP图像的支持。

### 渲染和打印

#### 在DrawingML图表中自定义轴标题 <sup>23.9</sup>

通过实现新的公共类[ChartAxisTitle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxistitle/)和[Title](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxis/title/)属性，引入了在DrawingML图表中自定义轴标题的功能。

#### 确定字体在段落中的垂直位置 <sup>23.9</sup>

现在可以使用新的public[BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/paragraphformat/baselinealignment/)属性和新的[BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/baselinealignment/)枚举来定义段落中字体的垂直位置。

#### 前景色控制 <sup>23.10</sup>

通过**BaseForeColor**属性，在[Fill](https://reference.aspose.com/words/net/aspose.words.drawing/fill/)和[Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/)类中添加了不使用修饰符检索前景色的功能。

#### 扩展图表的功能 <sup>23.10</sup>

使用新的方法和属性扩展了[ChartDataPointCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatapointcollection/)、[ChartSeries](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseries/)和[ChartFormat](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartformat/)类的功能。

#### 自动调整图像并使其适合形状 <sup>23.10</sup>

通过新的[FitImageToShape](https://reference.aspose.com/words/net/aspose.words.drawing/imagedata/fitimagetoshape/)方法提供了一种在特定形状内自动调整和拟合图像的简单方法。

#### DrawingML图表图例条目的默认字体格式 <sup>23.11</sup>

通过[Font](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartlegend/font/)属性添加了为DrawingML图表的图例条目指定默认字体格式的功能。 此功能有助于为图表元素提供更精简和一致的外观，从而提高整体文档美观度。

#### 在Reader中打开PDF时指定页面布局 <sup>23.12</sup>

通过向[PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)类引入新的[PageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/pagelayout/)属性和引入新的[PdfPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfpagelayout/)枚举，添加了在PDF阅读器中打开文档时指定要使用的页面布局的功能。

### 加载和保存文档

#### 在Markdown中指定要构造ImageURIs的文件夹名称 <sup>23.9</sup>

通过包含[ImagesFolderAlias](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imagesfolderalias/)属性扩展了[MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/)类，该属性允许指定用于构造写入Markdown文档中的图像URIs的文件夹的名称。

#### 减小PDF输出大小 <sup>23.10</sup>

已经实现了各种PDF渲染优化，以减少使用[OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/)设置时的输出大小。

#### 加载TXT文档时识别超链接 <sup>23.10</sup>

加载TXT文档时识别超链接的功能已通过添加新的[DetectHyperlinks](https://reference.aspose.com/words/net/aspose.words.loading/txtloadoptions/detecthyperlinks/)属性来实现。

### 其他

* 已经实现了用于确定光栅化大小的图元文件渲染仿真，专门针对WMF笔宽和EMF笔宽。 为此，将**ScaleWmfFontsToMetafileSize**属性替换为[EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpage/)属性，并添加[EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpageresolution/)属性。 <sup>23.9</sup>
* 使用[InsertDocumentInline](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertdocumentinline/)方法引入了将一个文档插入当前光标位置的另一个文档的简化方法。 <sup>23.10</sup>
* 通过引入新的[Locked](https://reference.aspose.com/words/net/aspose.words/style/locked/)属性，添加了访问和修改样式属性的功能。 <sup>23.10</sup>
* 泛型类型参数已添加到[CompositeNode](https://reference.aspose.com/words/net/aspose.words/compositenode/)类的方法中。 <sup>23.10</sup>
* 通过使用[Accept](https://reference.aspose.com/words/net/aspose.words/revisioncollection/accept/)和[Reject](https://reference.aspose.com/words/net/aspose.words/revisioncollection/reject/)方法实现了一种控制何时应该接受/拒绝某个修订的方法。 此增强功能允许用户更好地控制修订过程。 <sup>23.11</sup>
* 通过新的[XlsxSectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsectionmode/)枚举类型和新的[SectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsaveoptions/sectionmode/)属性提供了将文档的所有部分写入同一个XLSX工作表的能力。 <sup>23.11</sup>
* 通过`OoxmlSaveOptions`类的新Zip64Mode属性和新的Zip64Mode枚举实现了一种控制ZIP64格式扩展如何用于OOXML文档的方法。 <sup>23.12</sup>
* 已经引入了对WebP图像的支持。 请注意，此功能仅适用于。NetStandart和.NET6+版本。 <sup>23.12</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为.NET 23.9 发行通知书](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-9-release-notes/).

了解更多关于 [Aspose.Words为.NET 23.10 发行通知书](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-10-release-notes/).

了解更多关于 [Aspose.Words为.NET 23.11 发行通知书](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-11-release-notes/).

了解更多关于 [Aspose.Words为.NET 23.12 发行通知书](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-12-release-notes/).

{{% /alert %}}

## 请参阅

{{% alert color="primary" %}}

本页包含过去2年的最新发布消息。 有关早期版本的详细信息，请参阅 [发行通知书'](https://releases.aspose.com/words/net/release-notes/) 相关部分中的页面。

{{% /alert %}}
