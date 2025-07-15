---
title: 最新消息
second_title: Aspose.Words为Python via .NET
articleTitle: 最新消息 Aspose.Words为Python via .NET
linktitle: 最新消息 Aspose.Words为Python via .NET
type: docs
description: "Aspose.Words为Python via .NET 每天扩展和增强。 在这个页面上，您可以了解该产品的巨大和最有趣的功能。"
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /zh/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-06-23-21-02-49
---

本页介绍了最近版本中引入的最有趣的Aspose.Words新特性。

## Aspose.Words为Python via .NET25.5,25.6

Aspose.Words25.5通过新的样式选项增强了图表自定义，并通过提供对空段落处理方式的控制来改进Markdown导出。

Aspose.Words25.6通过引入高级图像导出选项、改进的MathML处理和更好的图表表示，增强了渲染精度和可视化功能。

### 转换、加载和保存文档

#### 将空段落导出为Markdown <sup>25.5</sup>

通过添加**MarkdownEmptyParagraphExportMode**枚举和**empty_paragraph_export_mode**属性，引入了控制如何将空段落导出到Markdown的能力。

#### 将多页文档导出为光栅图像格式 <sup>25.6</sup>

通过扩展图像导出功能，可以使用[customizable layouts](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/)（水平、垂直或网格）将多页文档导出为栅格图像格式（如PNG和JPEG）。

### 渲染图

#### 设置图表样式 <sup>25.5</sup>

通过添加**ChartStyle**枚举和**style**属性，引入了设置图表样式的功能。

#### 在MathML表达式中呈现连接器行 <sup>25.6</sup>

在MathML表达式中实现了连接器线的渲染，以确保更准确和视觉上一致地显示数学公式。

#### 瀑布图的渲染图例 <sup>25.6</sup>

引入了["Waterfall" charts](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriestype/)的图例渲染，提高了数据透明度并提高了这些图表的可解释性。

### 其他

* 增强了包装包含多个斜线的数学公式的能力，提高了布局清晰度和公式易读性。 <sup>25.6</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为Python via .NET25.5发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-5-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET25.6发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words对于Python通过.NET 25.1, 25.2, 25.3, 25.4

Aspose.Words25.1引入了AI支持的语法检查，并通过HTML、SVG和Markdown格式的高级选项增强了文档保存。

Aspose.Words25.2引入了带有AnthropicAI模型的文本摘要，增加了MsWorks格式支持，增强了排版控制，并改进了PDF结构和列表处理。

Aspose.Words25.3使用UpdateAmbiguousTextFont属性增强了AI支持的语法检查器和字体选择，并改进了PDF附件导出。

Aspose.Words25.4引入对新纸张尺寸的支持，启用高级HTML导出控制，并改进水印处理。

### AI功能

#### 文档AI语法检查

* 通过添加一个新的[check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/)方法，引入了使用OpenAI生成模型检查所提供文档语法的能力。 <sup>25.1</sup>
* 更新了AI支持的语法检查功能，以支持[AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/)枚举中可用的所有模型。 <sup>25.3</sup>

#### 使用Anthropic生成语言模型进行总结 <sup>25.2</sup>

通过引入一个新的公共类[AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/)，启用了使用Anthropic生成语言模型的文本摘要。

### 支持的格式 <sup>25.2</sup>

从版本25.2开始，添加了与MicrosoftWorks文档的新MsWorks加载格式的兼容性。

### 转换、加载和保存文档

#### 改进保存为HTML和SVG格式 <sup>25.1</sup>

通过向[HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/)和[SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/)类添加**id_prefix**和**remove_java_script_from_links**属性，已增强了保存为HTML和SVG格式的功能。

#### 保存为Markdown时设置图像分辨率和OfficeMath输出模式 <sup>25.1</sup>

* 在[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)类中添加了一个新的[image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/)选项来设置图像分辨率。
* 一个新的[office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/)选项和[MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/)枚举已添加到[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)类中以设置OfficeMath输出模式。

### 渲染图

#### 改进的排版控制 <sup>25.2</sup>

已添加[number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/)属性以改进排版控制。

#### 控制模糊字符的字体选择 <sup>25.3</sup>

在[SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/)类中添加了一个新的公共属性[update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/)，以根据使用的字符代码控制字体选择。

#### 纸张尺寸选项 <sup>25.4</sup>

通过向[PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/)枚举添加新值，引入了使用JISB4和JISB5纸张大小的功能。

#### HTML输出控制 <sup>25.4</sup>

通过添加[RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/)属性，可以在HTML导出期间从超链接URLs中删除JavaScript。

### 其他

* PDF逻辑结构得到了改进，支持TOA、BIBLIOGRAPHY和INDEX字段。 <sup>25.2</sup>
* 为了改进列表处理，引入了[add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate)方法。 <sup>25.2</sup>
* 添加了一个新属性[attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/)来替换**EmbedAttachments**以改进PDF附件的导出。 此外，新值已添加到[PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/)枚举以支持PDF/A版本附件。 此外，附件现在支持加密。 <sup>25.3</sup>
* 通过向[SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions)方法添加新的重载，引入了从流中设置图像水印的功能。 <sup>25.4</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为Python via .NET 25.1发行说明](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 25.2发行说明](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 25.3发行说明](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 25.4发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words对于Python通过.NET 24.9, 24.10, 24.11, 24.12

Aspose.Words24.9通过DocumentBuilder引入group shape插入和StructuredDocumentTag插入，使用渐变增强径向图表呈现，使用XAdES-EPES支持改进数字签名，添加Markdown下划线识别，并提供对脚注/尾注分隔符的访问。

Aspose.Words24.10引入了增强的ActiveX控件支持CommandButton创建，新的形状可见性控制，group shapes的能力，改进的Markdown表格导出，Pie和Doughnut图表的图表格式，更好的Big5编码处理，以及对过时的台湾字体的支持。

Aspose.Words24.11引入了AI支持的文档摘要，增强的呈现选项，改进了对文档属性的访问和ActiveX控制字幕。

Aspose.Words24.12引入了可自定义的数据标签放置，GoogleAI支持的文本翻译和增强的新LowCode处理类。

### AI功能

#### 使用OpenAI和Google进行文档摘要 <sup>24.11</sup>

通过添加[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)命名空间及其公共成员，集成了对使用**OpenAI**和**Google**生成语言模型的文档摘要的支持。

#### 使用Google生成语言模型进行文本翻译 <sup>24.12</sup>

通过将[translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/)方法和[Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/)枚举添加到[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)命名空间，在Aspose.Words中实现了使用Google生成语言模型翻译文本的功能。

### Low Code <sup>24.12</sup>

新的LowCode类，如[Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) 等。 已经引入，提供了一组方法，在文档处理的简单性和灵活性之间取得完美的平衡。

### 渲染和打印

#### 径向图表上的毕业 <sup>24.9</sup>

已经实现了在径向图表上绘制毕业图。

#### CommandButton ActiveX 控件<sup>24.10</sup>

通过添加新的公共方法[insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/)和新的公共类[Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/)，引入了创建CommandButtonActiveX控件的功能。

#### 控制形状可见性 <sup>24.10</sup>

添加了一个新的公共属性[hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/)来控制形状的可见性。

#### Pie和Doughnut图表的变化 <sup>24.10</sup>

为Pie和Doughnut图表的格式添加了几个新的公共属性。

#### 控制PDF选择表单字段边框的呈现 <sup>24.11</sup>

通过添加新的公共选项[render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/)，实现了控制PDF选择表单字段边框呈现的新选项。

#### 获取和设置图表数据的格式代码 <sup>24.11</sup>

通过在[ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/)、[ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/)和[BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/)类中实现[format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/)属性，添加了获取和设置图表数据格式代码的功能。

#### 使用箱和标签渲染直方图图表 <sup>24.11</sup>

通过允许指定数量的容器和标签，直方图图表的呈现得到了改进。

#### 自定义数据标签的放置 <sup>24.12</sup>

通过向th[ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/)和[ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/)类引入新属性，添加了自定义数据标签放置的功能。

### 转换、加载和保存文档

#### 加载Markdown文件时的下划线格式 <sup>24.9</sup>

加载Markdown文档时识别下划线格式的选项已通过添加新的公共属性[import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/)合并。

#### 保存到Markdown时，将表导出为HTML <sup>24.10</sup>

通过添加新的公共属性[export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/)和枚举[MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/)，实现了在将文档保存为Markdown格式时将表导出为HTML的选项。

#### 使用更新的逻辑结构导出PDF <sup>24.11</sup>

通过将表标题属性包含为PDF逻辑结构元素标题，已增强了PDF导出。

### 数码签署

#### 用XAdES-EPES签署文件 <sup>24.9</sup>

通过添加新的公共属性[xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/)和新的公共枚举[XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/)，可以使用XAdES-EPES级别XML-DSig签名对文档进行签名。

### 其他

* 一个新的公共方法[insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/)已添加到group shapes。 <sup>24.9</sup>
* 添加了一个新的公共方法[insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/)以将**StructuredDocumentTags**插入到文档中。 <sup>24.9</sup>
* 通过添加一些公共类和属性，提供了对脚注/尾注分隔符的公共访问。 <sup>24.9</sup>
* 通过添加[insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist)方法，引入了将单个形状（group shapes组合在一起，以及直接将形状和group shapes组合在一起的功能。 <sup>24.10</sup>
* 改进了TrueTypecmap表的Big5编码处理。 <sup>24.10</sup>
* 增强了对过时的台湾字体的支持。 <sup>24.10</sup>
* 要访问扩展文档属性，已将只读属性添加到[BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/)类。 <sup>24.11</sup>
* 通过向[Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/)属性添加一个新的公共setter，已启用ActiveX控件的标题设置。 <sup>24.11</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为Python via .NET 24.9发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 24.10发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 24.11发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 24.12发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words对于Python通过.NET 24.5, 24.6, 24.7, 24.8

Aspose.Words24.5扩展了程序集的选项，改进了呈现功能，并扩展了一些其他选项。

Aspose.Words24.6改进了渲染选项，增强了搜索和比较功能，并扩展了其他几个功能。

Aspose.Words24.7更改ActiveX的工作方式，扩展渲染功能，以及导出为Markdown和XLSX格式。

Aspose.Words24.8通过对轴标签的精确控制来增强图表自定义，扩展字体管理，改进文档结构处理，并为HTML/XAML导出、PDF功能、文档转换和数字签名添加新功能。

### 支持的格式

从版本24.7开始，支持导出到PDF/UA-2，以确保残疾用户的可访问性。

### 渲染和打印

#### 图表、形状和DrawingML的变化 <sup>24.5</sup>

* 已经实现了SVG图形的DrawingML效果渲染，扩展了以前仅限于图像的功能。
* 通过添加[ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/)和[ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/)类以及[series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/)属性，支持在序列组中创建组合图和调整间隙宽度、重叠和气泡比例等属性。
* 通过添加[SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/)类实现了操作形状SoftEdge效果的功能。
* 通过添加**AdjustmentCollection**和**Adjustment**公共类以及[adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/)属性，实现了修改形状调整值的功能。

#### 图表、形状和绘图的变化 <sup>24.6</sup>

- 制图能力得到了增强。 您现在可以创建更多种类的图表，包括*Treemaps*, *Sunbursts*, *Histograms*, *Pareto* 图表，*Box & Whisker*图表，*Waterfalls*和*Funnels*。 这使您能够以更加多样化和信息丰富的方式可视化数据。
- 阴影格式的颜色控制已得到改进。 通过访问阴影颜色，您可以更精确地控制文档的外观。
- 改进了后台渲染的性能提升。 借助原生平铺技术，您可以显着加快包含小元素的背景的渲染速度。
- 添加了形状的逼真渐变。 您现在可以创建具有非线性渐变的DML形状，模仿Microsoft Word的视觉样式以获得更抛光的外观。

#### 图表数据标签定制 <sup>24.7</sup>

添加了自定义图表数据标签（如**Orientation**和**Rotation**）的功能。

#### 列表级别的自定义数字样式 <sup>24.7</sup>

已添加公共属性[custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/)的setter。 您现在可以为列表级别定义自定义数字样式。

#### 使用ActiveX的更改 <sup>24.7</sup>

- 现在可以修改ActiveX对象的属性，使您可以更好地控制其行为。
- 添加了修改单选按钮ActiveX控件的值以启用动态交互的功能。
- 添加了将ActiveXcheckbox切换为"已选中"或"未选中"的功能。

#### 控制图表轴刻度标签的方向和旋转 <sup>24.8</sup>

添加了对图表轴刻度标签的方向和旋转的精确控制，以便于更方便的图表定制-[AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/)类已扩展为新的[orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/)和[rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/)属性。

#### 用日元符号替换反斜杠 <sup>24.8</sup>

改进了向后兼容的HTML和XAML导出，用于用日元符号替换反斜杠字符。 为此，**replace_backslash_with_yen_sign**属性已添加到[HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/)和[XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/)类中。

#### 导出到PDF时使用SDT标记作为表单字段名称 <sup>24.8</sup>

通过向[PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/)类添加新的[use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/)属性，增强了支持使用SDT标记作为表单字段名称的PDF导出。

### 转换、加载和保存文档

#### 将链接导出为Markdown格式 <sup>24.7</sup>

通过实现[link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/)属性，添加了控制Markdown格式链接导出的功能。

#### LowCode 24.8 <sup>24.8</sup>

引入了一个新的[LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/)类，旨在提供一组用一行代码转换各种文档类型的方法。

### 搜索和比较

#### 高级比较选项 <sup>24.6</sup>

增加了通过改进的比较功能简化数据分析工作流的能力。 这包括一个新的[ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/)选项和一个重新设计的高级比较界面。

### 其他

* 通过添加[remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/)方法实现了从文档中消除空页的功能。 <sup>24.5</sup>
* 通过添加[has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/)属性，可以在不加载文档的情况下检查VBA宏是否存在。 <sup>24.5</sup>
* 现在支持在使用LINQ报告引擎插入文档时保持源编号。 <sup>24.5</sup>
* 添加了一个新的[date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/)属性-这为注释提供了更精确的时间戳，改善了组织和可追溯性。 <sup>24.6</sup>
* 现在会自动检测datetime格式，以便无缝导出为XLSX格式。 <sup>24.7</sup>
* 已添加公共属性[is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/)，它允许您验证VBA项目是否受保护。 <sup>24.7</sup>
* 字体信息已扩展，**embedding_licensing_rights**属性添加到[FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/)和[PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/)类。 <sup>24.8</sup>
* 添加了一种在保留水印的同时有效清除部分页眉和页脚的方法，以更准确地使用文档结构。 要清除节页眉和页脚，请使用新的公共方法[clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default)。 <sup>24.8</sup>
* 已启用使用[XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/)对XPS文档进行数字签名–为此添加了一个新属性[digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/)。 <sup>24.8</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为Python via .NET 24.5发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 24.6发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 24.7发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 24.8发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words对于Python通过.NET 24.1, 24.2, 24.3, 24.4

Aspose.Words24.1改进了管理笔划颜色的体验，增强了OLE对象，并引入了新的`Bibliography Sources`publicAPI。

Aspose.Words24.2扩展图表API和样式管理。 此版本的Aspose.Words还引入了在渲染期间指定SvgSaveOptions的功能，更灵活地控制加载Markdown文件，以及处理脚注和尾注的参考文本。

Aspose.Words24.3为WMF元文件引入了一个新的TIFF读取器/写入器和二进制栅格操作的仿真。 Aspose.Words24.3也继续扩展图表API。

Aspose.Words24.4增强了保存格式，一些渲染选项，以及改进了数字签名的工作。

### 支持的格式 <sup>24.4</sup>

现代**WebP**图像格式现在支持 Aspose.Words为.NET Framework 4.6.2 而且更高。 您现在可以读取WebP图像并将其插入到文档中，以及以WebP格式保存图像。

请注意，WebP目前仅在.NET Standard和.NET Frameworkv4.6.2及以上版本中提供。

### 渲染和打印

#### 笔画颜色控制 <sup>24.1</sup>

[Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/)类已扩展为一组与管理笔划颜色相关的新公共属性：[fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/)和[back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/)，[fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/)和[back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/)。

#### DrawingML图表API扩展 <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API**继续扩展。

#### 嵌入在@font-face规则中声明的字体 <sup>24.4</sup>

添加了将在@font-face规则中声明的字体嵌入到结果文档的字体定义中的功能，通过添加新的[support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/)属性引入。

#### 使用发光和反射格式 <sup>24.4</sup>

已经实现了使用绘图对象的发光和反射格式的能力。

### 加载和保存文档

#### 在渲染期间指定SvgSaveOptions <sup>24.2</sup>

使用[ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/)添加了在渲染期间指定[SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/)的功能。[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions)和[OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/)。[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions)方法。

#### 加载Markdown文件时保留空行 <sup>24.2</sup>

添加了加载Markdown文件时保留空行的功能。

#### 一个新的TIFF读者/作家 <sup>24.3</sup>

已开发出适用于 Aspose.Words 的新 TIFF 读取器/写入器。针对 .NET 24.3 的 Aspose.Words增加了对读取 TIFF 压缩类型为 JPEG 和旧 JPEG 的图像的支持，并且显著提高了读写操作的质量。

### 其他

* 通过向新的**TextBoxControl**类添加新的**Text**属性，引入了修改`TextBox`OLE控件文本的功能。 <sup>24.1</sup>
* 参考书目源publicAPI是通过添加新的命名空间[Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/)及其新的类和枚举以及向[Document](https://reference.aspose.com/words/python-net/aspose.words/document/)类添加新的[bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/)属性来实现的。 <sup>24.1</sup>
* 已将用于增强样式管理的新公共属性[priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/)、[unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/)和[semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/)添加到[Style](https://reference.aspose.com/words/python-net/aspose.words/style/)类中。 <sup>24.2</sup>
* 使用[actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/)属性和[update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default)方法增强了检索脚注和尾注的实际参考标记文本的功能。 <sup>24.2</sup>
* 已经实现了对WMF元文件的二进制栅格操作的仿真。 <sup>24.3</sup>
* 通过添加具有新公共成员的新[DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/)类以及向[OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/)、[DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/)和[OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/)类添加新属性，启用了为**SaveOptions**内文档定义签名选项的功能。 <sup>24.4</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为Python via .NET 24.1发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 24.2发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 24.3发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 24.4发行说明](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words对于Python通过.NET 23.9, 23.10, 23.11, 23.12

Aspose.Words23.9扩展渲染选项、图元文件渲染仿真和markdown保存选项。

Aspose.Words23.10改进了渲染，扩展了加载和保存文档的选项，并允许用户以新的方式合并文档。

Aspose.Words23.11通过其他选项增强了图表图例上的修订、XLSX格式和字体的工作。

Aspose.Words23.12引入了用于处理PDF和OOXML文档的新属性和枚举，以及对WebP图像的支持。

### 渲染和打印

#### 在DrawingML图表中自定义轴标题 <sup>23.9</sup>

通过实现新的公共类[ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/)和[title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/)属性，引入了在DrawingML图表中自定义轴标题的功能。

####  确定字体在段落中的垂直位置 <sup>23.9</sup>

现在可以使用新的public[baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/)属性和新的[BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/)枚举来定义段落中字体的垂直位置。

#### 前景色控制 <sup>23.10</sup>

通过**BaseForeColor**属性，在[Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/)和[Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/)类中添加了不使用修饰符检索前景色的功能。

#### 扩展图表的功能 <sup>23.10</sup>

使用新的方法和属性扩展了[ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/)、[ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/)和[ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/)类的功能。

#### 自动调整图像并使其适合形状 <sup>23.10</sup>

通过新的[fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default)方法提供了一种在特定形状内自动调整和拟合图像的简单方法。

#### DrawingML图表图例条目的默认字体格式 <sup>23.11</sup>

通过[font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/)属性添加了为DrawingML图表的图例条目指定默认字体格式的功能。 此功能有助于为图表元素提供更加精简和一致的外观，从而提高整体文档美观度。

#### 在Reader中打开PDF时指定页面布局 <sup>23.12</sup>

通过向[PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/)类引入新的[page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/)属性和引入新的[PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/)枚举，添加了在PDF阅读器中打开文档时指定要使用的页面布局的功能。

### 加载和保存文档

#### 在Markdown中指定要构造ImageURIs的文件夹名称 <sup>23.9</sup>

通过包含[images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/)属性扩展了[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)类，该属性允许指定用于构造写入Markdown文档中的图像URIs的文件夹的名称。

#### 减小PDF输出大小 <sup>23.10</sup>

已经实现了各种PDF渲染优化，以减少使用[optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/)设置时的输出大小。

#### 加载TXT文档时识别超链接 <sup>23.10</sup>

加载TXT文档时识别超链接的功能已通过添加新的[detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/)属性来实现。

### 其他

- 已经实现了用于确定光栅化大小的图元文件渲染仿真，专门针对WMF笔宽和EMF笔宽。 为此，将**ScaleWmfFontsToMetafileSize**属性替换为[emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/)属性，并添加[emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/)属性。 <sup>23.9</sup>
- 使用[insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions)方法引入了将一个文档插入当前光标位置的另一个文档的简化方法。 <sup>23.10</sup>
- 通过引入新的[locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/)属性，添加了访问和修改样式属性的功能。 <sup>23.10</sup>
- 泛型类型参数已添加到[CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/)类的方法中。 <sup>23.10</sup>
- 通过新的[XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/)枚举类型和新的[section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/)属性提供了将文档的所有部分写入同一个XLSX工作表的能力。 <sup>23.11</sup>
* 通过`OoxmlSaveOptions`类的新Zip64Mode属性和新的Zip64Mode枚举实现了一种控制ZIP64格式扩展如何用于OOXML文档的方法。 <sup>23.12</sup>
* 已经引入了对WebP图像的支持。 请注意，此功能仅适用于。NetStandart和.NET6+版本。 <sup>23.12</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为Python via .NET 23.9发行说明](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 23.10发行说明](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 23.11发行说明](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

了解更多关于 [Aspose.Words为.NET 23.12 发行通知书](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words对于Python通过.NET 23.5, 23.6, 23.7, 23.8

Aspose.Words23.5增强了处理图表系列数据的能力和处理ODT文档的能力，以及改进页眉/页脚及其文本包装。

Aspose.Words23.6扩展渲染选项，添加新的导出格式，改进LINQ报告和LowCode工具。

Aspose.Words23.7增强了报告功能，添加了新的导出格式，并引入了对表和数字签名的处理的更改。

Aspose.Words23.8扩展了不同格式的功能，改进了渲染，并添加了用于处理字段的新选项。

### 支持的格式

* 从版本23.6开始，可以以XLSX格式保存文档。 现在您可以将文档转换为Excel格式。 <sup>23.6</sup>

* 从版本23.7开始，可以以EPS格式保存文档页面或形状。 <sup>23.7</sup>

### 新格式功能

- 介绍了为MOBI文档自动生成目录(TOC)的功能。 <sup>23.8</sup>
- [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions)构造函数已用[PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions)展开。 <sup>23.8</sup>
- 已经实现了EMF元文件的垂直文本整形。 <sup>23.8</sup>

### 渲染图

#### 获取和修改图表系列数据 <sup>23.5</sup>

获取和修改图表系列数据的功能是通过添加:

- 新课程: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- 新枚举类型：[ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/),[ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### 支持高级排版 <sup>23.6</sup>

在WMF，EMF和EMF+渲染中添加了对高级排版的支持。

#### 页面上的彩色内容 <sup>23.6</sup>

已添加公共属性[PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/)，指示页面是否着色。

#### 图表数据标签的格式设置 <sup>23.6</sup>

已经实现了为图表数据标签设置填充、描边和标注格式的功能。

### Mail Merge和报告

#### 动态HTML插入LINQ报告引擎 <sup>23.6</sup>

为LINQ报告引擎添加了动态HTML插入的新方法。

#### Mustache标签支持 <sup>23.7</sup>

[MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/)和[MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/)方法现在支持Mustache标记。

#### 指定渲染图像的大小 <sup>23.8</sup>

引入了一个新的公共属性[image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/)，用于指定以像素为单位的渲染图像的大小。

#### 为JSON字符串值保留空白空间-LINQ <sup>23.8</sup>

已向LINQ报告引擎添加了一个选项，用于为JSON字符串值保留空白空间。

### LowCode <sup>23.6</sup>

添加了用于将不同类型的文档合并为单个输出文档的新LowCode方法。

### 其他

- 已经实现了对页眉/页脚中的文本包装的支持。 <sup>23.5</sup>
- 通过[RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str)方法添加了从ODT文档中删除数字签名的功能。 <sup>23.5</sup>
- 添加了获取语音指南[Run](https://reference.aspose.com/words/python-net/aspose.words/run/)的基础和ruby文本的公共属性[phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/)。 <sup>23.5</sup>
- 通过引入新的[signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/)属性，添加了以字节数组形式从数字签名文档中检索数字签名值的功能。 <sup>23.7</sup>
- [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/)和[Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/)类已扩展为新的公共成员– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), 和[Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/)。 <sup>23.7</sup>

{{% alert color="primary" %}}

了解更多关于 [Aspose.Words为Python via .NET 23.5发行说明](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-5-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 23.6发行说明](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-6-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 23.7发行说明](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

了解更多关于 [Aspose.Words为Python via .NET 23.8发行说明](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## 请参阅

{{% alert color="primary" %}}

本页包含过去2年的最新发布消息。 有关早期版本的详细信息，请参阅 [发行通知书'](https://releases.aspose.com/words/python/release-notes/) 相关部分中的页面。

{{% /alert %}}
