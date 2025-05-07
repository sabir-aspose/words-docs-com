---
title: What's new
second_title: Aspose.Words for Python via .NET
articleTitle: What's new in Aspose.Words for Python via .NET
linktitle: What's new in Aspose.Words for Python via .NET
type: docs
description: "Aspose.Words for Python via .NET expands and enhances daily. On this page, you can learn about the huge and most interesting features of the product."
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-04-16-07-02-05
---

This page describes the most interesting new Aspose.Words features introduced in recent releases.

## Aspose.Words for Python via .NET 25.5

Aspose.Words 25.5 enhances chart customization with new styling options and improves Markdown export by offering control over how empty paragraphs are handled.

### Converting, Loading, and Saving Documents

#### Export Empty Paragraphs to Markdown <sup>25.5</sup>

The ability to control how empty paragraphs are exported to Markdown has been introduced by adding the **MarkdownEmptyParagraphExportMode** enumeration and the **empty_paragraph_export_mode** property.

### Rendering

#### Setting the Chart Style <sup>25.5</sup>

The ability to set the chart style has been introduced by adding the **ChartStyle** enumeration and the **style** property.

{{% alert color="primary" %}}

Learn more about [Aspose.Words for Python via .NET 25.4 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words for Python via .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 introduces AI-powered grammar checking and enhances document saving with advanced options for HTML, SVG, and Markdown formats.

Aspose.Words 25.2 introduces text summarization with Anthropic AI models, adds MsWorks format support, enhances typographic control, and improves PDF structure and list handling.

Aspose.Words 25.3 enhances an AI-powered grammar checker and font selection with the UpdateAmbiguousTextFont property, as well as improves PDF attachments export.

Aspose.Words 25.4 introduces support for new paper sizes, enables advanced HTML export control, and improves watermark handling.

### AI-powered Features

#### Document AI Grammar Checking

* The ability to check the grammar of the provided document using OpenAI generative models has been introduced by adding a new [check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/) method. <sup>25.1</sup>
* The AI-powered Grammar Checking feature has been updated to support all models available in the [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/) enumeration. <sup>25.3</sup>

#### Summarization Using Anthropic Generative Language Models <sup>25.2</sup>

Text summarization using Anthropic generative language models has been enabled by introducing a new public class [AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/).

### Supported Formats <sup>25.2</sup>

Starting from version 25.2, compatibility with the new MsWorks load format for Microsoft Works documents has been added.

### Converting, Loading, and Saving Documents

#### Improved Saving to HTML and SVG Formats <sup>25.1</sup>

Saving to HTML and SVG formats has been enhanced by adding **id_prefix** and **remove_java_script_from_links** properties to both the [HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/) and [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) classes.

#### Set Image Resolution and OfficeMath Output Mode When Saving to Markdown <sup>25.1</sup>

* A new [image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/) option has been added to the [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) class to set the image resolution.
* A new [office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/) option and [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/) enumeration have been and added to the [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) class to set OfficeMath output mode.

### Rendering

#### Improved Typographic Control <sup>25.2</sup>

The [number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/)  property has been added for improved typographic control.

#### Controlling Font Selection for Ambiguous Characters <sup>25.3</sup>

A new public property [update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/) has been added to the [SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/) class to control the font selection according to the character code used.

#### Paper Size Options <sup>25.4</sup>

The ability to use JIS B4 and JIS B5 paper sizes has been introduced by adding new values to the [PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/) enumeration.

#### HTML Output Control <sup>25.4</sup>

The ability to remove JavaScript from hyperlink URLs during HTML export has been introduced by adding the [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/) property.

### Other

* PDF logical structure has been improved with support for TOA, BIBLIOGRAPHY, and INDEX fields. <sup>25.2</sup>
* The [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate) method has been introduced for improved list handling. <sup>25.2</sup>
* A new property [attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/) has been added to replace **EmbedAttachments** to improve PDF attachments' export. Also, new values have been added to the [PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/) enumeration to support PDF/A version attachments. Additionally, attachments are now supported with encryption. <sup>25.3</sup>
* The ability to set an image watermark from a stream has been introduced by adding a new overload to the [SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions) method. <sup>25.4</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for Python via .NET 25.1 Release Notes](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

Learn more about [Aspose.Words for Python via .NET 25.2 Release Notes](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

Learn more about [Aspose.Words for Python via .NET 25.3 Release Notes](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

Learn more about [Aspose.Words for Python via .NET 25.4 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words for Python via .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduces group shape insertion and StructuredDocumentTag insertion via DocumentBuilder, enhances radial chart rendering with graduations, improves digital signatures with XAdES-EPES support, adds Markdown underline recognition, and provides access to footnote/endnote separators.

Aspose.Words 24.10 introduces enhanced ActiveX control support with CommandButton creation, new shape visibility control, the ability to group shapes, improved Markdown export for tables, chart formatting for Pie and Doughnut charts, better Big5 encoding handling, and support for outdated Taiwanese fonts.

Aspose.Words 24.11 introduces AI-powered document summarization, enhanced rendering options, improved access to document properties and ActiveX control captioning.

Aspose.Words 24.12 introduces customizable data label placement, Google AI-powered text translation, and enhanced new LowCode processing classes.

### AI-powered Features

#### Document Summarization Using OpenAI and Google <sup>24.11</sup>

Support for document summarization using **OpenAI** and **Google** generative language models has been integrated by adding the [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) namespace with its public members.

#### Text translation using Google's generative language models <sup>24.12</sup>

The ability to translate text using Google's generative language models has been implemented in Aspose.Words by adding the [translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/) method and the [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) enumeration to the [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) namespace.

### Low Code <sup>24.12</sup>

New LowCode classes like [Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) etc. has been introduced, offering a set of methods that strike the perfect balance between simplicity and flexibility for document processing.

### Rendering and Printing

#### Graduations on Radial Charts <sup>24.9</sup>

Rendering of graduations on radial charts has been implemented.

#### CommandButton ActiveX Controls <sup>24.10</sup>

The ability to create CommandButton ActiveX controls has been introduced by adding a new public method [insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/) and a new public class [Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/).

#### Control Shape Visibility <sup>24.10</sup>

A new public property [hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/) has been added to control the visibility of shapes.

#### Changes in Pie and Doughnut Charts <sup>24.10</sup>

Several new public properties have been added to format Pie and Doughnut charts.

#### Control the Rendering of PDF Choice Form Field Borders <sup>24.11</sup>

A new option to control the rendering of PDF choice form field borders has been implemented by adding a new public option [render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/).

#### Get and Set Format Codes for Chart Data <sup>24.11</sup>

The ability to get and set format codes for chart data has been added by implementing the [format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/) property in the [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), and [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/) classes.

#### Render Histogram Charts with Bins and Labels <sup>24.11</sup>

Histogram chart rendering has been improved by allowing for a specified number of bins and labels.

#### Customize the Placement of Data Labels <sup>24.12</sup>

The ability to customize the placement of data labels has been added by introducing new properties to th [ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/) and [ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/) classes.

### Converting, Loading and Saving Documents

#### Underline Formatting when Loading Markdown Files <sup>24.9</sup>

The option to recognize underline formatting when loading Markdown documents has been incorporated by adding a new public property [import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/).

#### Exporting tables as HTML when saving to Markdown <sup>24.10</sup>

An option to export tables as HTML when saving documents to Markdown format has been implemented by adding a new public property [export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/) and an enumeration [MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/).

#### Export PDF with Updated Logical Structure <sup>24.11</sup>

PDF export has been enhanced by including table title properties as PDF logical structure element titles.

### Digital Signatures

#### Sign Documents with XAdES-EPES <sup>24.9</sup>

The ability to sign documents with XAdES-EPES level XML-DSig signatures has been introdused by adding a new public property [xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/) and a new public enumeration [XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/).

### Other

* A new public method [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/) has been added to group shapes. <sup>24.9</sup>
* A new public method [insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/) has been added to insert **StructuredDocumentTags** into a document. <sup>24.9</sup>
* Public access to footnote/endnote separators has been provided by adding a few public classes and properties. <sup>24.9</sup>
* The ability to group individual shapes, group shapes together, and directly group both shapes and group shapes has been introduced by adding the [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist) method. <sup>24.10</sup>
* Big5 encoding handling for TrueType cmap tables has been improved. <sup>24.10</sup>
* Support for outdated Taiwanese fonts has been enhanced. <sup>24.10</sup>
* To access extended document properties, read-only properties have been added to the [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/) class. <sup>24.11</sup>
* Setting captions for ActiveX controls has been enabled by adding a new public setter to the [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/) property. <sup>24.11</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for Python via .NET 24.9 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

Learn more about [Aspose.Words for Python via .NET 24.10 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

Learn more about [Aspose.Words for Python via .NET 24.11 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

Learn more about [Aspose.Words for Python via .NET 24.12 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words for Python via .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 expands options for assemblies, improves rendering capabilities, and expands some other options.

Aspose.Words 24.6 improves rendering options, enhances search and compare functionality, and expands several other features.

Aspose.Words 24.7 changes how you work with ActiveX, expands rendering capabilities, as well as exporting to Markdown and XLSX formats.

Aspose.Words 24.8 enhances chart customization with precise control over axis labels, expands font management, improves document structure handling, and adds new capabilities for HTML/XAML export, PDF functionality, document conversion, and digital signatures.

### Supported Formats

Starting from version 24.7, export to PDF/UA-2 is supported to ensure accessibility for users with disabilities.

### Rendering and Printing

#### Changes in Charts, Shapes and DrawingML <sup>24.5</sup>

* DrawingML effects rendering for SVG graphics, extending previous functionality limited to images, has been implemented.
* Support for creating combo charts and adjusting properties such as gap width, overlap, and bubble scale within series groups has been introduced by adding the [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/) and [ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/) classes and the [series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/) property.
* Functionality to manipulate the SoftEdge effect of shapes has been implemented by adding the [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/) class.
* The ability to modify adjust values of shapes has been implemented by adding the **AdjustmentCollection** and **Adjustment** public classes and [adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/) property.

#### Changes in Charts, Shapes and Drawing <sup>24.6</sup>

- Charting capabilities have been enhanced. You can now create a wider variety of charts, including *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* charts, *Box & Whisker* charts, *Waterfalls*, and *Funnels*. This allows you to visualize your data in a more diverse and informative way.
- Color control for shadow formatting has been improved. You can gain more precise control over the appearance of your documents by accessing shadow colors.
- Performance boost for background rendering has been improved. You can significantly speed up the rendering of backgrounds containing small elements thanks to native tiling technology.
- Realistic gradients for shapes have been added. You can now create DML shapes with non-linear gradients, mimicking the visual style of Microsoft Word for a more polished look.

#### Chart Data Label Customization <sup>24.7</sup>

The ability to customize chart data labels such as **Orientation** and **Rotation** has been added.

#### Custom Number Styling for List Levels <sup>24.7</sup>

A setter for the public property [custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/) has been added. You can now define a custom number styling for list levels.

#### Changes in working with ActiveX <sup>24.7</sup>

- The properties of ActiveX objects can now be modified, giving you more control over their behavior.
- The ability to modify the value of the radio button ActiveX control to enable dynamic interaction has been added.
- The ability to toggle an ActiveX checkbox to "checked" or "unchecked" has been added.

#### Control Over the Chart Axis Tick Labels Orientation and Rotation <sup>24.8</sup>

Precise control over the orientation and rotation of chart axis tick labels has been added for more convenient chart customization – the [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) class has been extended with new [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) and [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/) properties.

#### Replacing the Backslash with the Yen Sign <sup>24.8</sup>

The backwards compatible HTML and XAML export for replacing the backslash character with the Yen sign has been improved. To achieve this, the **replace_backslash_with_yen_sign** property has been added to the [HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/) and [XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/) classes.

#### Using SDT Tags as Form Field Names when Exporting to PDF <sup>24.8</sup>

PDF export with support for using SDT tags as form field names has been enhanced by adding a new [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) property to the [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) class.

### Converting, Loading and Saving Documents

#### Exporting Links to Markdown Format <sup>24.7</sup>

The ability to control the export of links in Markdown format has been added through the implementation of the [link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/) property.

#### LowCode 24.8 <sup>24.8</sup>

A new [LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/) class, designed to provide a set of methods for converting various document types with a single line of code, has been introduced.

### Search and Compare

#### Advanced Comparison Options <sup>24.6</sup>

The ability to streamline data analysis workflows with improved comparison functionality has been added. This includes a new [ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/) option and a redesigned interface for advanced comparisons.

### Other

* The function to eliminate empty pages from a document has been implemented by adding the [remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/) method. <sup>24.5</sup>
* The ability  to check for the presence of VBA macros without loading a document has been provided by adding the [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/) property. <sup>24.5</sup>
* Keeping source numbering while inserting a document using the LINQ Reporting Engine is now supported. <sup>24.5</sup>
* A new [date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/) property has been added – this provides a more precise timestamp for comments, improving organization and traceability. <sup>24.6</sup>
* The datetime format is now automatically detected for seamless export to XLSX format. <sup>24.7</sup>
* The public property [is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/), which allows you to verify whether a VBA project is protected, has been added. <sup>24.7</sup>
* Font information has been expanded with the **embedding_licensing_rights** property added to the [FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/) and [PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/) classes. <sup>24.8</sup>
* A way to efficiently clear section headers and footers while preserving watermarks has been added to more accurately work with document structure. To clear section headers and footers, use the new public method [clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default). <sup>24.8</sup>
* Digital signing of XPS documents using [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/) has been enabled – a new property [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/) has been added for this purpose. <sup>24.8</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for Python via .NET 24.5 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

Learn more about [Aspose.Words for Python via .NET 24.6 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

Learn more about [Aspose.Words for Python via .NET 24.7 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

Learn more about [Aspose.Words for Python via .NET 24.8 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words for Python via .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 improves the experience around managing stroke colors, enhances OLE objects, as well as introduces a new `Bibliography Sources` public API.

Aspose.Words 24.2 expanded Charts API and style management. This version of Aspose.Words also introduced the capability to specify SvgSaveOptions during rendering, more flexible control loading Markdown files, and working with reference text for footnotes and endnotes.

Aspose.Words 24.3 introduces a new TIFF Reader/Writer and Emulation of binary raster operations for WMF metafiles. Aspose.Words 24.3 also continues to expand the Charts API.

Aspose.Words 24.4 enhances saving formats, some rendering options, as well as improves work with digital signatures.

### Supported Formats <sup>24.4</sup>

The modern **WebP** image format is now supported in Aspose.Words for .NET Framework 4.6.2 and higher. You can now read and insert WebP images into documents, as well as save images in WebP format.

Please note that WebP is currently only available in .NET Standard and .NET Framework v4.6.2 and above.

### Rendering and Printing

#### Stroke Color Control <sup>24.1</sup>

The [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) class has been extended with a set of new public properties related to managing stroke colors: [fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/) and [back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/), [fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/) and [back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### DrawingML Charts API Extension <sup>24.2 / 24.3 / 24.4</sup>

The **DrawingML Charts API** continues to be expanded.

#### Embed Fonts Declared in @font-face Rules <sup>24.4</sup>

Added an ability to embed fonts declared in @font-face rules into the resulting document’s font definitions has been introduced by adding a new [support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/) property.

#### Work with Glow and Reflection Formatting <sup>24.4</sup>

The ability to work with glow and reflection formatting for a drawing object has been implemented.

### Loading and Saving Documents

#### Specify SvgSaveOptions During Rendering <sup>24.2</sup>

The capability to specify [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) during rendering has been added using the [ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) and [OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) methods.

#### Preserve Empty Lines when Loading Markdown files <sup>24.2</sup>

The ability to preserve empty lines when loading Markdown files has been added.

#### A New TIFF Reader/Writer <sup>24.3</sup>

A new TIFF reader/writer for Aspose.Words has been developed. Aspose.Words for .NET 24.3 added support for reading TIFF images with JPEG and Old JPEG compression types, and also significantly improved the quality of read and write operations.

### Other

* The capability to modify the text of the `TextBox` OLE control has been introduced by adding a new **Text** property to the new **TextBoxControl** class. <sup>24.1</sup>
* The Bibliography Sources public API was implemented through the adding a new namespace [Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/) with its new classes and enumerations, and through the adding a new [bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/) property to the [Document](https://reference.aspose.com/words/python-net/aspose.words/document/) class. <sup>24.1</sup>
* New public properties [priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/), [unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/), and [semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/) for enhanced style management have been added to the [Style](https://reference.aspose.com/words/python-net/aspose.words/style/) class. <sup>24.2</sup>
* The functionality to retrieve the actual reference mark text for footnotes and endnotes has been enhanced with the [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/) property and the [update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default) method. <sup>24.2</sup>
* Emulation of binary raster operations for WMF metafiles has been implemented. <sup>24.3</sup>
* The capability to define signature options for documents within **SaveOptions** has been enabled by adding a new [DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/) class with new public members, as well as adding new properties to the [OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/) and [OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/) classes. <sup>24.4</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for Python via .NET 24.1 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

Learn more about [Aspose.Words for Python via .NET 24.2 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

Learn more about [Aspose.Words for Python via .NET 24.3 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

Learn more about [Aspose.Words for Python via .NET 24.4 Release Notes](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words for Python via .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 expands rendering options, metafile rendering emulation, and markdown save options.

Aspose.Words 23.10 improves rendering, expands options for loading and saving documents, and allows users to merge documents in new ways.

Aspose.Words 23.11 enhances the work with revisions, XLSX format and fonts on chart legend with additional options.

Aspose.Words 23.12 introduces new properties and enumerations for working with PDF and OOXML documents, as well as support for WebP images.

### Rendering and Printing

#### Customizing Axes Titles in DrawingML Charts <sup>23.9</sup>

The capability to customize axis titles in DrawingML charts has been introduced by the implementation of a new public class [ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/) and [title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/) property.

####  Determining the Vertical Position of Fonts within a Paragraph <sup>23.9</sup>

It is now possible to define the vertical position of fonts within a paragraph using the new public [baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/) property and the new [BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/) enumeration.

#### Foreground Color Control <sup>23.10</sup>

The ability to retrieve the foreground color without modifiers has been added to the [Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/) and [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) classes via the **BaseForeColor** property.

#### Expanding the Functionality of Charts <sup>23.10</sup>

The functionality of the [ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/), and [ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/) classes has been expanded with new methods and properties.

#### Automatically Adjust and Fit an Image into a Shape <sup>23.10</sup>

A simple way to automatically adjust and fit an image within a particular shape has been provided through the new [fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default) method.

#### Default Font Formatting for DrawingML Chart Legend Entries <sup>23.11</sup>

The ability to specify default font formatting for legend entries of DrawingML charts has been added via the [font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/) property. This feature facilitates a more streamlined and consistent appearance for chart elements, improving the overall document aesthetics.

#### Specify Page Layout when Opening PDF in Reader <sup>23.12</sup>

The ability to specify the page layout to be used when opening a document in a PDF reader has been added through the introduction of a new [page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/) property to the [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) class and the introduction of a new [PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/) enumeration.

### Loading and Saving Documents

#### Specifying a Folder Name to Construct Image URIs in Markdown <sup>23.9</sup>

The [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) class has been expanded by including the [images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/) property, which allows to specifies the name of the folder used to construct image URIs written into the Markdown document.

#### Reduce PDF Output Size <sup>23.10</sup>

Various PDF rendering optimizations to reduce output size when utilizing [optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/) settings have been implemented.

#### Recognize Hyperlinks when Loading TXT Documents <sup>23.10</sup>

The feature to recognize hyperlinks when loading TXT documents has been implemented by adding a new [detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/) property.

### Other

- Metafile rendering emulation to determine rasterization size has been implemented, specifically for WMF pen width and EMF cosmetic pen width. To achieve this, the **ScaleWmfFontsToMetafileSize** property was replaced with the [emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/) property and the [emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/) property was added. <sup>23.9</sup>
- A simplified method for inserting one document into another document at the current cursor position has been introduced using the [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions) method. <sup>23.10</sup>
- The ability to access and modify style properties has been added through the introduction of the new [locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/) property.  <sup>23.10</sup>
- A generic type parameter has been added to the methods of the [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/) class. <sup>23.10</sup>
- The ability to write all sections of a document onto the same XLSX worksheet has been provided through the new [XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/) enumeration type and the new [section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/) property. <sup>23.11</sup>
* A way to control how ZIP64 format extensions will be used for OOXML documents has been implemented through the new Zip64Mode property of the `OoxmlSaveOptions` class and the new Zip64Mode enumeration. <sup>23.12</sup>
* Support for WebP image has been introduced. Please note that this feature is only available for .NetStandart and .NET6+ versions. <sup>23.12</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for Python via .NET 23.9 Release Notes](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

Learn more about [Aspose.Words for Python via .NET 23.10 Release Notes](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

Learn more about [Aspose.Words for Python via .NET 23.11 Release Notes](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

Learn more about [Aspose.Words for .NET 23.12 Release Notes](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words for Python via .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 enhances the ability to work with chart series data and the ability to work with ODT documents, as well as improve headers/footers and their text wrapping.

Aspose.Words 23.6 expands rendering options, adds a new export format, improves LINQ reporting and LowCode tools.

Aspose.Words 23.7 enhances reporting capabilities, adds a new export format, and introduces changes to working with tables and digital signatures.

Aspose.Words 23.8 expands the capabilities of different formats, improves rendering, and adds new options for working with fields. 

### Supported Formats

* Starting with version 23.6, it is possible to save a document in XLSX format. Now you can convert your documents to Excel format. <sup>23.6</sup>

* Starting with version 23.7, it is possible to save a document page or shape in EPS format. <sup>23.7</sup>

### New Format Features

- The functionality to automatically generate Table of Contents (TOC) for MOBI documents has been introduced. <sup>23.8</sup>
- The [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) constructor has been expanded with [PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions). <sup>23.8</sup>
- Shaping of vertical text for EMF metafiles has been implemented. <sup>23.8</sup>

### Rendering

#### Get and Modify Chart Series Data <sup>23.5</sup>

The feature to get and modify chart series data was provided by adding:

- new classes: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- new enum types: [ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### Support for Advanced Typography <sup>23.6</sup>

Support for Advanced Typography in WMF, EMF and EMF+ rendering has been added.

#### Colored Content on the Page <sup>23.6</sup>

The public property [PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/), indicating whether the page is colored or not, has been added.

#### Formatting for Chart Data Labels <sup>23.6</sup>

The ability to set fill, stroke, and callout formatting for chart data labels has been implemented.

### Mail Merge and Reporting

#### Dynamic HTML Insertion for LINQ Reporting Engine <sup>23.6</sup>

A new way of dynamic HTML insertion for LINQ Reporting Engine has been added.

#### Mustache Tags Support <sup>23.7</sup>

Mustache tags are now supported in the [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/) and [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/) methods.

#### Specifying the Size of Rendered Images <sup>23.8</sup>

A new public property [image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/) for specifying the size of rendered images in pixel has been introduced.

#### Preserve Whitespaces for JSON String Values – LINQ <sup>23.8</sup>

An option has been added to the LINQ Reporting Engine to preserve whitespaces for JSON string values.

### LowCode <sup>23.6</sup>

New LowCode methods intended to merge different types of documents into a single output document have been added.

### Other

- Support for text wrapping in headers/footers has been implemented. <sup>23.5</sup>
- The ability to remove digital signatures from ODT documents has been added through the [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str) method. <sup>23.5</sup>
- The public property [phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/) to obtain the base and ruby text of the phonetic guide [Run](https://reference.aspose.com/words/python-net/aspose.words/run/) has been added. <sup>23.5</sup>
- The ability to retrieve a digital signature value from a digitally signed document as a byte array has been added by introducing a new [signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/) property. <sup>23.7</sup>
- The [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/) and [Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/) classes have been extended with new public members – [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), and [Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/). <sup>23.7</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for Python via .NET 23.5 Release Notes](/words/python-net/aspose-words-for-python-via-dotnet-23-5-release-notes/).

Learn more about [Aspose.Words for Python via .NET 23.6 Release Notes](/words/python-net/aspose-words-for-python-via-dotnet-23-6-release-notes/).

Learn more about [Aspose.Words for Python via .NET 23.7 Release Notes](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

Learn more about [Aspose.Words for Python via .NET 23.8 Release Notes](/words/python-net/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## See Also

{{% alert color="primary" %}}

This page contains the latest release news for the past 2 years. For details on earlier releases, see the [Release Notes'](https://releases.aspose.com/words/python/release-notes/) pages in the relevant sections.

{{% /alert %}}
