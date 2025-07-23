---
title: What's new
second_title: Aspose.Words for .NET
articleTitle: What's new in Aspose.Words for .NET
linktitle: What's new in Aspose.Words for .NET
type: docs
description: "Aspose.Words for .NET expands and enhances daily. On this page, you can learn about the huge and most interesting features of the product."
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /net/what-s-new-in-aspose-words-for-net/
timestamp: 2025-06-23-21-02-49
---

This page describes the most interesting new Aspose.Words features introduced in recent releases.

## Aspose.Words for .NET 25.5, 25.6

Aspose.Words 25.5 enhances chart customization with new styling options and improves Markdown export by offering control over how empty paragraphs are handled.

Aspose.Words 25.6 enhances rendering precision and visualization features by introducing advanced image export options, improved MathML handling, and better chart representation.

### Converting, Loading, and Saving Documents

#### Export Empty Paragraphs to Markdown <sup>25.5</sup>

The ability to control how empty paragraphs are exported to Markdown has been introduced by adding the [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownemptyparagraphexportmode/) enumeration and the [EmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/emptyparagraphexportmode/) property.

#### Export Multi-page Documents to Raster Image Formats <sup>25.6</sup>

The ability to export multi-page documents to raster image formats (such as PNG and JPEG) with [customizable layouts](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) – Horizontal, Vertical, or Grid – has been introduced by extending image export functionality.

### Rendering

#### Setting the Chart Style <sup>25.5</sup>

The ability to set the chart style has been introduced by adding the [ChartStyle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartstyle/) enumeration and the [Style](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/style/) property.

#### Rendering Connector Lines in MathML Expressions <sup>25.6</sup>

The rendering of connector lines in MathML expressions has been implemented to ensure more accurate and visually consistent display of mathematical formulas.

#### Rendering Legends for Waterfall Charts <sup>25.6</sup>

The rendering of legends for ["Waterfall" charts](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriestype/) has been introduced, increasing data transparency and improving the interpretability of these charts.

### Other

* The ability to wrap mathematical formulas containing multiple slashes has been enhanced, improving layout clarity and formula legibility. <sup>25.6</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for .NET 25.5 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-5-release-notes/).

Learn more about [Aspose.Words for .NET 25.6 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words for .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 introduces AI-powered grammar checking and enhances document saving with advanced options for HTML, SVG, and Markdown formats.

Aspose.Words 25.2 introduces text summarization with Anthropic AI models, adds MsWorks format support, enhances typographic control, and improves PDF structure and list handling.

Aspose.Words 25.3 enhances an AI-powered grammar checker and font selection with the UpdateAmbiguousTextFont property, as well as improves PDF attachments export.

Aspose.Words 25.4 introduces support for new paper sizes, enables advanced HTML export control, improves watermark handling, and enhances the usability of the LowCode API.

### AI-powered Features

#### Document AI Grammar Checking

* The ability to check the grammar of the provided document using OpenAI generative models has been introduced by adding a new [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/aimodel/checkgrammar/) method. <sup>25.1</sup>
* The AI-powered Grammar Checking feature has been updated to support all models available in the [AiModelType](https://reference.aspose.com/words/net/aspose.words.ai/aimodeltype/) enumeration. <sup>25.3</sup>

#### Summarization Using Anthropic Generative Language Models <sup>25.2</sup>

Text summarization using Anthropic generative language models has been enabled by introducing a new public class [AnthropicAiModel](https://reference.aspose.com/words/net/aspose.words.ai/anthropicaimodel/).

### Low Code

#### Low Code API Usability <sup>25.4</sup>

Significant improvements to the usability of the **LowCode API** have been introduced, simplifying document processing and reducing the need for repetitive code.

### Supported Formats <sup>25.2</sup>

Starting from version 25.2, compatibility with the new MsWorks load format for Microsoft Works documents has been added.

### Converting, Loading, and Saving Documents

#### Improved Saving to HTML and SVG Formats <sup>25.1</sup>

Saving to HTML and SVG formats has been enhanced by adding **IdPrefix** and **RemoveJavaScriptFromLinks** properties to both the [HtmlFixedSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlfixedsaveoptions/) and [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/) classes.

#### Set Image Resolution and OfficeMath Output Mode When Saving to Markdown <sup>25.1</sup>

* A new [ImageResolution](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imageresolution/) option has been added to the [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) class to set the image resolution.
* A new [OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/officemathexportmode/) option and [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownofficemathexportmode/) enumeration have been and added to the [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) class to set OfficeMath output mode.
* The ability to set an image watermark from a stream has been introduced by adding a new overload to the [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage_2) method. <sup>25.4</sup>

### Rendering

#### Improved Typographic Control <sup>25.2</sup>

The [NumberSpacing](https://reference.aspose.com/words/net/aspose.words/font/numberspacing/) property has been added for improved typographic control.

#### Controlling Font Selection for Ambiguous Characters <sup>25.3</sup>

A new public property [UpdateAmbiguousTextFont](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/updateambiguoustextfont/) has been added to the [SaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/) class to control the font selection according to the character code used.

#### Paper Size Options <sup>25.4</sup>

The ability to use JIS B4 and JIS B5 paper sizes has been introduced by adding new values to the [PaperSize](https://reference.aspose.com/words/net/aspose.words/papersize/) enumeration.

#### HTML Output Control <sup>25.4</sup>

The ability to remove JavaScript from hyperlink URLs during HTML export has been introduced by adding the [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/removejavascriptfromlinks/) property.

### Other

* PDF logical structure has been improved with support for TOA, BIBLIOGRAPHY, and INDEX fields. <sup>25.2</sup>
* The [AddSingleLevelList](https://reference.aspose.com/words/net/aspose.words.lists/listcollection/addsinglelevellist/) method has been introduced for improved list handling. <sup>25.2</sup>
* A new property [AttachmentsEmbeddingMode](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/attachmentsembeddingmode/) has been added to replace **EmbedAttachments** to improve PDF attachments' export. Also, new values have been added to the [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) enumeration to support PDF/A version attachments. Additionally, attachments are now supported with encryption. <sup>25.3</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for .NET 25.1 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-1-release-notes/).

Learn more about [Aspose.Words for .NET 25.2 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-2-release-notes/).

Learn more about [Aspose.Words for .NET 25.3 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-3-release-notes/).

Learn more about [Aspose.Words for .NET 25.4 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words for .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduces group shape insertion and StructuredDocumentTag insertion via DocumentBuilder, enhances radial chart rendering with graduations, improves digital signatures with XAdES-EPES support, adds Markdown underline recognition, and provides access to footnote/endnote separators.

Aspose.Words 24.10 introduces enhanced ActiveX control support with CommandButton creation, new shape visibility control, the ability to group shapes, improved Markdown export for tables, chart formatting for Pie and Doughnut charts, better Big5 encoding handling, and support for outdated Taiwanese fonts.

Aspose.Words 24.11 introduces AI-powered document summarization, enhanced rendering options, improved access to document properties and ActiveX control captioning.

Aspose.Words 24.12 introduces customizable data label placement, Google AI-powered text translation, enhanced Mail Merge cleanup options, and new LowCode processing classes.

### AI-powered Features

#### Document Summarization Using OpenAI and Google <sup>24.11</sup>

Support for document summarization using **OpenAI** and **Google** generative language models has been integrated by adding the [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) namespace with its public members.

#### Text translation using Google's generative language models <sup>24.12</sup>

The ability to translate text using Google's generative language models has been implemented in Aspose.Words by adding the [Translate](https://reference.aspose.com/words/net/aspose.words.ai/aimodel/translate/) method and the [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) enumeration to the [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) namespace.

### Low Code <sup>24.12</sup>

New LowCode classes like [Comparer](https://reference.aspose.com/words/net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/net/aspose.words.lowcode/splitter/) etc. has been introduced, offering a set of methods that strike the perfect balance between simplicity and flexibility for document processing.

### Rendering and Printing

#### Graduations on Radial Charts <sup>24.9</sup>

Rendering of graduations on radial charts has been implemented.

#### CommandButton ActiveX Controls <sup>24.10</sup>

The ability to create CommandButton ActiveX controls has been introduced by adding a new public method [InsertForms2OleControl](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertforms2olecontrol/) and a new public class [Forms2OleControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/).

#### Control Shape Visibility <sup>24.10</sup>

A new public property [Hidden](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/hidden/) has been added to control the visibility of shapes.

#### Changes in Pie and Doughnut Charts <sup>24.10</sup>

Several new public properties have been added to format Pie and Doughnut charts.

#### Control the Rendering of PDF Choice Form Field Borders <sup>24.11</sup>

A new option to control the rendering of PDF choice form field borders has been implemented by adding a new public option [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/renderchoiceformfieldborder/).

#### Get and Set Format Codes for Chart Data <sup>24.11</sup>

The ability to get and set format codes for chart data has been added by implementing the [FormatCode](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/formatcode/) property in the [ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/), and [BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/) classes.

#### Render Histogram Charts with Bins and Labels <sup>24.11</sup>

Histogram chart rendering has been improved by allowing for a specified number of bins and labels.

#### Customize the Placement of Data Labels <sup>24.12</sup>

The ability to customize the placement of data labels has been added by introducing new properties to the [ChartDataLabel](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabel/) and [ChartDataLabelCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/) classes.

### Converting, Loading and Saving Documents

#### Underline Formatting when Loading Markdown Files <sup>24.9</sup>

The option to recognize underline formatting when loading Markdown documents has been incorporated by adding a new public property [ImportUnderlineFormatting](https://reference.aspose.com/words/net/aspose.words.loading/markdownloadoptions/importunderlineformatting/).

#### Exporting tables as HTML when saving to Markdown <sup>24.10</sup>

An option to export tables as HTML when saving documents to Markdown format has been implemented by adding a new public property [ExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/exportashtml/) and an enumeration [MarkdownExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownexportashtml/).

#### Export PDF with Updated Logical Structure <sup>24.11</sup>

PDF export has been enhanced by including table title properties as PDF logical structure element titles.

### Mail Merge and Reporting

#### Remove Empty Tables during Mail Merge <sup>24.12</sup>

A new **RemoveEmptyTables** option has been added to the [MailMergeCleanupOptions](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmergecleanupoptions/) enumeration to refine Mail Merge output.

### Digital Signatures

#### Sign Documents with XAdES-EPES <sup>24.9</sup>

The ability to sign documents with XAdES-EPES level XML-DSig signatures has been introdused by adding a new public property [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/signoptions/xmldsiglevel/) and a new public enumeration [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/xmldsiglevel/).

### Other

* A new public method [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/) has been added to group shapes. <sup>24.9</sup>
* A new public method [InsertStructuredDocumentTag](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertstructureddocumenttag/) has been added to insert **StructuredDocumentTags** into a document. <sup>24.9</sup>
* Public access to footnote/endnote separators has been provided by adding a few public classes and properties. <sup>24.9</sup>
* The ability to group individual shapes, group shapes together, and directly group both shapes and group shapes has been introduced by adding the [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/#insertgroupshape_1) method. <sup>24.10</sup>
* Big5 encoding handling for TrueType cmap tables has been improved. <sup>24.10</sup>
* Support for outdated Taiwanese fonts has been enhanced. <sup>24.10</sup>
* To access extended document properties, read-only properties have been added to the [BuiltInDocumentProperties](https://reference.aspose.com/words/net/aspose.words.properties/builtindocumentproperties/) class. <sup>24.11</sup>
* Setting captions for ActiveX controls has been enabled by adding a new public setter to the [Forms2OleControl.Caption](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/caption/) property. <sup>24.11</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for .NET 24.9 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-9-release-notes/).

Learn more about [Aspose.Words for .NET 24.10 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-10-release-notes/).

Learn more about [Aspose.Words for .NET 24.11 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-11-release-notes/).

Learn more about [Aspose.Words for .NET 24.12 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words for .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 expands options for assemblies, improves rendering capabilities, and expands some other options.

Aspose.Words 24.6 improves rendering options, enhances search and compare functionality, and expands several other features.

Aspose.Words 24.7 changes how you work with ActiveX, expands rendering capabilities, as well as exporting to Markdown and XLSX formats.

Aspose.Words 24.8 enhances chart customization with precise control over axis labels, expands font management, improves document structure handling, and adds new capabilities for HTML/XAML export, PDF functionality, document conversion, and digital signatures.

### Supported Formats

Starting from version 24.7, export to PDF/UA-2 is supported to ensure accessibility for users with disabilities.

### Platforms <sup>24.5</sup>

.NET 7.0/8.0 assemblies have been included in the Aspose.Words NuGet package.

### Rendering and Printing

#### Changes in Charts, Shapes and DrawingML <sup>24.5</sup>

* DrawingML effects rendering for SVG graphics, extending previous functionality limited to images, has been implemented.
* Support for creating combo charts and adjusting properties such as gap width, overlap, and bubble scale within series groups has been introduced by adding the [ChartSeriesGroup](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroup/) and [ChartSeriesGroupCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroupcollection/) classes and the [SeriesGroups](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/seriesgroups/) property.
* Functionality to manipulate the SoftEdge effect of shapes has been implemented by adding the [SoftEdgeFormat](https://reference.aspose.com/words/net/aspose.words.drawing/softedgeformat/) class.
* The ability to modify adjust values of shapes has been implemented by adding the [AdjustmentCollection](https://reference.aspose.com/words/net/aspose.words.drawing/adjustmentcollection/) and [Adjustment](https://reference.aspose.com/words/net/aspose.words.drawing/adjustment/) public classes and [Adjustments](https://reference.aspose.com/words/net/aspose.words.drawing/shape/adjustments/) property.

#### Changes in Charts, Shapes and Drawing <sup>24.6</sup>

* Charting capabilities have been enhanced. You can now create a wider variety of charts, including *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* charts, *Box & Whisker* charts, *Waterfalls*, and *Funnels*. This allows you to visualize your data in a more diverse and informative way.
* Color control for shadow formatting has been improved. You can gain more precise control over the appearance of your documents by accessing shadow colors.
* Performance boost for background rendering has been improved. You can significantly speed up the rendering of backgrounds containing small elements thanks to native tiling technology.
* Realistic gradients for shapes have been added. You can now create DML shapes with non-linear gradients, mimicking the visual style of Microsoft Word for a more polished look.

#### Chart Data Label Customization <sup>24.7</sup>

The ability to customize chart data labels such as **Orientation** and **Rotation** has been added.

#### Custom Number Styling for List Levels <sup>24.7</sup>

A setter for the public property [CustomNumberStyleFormat](https://reference.aspose.com/words/net/aspose.words.lists/listlevel/customnumberstyleformat/) has been added. You can now define a custom number styling for list levels.

#### Changes in working with ActiveX <sup>24.7</sup>

* The properties of ActiveX objects can now be modified, giving you more control over their behavior.
* The ability to modify the value of the radio button ActiveX control to enable dynamic interaction has been added.
* The ability to toggle an ActiveX checkbox to "checked" or "unchecked" has been added.

#### Control Over the Chart Axis Tick Labels Orientation and Rotation <sup>24.8</sup>

Precise control over the orientation and rotation of chart axis tick labels has been added for more convenient chart customization – the [AxisTickLabels](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/) class has been extended with new [Orientation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/orientation/) and [Rotation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/rotation/) properties.

#### Replacing the Backslash with the Yen Sign <sup>24.8</sup>

The backwards compatible HTML and XAML export for replacing the backslash character with the Yen sign has been improved. To achieve this, the **ReplaceBackslashWithYenSign** property has been added to the [HtmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/) and [XamlFlowSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xamlflowsaveoptions/) classes.

#### Using SDT Tags as Form Field Names when Exporting to PDF <sup>24.8</sup>

PDF export with support for using SDT tags as form field names has been enhanced by adding a new [UseSdtTagAsFormFieldName](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/usesdttagasformfieldname/) property to the [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) class.

### Converting, Loading and Saving Documents

#### Exporting Links to Markdown Format <sup>24.7</sup>

The ability to control the export of links in Markdown format has been added through the implementation of the [LinkExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/linkexportmode/) property.

#### LowCode 24.8 <sup>24.8</sup>

A new [LowCode.Converter](https://reference.aspose.com/words/net/aspose.words.lowcode/converter/) class, designed to provide a set of methods for converting various document types with a single line of code, has been introduced.

### Search and Compare

#### Advanced Comparison Options <sup>24.6</sup>
The ability to streamline data analysis workflows with improved comparison functionality has been added. This includes a new [IgnoreStoreItemId](https://reference.aspose.com/words/net/aspose.words.comparing/advancedcompareoptions/ignorestoreitemid/) option and a redesigned interface for advanced comparisons.

### Other

* The function to eliminate empty pages from a document has been implemented by adding the [RemoveBlankPages](https://reference.aspose.com/words/net/aspose.words/document/removeblankpages/) method. <sup>24.5</sup>
* The ability  to check for the presence of VBA macros without loading a document has been provided by adding the [HasMacros](https://reference.aspose.com/words/net/aspose.words/fileformatinfo/hasmacros/) property. <sup>24.5</sup>
* Keeping source numbering while inserting a document using the LINQ Reporting Engine is now supported. <sup>24.5</sup>
* A new [DateTimeUtc](https://reference.aspose.com/words/net/aspose.words/comment/datetimeutc/) property has been added – this provides a more precise timestamp for comments, improving organization and traceability. <sup>24.6</sup>
* The LINQ Reporting Engine has been improved. Selective removal of empty paragraphs and definition of custom messages for missing object members have been made, leading to cleaner and more informative reports. <sup>24.6</sup>
* The datetime format is now automatically detected for seamless export to XLSX format. <sup>24.7</sup>
* The public property [IsProtected](https://reference.aspose.com/words/net/aspose.words.vba/vbaproject/isprotected/), which allows you to verify whether a VBA project is protected, has been added. <sup>24.7</sup>
* Font information has been expanded with the **EmbeddingLicensingRights** property added to the [FontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/fontinfo/) and [PhysicalFontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/physicalfontinfo/) classes. <sup>24.8</sup>
* A way to efficiently clear section headers and footers while preserving watermarks has been added to more accurately work with document structure. To clear section headers and footers, use the new public method [ClearHeadersFooters](https://reference.aspose.com/words/net/aspose.words/section/clearheadersfooters/). <sup>24.8</sup>
* Digital signing of XPS documents using [XpsSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/) has been enabled – a new property [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/digitalsignaturedetails/) has been added for this purpose. <sup>24.8</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for .NET 24.5 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-5-release-notes/).

Learn more about [Aspose.Words for .NET 24.6 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-6-release-notes/).

Learn more about [Aspose.Words for .NET 24.7 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-7-release-notes/).

Learn more about [Aspose.Words for .NET 24.8 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words for .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 improves the experience around managing stroke colors, enhances OLE objects and LINQ reporting, as well as introduces a new `Bibliography Sources` public API.

Aspose.Words 24.2 expanded Charts API, style management, and LINQ options. This version of Aspose.Words also introduced the capability to specify SvgSaveOptions during rendering, more flexible control loading Markdown files, and working with reference text for footnotes and endnotes.

Aspose.Words 24.3 introduces a new TIFF Reader/Writer and Emulation of binary raster operations for WMF metafiles. Aspose.Words 24.3 also continues to expand the Charts API.

Aspose.Words 24.4 enhances saving formats, some rendering options, as well as improves work with digital signatures.

### Supported Formats <sup>24.4</sup>

The modern **WebP** image format is now supported in Aspose.Words for .NET Framework 4.6.2 and higher. You can now read and insert WebP images into documents, as well as save images in WebP format.

Please note that WebP is currently only available in .NET Standard and .NET Framework v4.6.2 and above.

### Rendering and Printing

#### Stroke Color Control <sup>24.1</sup>

The [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) class has been extended with a set of new public properties related to managing stroke colors: [ForeThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/forethemecolor/) and [BackThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/foretintandshade/) and [BackTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backtintandshade/).

#### DrawingML Charts API Extension <sup>24.2 / 24.3 / 24.4</sup>

The **DrawingML Charts API** continues to be expanded.

#### Embed Fonts Declared in @font-face Rules <sup>24.4</sup>

Added an ability to embed fonts declared in @font-face rules into the resulting document’s font definitions has been introduced by adding a new [SupportFontFaceRules](https://reference.aspose.com/words/net/aspose.words.loading/htmlloadoptions/supportfontfacerules/) property.

#### Work with Glow and Reflection Formatting <sup>24.4</sup>

The ability to work with glow and reflection formatting for a drawing object has been implemented.

### Loading and Saving Documents

#### Specify SvgSaveOptions During Rendering <sup>24.2</sup>

The capability to specify [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/) during rendering has been added using the [ShapeRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) and [OfficeMathRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) methods.

#### Preserve Empty Lines when Loading Markdown files <sup>24.2</sup>

The ability to preserve empty lines when loading Markdown files has been added.

#### A New TIFF Reader/Writer <sup>24.3</sup>

A new TIFF reader/writer for Aspose.Words for .NET Standard, .NET 6 and later has been developed. Aspose.Words for .NET 24.3 added support for reading TIFF images with JPEG and Old JPEG compression types, and also significantly improved the quality of read and write operations.

### Other

* The capability to modify the text of the `TextBox` OLE control has been introduced by adding a new [Text](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/text/) property to the new [TextBoxControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/) class. <sup>24.1</sup>
* The Bibliography Sources public API was implemented through the adding a new namespace [Aspose.Words.Bibliography](https://reference.aspose.com/words/net/aspose.words.bibliography/) with its new classes and enumerations, and through the adding a new [Bibliography](https://reference.aspose.com/words/net/aspose.words/document/bibliography/) property to the [Document](https://reference.aspose.com/words/net/aspose.words/document/) class. <sup>24.1</sup>
* An API to limit access to type members using template syntax for the `LINQ Reporting Engine` has been provided. <sup>24.1</sup>
* New public properties [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/), and [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) for enhanced style management have been added to the [Style](https://reference.aspose.com/words/net/aspose.words/style/) class. <sup>24.2</sup>
* The functionality to retrieve the actual reference mark text for footnotes and endnotes has been enhanced with the [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) property and the [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/) method. <sup>24.2</sup>
* Compatibility with `Word 2016` charts for the `LINQ Reporting Engine` has been enabled. <sup>24.2</sup>
* Emulation of binary raster operations for WMF metafiles has been implemented. <sup>24.3</sup>
* The capability to define signature options for documents within **SaveOptions** has been enabled by adding a new [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/digitalsignaturedetails/) class with new public members, as well as adding new properties to the [OoxmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/docsaveoptions/) and [OdtSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/odtsaveoptions/) classes. <sup>24.4</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for .NET 24.1 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-1-release-notes/).

Learn more about [Aspose.Words for .NET 24.2 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-2-release-notes/).

Learn more about [Aspose.Words for .NET 24.3 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-3-release-notes/).

Learn more about [Aspose.Words for .NET 24.4 Release Notes](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words for .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 expands rendering options, metafile rendering emulation, and markdown save options.

Aspose.Words 23.10 improves rendering, expands options for loading and saving documents, and allows users to merge documents in new ways.

Aspose.Words 23.11 enhances the work with revisions, XLSX format and fonts on chart legend with additional options.

Aspose.Words 23.12 introduces new properties and enumerations for working with PDF and OOXML documents, as well as support for WebP images.

### Rendering and Printing

#### Customizing Axes Titles in DrawingML Charts <sup>23.9</sup>

The capability to customize axis titles in DrawingML charts has been introduced by the implementation of a new public class [ChartAxisTitle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxistitle/) and [Title](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxis/title/) property.

#### Determining the Vertical Position of Fonts within a Paragraph <sup>23.9</sup>

It is now possible to define the vertical position of fonts within a paragraph using the new public [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/paragraphformat/baselinealignment/) property and the new [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/baselinealignment/) enumeration.

#### Foreground Color Control <sup>23.10</sup>

The ability to retrieve the foreground color without modifiers has been added to the [Fill](https://reference.aspose.com/words/net/aspose.words.drawing/fill/) and [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) classes via the **BaseForeColor** property.

#### Expanding the Functionality of Charts <sup>23.10</sup>

The functionality of the [ChartDataPointCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseries/), and [ChartFormat](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartformat/) classes has been expanded with new methods and properties.

#### Automatically Adjust and Fit an Image into a Shape <sup>23.10</sup>

A simple way to automatically adjust and fit an image within a particular shape has been provided through the new [FitImageToShape](https://reference.aspose.com/words/net/aspose.words.drawing/imagedata/fitimagetoshape/) method.

#### Default Font Formatting for DrawingML Chart Legend Entries <sup>23.11</sup>

The ability to specify default font formatting for legend entries of DrawingML charts has been added via the [Font](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartlegend/font/) property. This feature facilitates a more streamlined and consistent appearance for chart elements, improving the overall document aesthetics.

#### Specify Page Layout when Opening PDF in Reader <sup>23.12</sup>

The ability to specify the page layout to be used when opening a document in a PDF reader has been added through the introduction of a new [PageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/pagelayout/) property to the [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) class and the introduction of a new [PdfPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfpagelayout/) enumeration.

### Loading and Saving Documents

#### Specifying a Folder Name to Construct Image URIs in Markdown <sup>23.9</sup>

The [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) class has been expanded by including the [ImagesFolderAlias](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imagesfolderalias/) property, which allows to specifies the name of the folder used to construct image URIs written into the Markdown document.

#### Reduce PDF Output Size <sup>23.10</sup>

Various PDF rendering optimizations to reduce output size when utilizing [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) settings have been implemented.

#### Recognize Hyperlinks when Loading TXT Documents <sup>23.10</sup>

The feature to recognize hyperlinks when loading TXT documents has been implemented by adding a new [DetectHyperlinks](https://reference.aspose.com/words/net/aspose.words.loading/txtloadoptions/detecthyperlinks/) property.

### Other

* Metafile rendering emulation to determine rasterization size has been implemented, specifically for WMF pen width and EMF cosmetic pen width. To achieve this, the **ScaleWmfFontsToMetafileSize** property was replaced with the [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpage/) property and the [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpageresolution/) property was added. <sup>23.9</sup>
* A simplified method for inserting one document into another document at the current cursor position has been introduced using the [InsertDocumentInline](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertdocumentinline/) method. <sup>23.10</sup>
* The ability to access and modify style properties has been added through the introduction of the new [Locked](https://reference.aspose.com/words/net/aspose.words/style/locked/) property.  <sup>23.10</sup>
* A generic type parameter has been added to the methods of the [CompositeNode](https://reference.aspose.com/words/net/aspose.words/compositenode/) class. <sup>23.10</sup>
* A way to control when a certain revision should be accepted/rejected or not has been implemented by using the [Accept](https://reference.aspose.com/words/net/aspose.words/revisioncollection/accept/) and [Reject](https://reference.aspose.com/words/net/aspose.words/revisioncollection/reject/) methods. This enhancement grants users finer control over the revision process. <sup>23.11</sup>
* The ability to write all sections of a document onto the same XLSX worksheet has been provided through the new [XlsxSectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsectionmode/) enumeration type and the new [SectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsaveoptions/sectionmode/) property. <sup>23.11</sup>
* A way to control how ZIP64 format extensions will be used for OOXML documents has been implemented through the new Zip64Mode property of the `OoxmlSaveOptions` class and the new Zip64Mode enumeration. <sup>23.12</sup>
* Support for WebP image has been introduced. Please note that this feature is only available for .NetStandart and .NET6+ versions. <sup>23.12</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for .NET 23.9 Release Notes](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-9-release-notes/).

Learn more about [Aspose.Words for .NET 23.10 Release Notes](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-10-release-notes/).

Learn more about [Aspose.Words for .NET 23.11 Release Notes](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-11-release-notes/).

Learn more about [Aspose.Words for .NET 23.12 Release Notes](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-12-release-notes/).

{{% /alert %}}

## See Also

{{% alert color="primary" %}}

This page contains the latest release news for the past 2 years. For details on earlier releases, see the [Release Notes'](https://releases.aspose.com/words/net/release-notes/) pages in the relevant sections.

{{% /alert %}}
