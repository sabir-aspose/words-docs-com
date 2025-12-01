---
title: What's new
second_title: Aspose.Words for C++
articleTitle: What's new in Aspose.Words for C++
linktitle: What's new in Aspose.Words for C++
type: docs
description: "Aspose.Words for C++ expands and enhances daily. On this page, you can learn about the huge and most interesting features of the product."
weight: 2
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cpp/what-s-new-in-aspose-words-for-cpp/
timestamp: 2025-12-01-11-12-25
---

This page describes the most interesting new Aspose.Words features introduced in recent releases.

## Aspose.Words for C++ 25.9, 25.10, 25.11

Aspose.Words 25.9 enhances document loading reliability, expands shape and text formatting, improves Markdown export with math support, and strengthens font handling diagnostics.

Aspose.Words 25.10 introduces enhancements to text and PDF exports, improves accessibility compliance, and adds new options for resource management during Markdown export.

Aspose.Words 25.11 expands AI integration capabilities, enhances Markdown export, and introduces advanced control over print operations.

### AI-powered Features

#### Сonfigure AI Model Service Endpoints <sup>25.11</sup>

The ability to configure [AI model](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodel/) service endpoints has been introduced by adding support for specifying **custom URLs** and **request timeouts**, allowing greater flexibility in AI-powered integrations.

### Converting, Loading, and Saving Documents

#### Control How Corrupted Documents Are Opened <sup>25.9</sup>

The ability to control how corrupted documents are opened has been introduced by adding a new **RecoveryMode** option.

#### Export Mathematical Equations to LaTeX Expression <sup>25.9</sup>

The ability to export mathematical equations (Office Math) to LaTeX expressions has been introduced:

* For export to Markdown format using the [MarkdownSaveOptions.OfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_officemathexportmode/) property. <sup>25.9</sup>
* For export to TXT format using the **TxtSaveOptions.OfficeMathExportMode** property. <sup>25.10</sup>

#### Improved Document Conversion Fidelity to Markdown <sup>25.11</sup>

The fidelity of document conversion to Markdown has been improved by enabling the [export of OfficeMath objects](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownofficemathexportmode/) into LaTeX format, ensuring compatibility with MarkItDown renderers.

#### Control Floating Shape Tagging When Exporting to PDF <sup>25.10</sup>

A new save option **ExportFloatingShapesAsInlineTag** has been added to provide precise control over the tagging of floating shapes as either inline or block-level elements, improving layout accuracy and accessibility.

#### Control How Images and Other External Resources are Exported to Markdown <sup>25.10</sup>

A new **resource-saving callback** has been implemented to give developers greater flexibility in controlling how images and other external resources are exported.

#### PDF/UA Export & Accessibility <sup>25.10</sup>

Compliance with PDF/UA standards has been improved by correctly tagging horizontal rules as artifacts, enhancing a better experience for users of assistive technologies.

### Rendering

#### Fine-tune Shadow Effects <sup>25.9</sup>

The ability to fine-tune [shadow effects](https://reference.aspose.com/words/cpp/aspose.words.drawing/shadowformat/) has been enhanced by introducing new public properties.

#### Improve Diagnostics for Font Substitution <sup>25.9</sup>
The ability to improve diagnostics and error handling for **font substitution** has been implemented by adding typed warnings.

### Other

* new advanced print control options have been added: <sup>25.11</sup>

    * **A new callback interface**, similar to `IWarningCallback`, has been introduced to allow programmatic control over page skipping during print operations.
    * A new public property has been added to accurately **retrieve the actual number of pages** rendered by a print job.
    * The ability to specify distinct target printers for **color and monochrome** (black & white) pages within a single print job has also been introduced.

{{% alert color="primary" %}}

Learn more about [Aspose.Words for C++ 25.9 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-9-release-notes/).

Learn more about [Aspose.Words for C++ 25.10 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-10-release-notes/).

Learn more about [Aspose.Words for C++ 25.11 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-11-release-notes/).

{{% /alert %}}

## Aspose.Words for C++ 25.5, 25.6, 25.7, 25.8

Aspose.Words 25.5 enhances chart customization with new styling options and improves Markdown export by offering control over how empty paragraphs are handled.

Aspose.Words 25.6 enhances rendering precision and visualization features by introducing advanced image export options, improved MathML handling, and better chart representation.

Aspose.Words 25.7 introduces AI enhancements with support for self-hosted LLMs, more precise control during text replacement, flexible table row visibility, and richer typography with OpenType Font Variations.

Aspose.Words 25.8 expands capabilities for Markdown import/export, enhances Find and Replace with an option to ignore Office Math objects, and provides greater control over page extraction.

### AI-powered Features

#### Integrating a Self-Hosted LLM <sup>25.7</sup>

The ability to integrate and use self-hosted LLM (Large Language Model) has been introduced, providing greater privacy and control over AI-powered document features.

### Converting, Loading, and Saving Documents

#### Export Empty Paragraphs to Markdown <sup>25.5</sup>

The ability to control how empty paragraphs are exported to Markdown has been introduced by adding the [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownemptyparagraphexportmode/) enumeration and the [EmptyParagraphExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_emptyparagraphexportmode/) property.

#### Export Multi-page Documents to Raster Image Formats <sup>25.6</sup>

The ability to export multi-page documents to raster image formats (such as PNG and JPEG) with [customizable layouts](https://reference.aspose.com/words/cpp/aspose.words.saving/multipagelayout/) – Horizontal, Vertical, or Grid – has been introduced by extending image export functionality.

#### Export Non-compatible Tables to Raw HTML <sup>25.8</sup>

The ability to control how non-compatible tables are rendered when exporting to raw HTML has been introduced by adding the new [MarkdownExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownexportashtml/) enumeration.

#### Specify Character for Soft Line Breaks When Importing to Markdown <sup>25.8</sup>

The ability to specify a character for soft line breaks when importing to Markdown has been introduced by adding the new **SoftLineBreakCharacter** property.

### Rendering

#### Setting the Chart Style <sup>25.5</sup>

The ability to set the chart style has been introduced by adding the [ChartStyle](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartstyle/) enumeration and the [Style](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chart/get_style/) property.

#### Rendering Connector Lines in MathML Expressions <sup>25.6</sup>

The rendering of connector lines in MathML expressions has been implemented to ensure more accurate and visually consistent display of mathematical formulas.

#### Rendering Legends for Waterfall Charts <sup>25.6</sup>

The rendering of legends for ["Waterfall" charts](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartseriestype/) has been introduced, increasing data transparency and improving the interpretability of these charts.

#### Support for OpenType Font Variations <sup>25.7</sup>

Initial support for OpenType Font Variations has been implemented, allowing for more flexible and expressive typographic rendering.

### Other

* The ability to wrap mathematical formulas containing multiple slashes has been enhanced, improving layout clarity and formula legibility. <sup>25.6</sup>
* A new [ReplacingArgs.MatchEndNode](https://reference.aspose.com/words/cpp/aspose.words.replacing/replacingargs/get_matchendnode/) property has been added to enable more precise control during text replacement operations across document content. <sup>25.7</sup>
* The ability to programmatically show or hide specific table rows has been introduced by adding the [Row.Hidden](https://reference.aspose.com/words/cpp/aspose.words.tables/row/get_hidden/) property. <sup>25.7</sup>
* A new **IgnoreOfficeMath** property has been added to ignore Office Math objects when searching and replacing. <sup>25.8</sup>
* New options have been added to the **PageExtractOptions** class to provide more control over the page extraction process. <sup>25.8</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for C++ 25.5 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-5-release-notes/).

Learn more about [Aspose.Words for C++ 25.6 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-6-release-notes/).

Learn more about [Aspose.Words for C++ 25.7 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-7-release-notes/).

Learn more about [Aspose.Words for C++ 25.8 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-8-release-notes/).

{{% /alert %}}

## Aspose.Words for C++ 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 introduces AI-powered grammar checking and enhances document saving with advanced options for HTML, SVG, and Markdown formats.

Aspose.Words 25.2 introduces text summarization with Anthropic AI models, adds MsWorks format support, enhances typographic control, and improves PDF structure and list handling.

Aspose.Words 25.3 enhances an AI-powered grammar checker and font selection with the UpdateAmbiguousTextFont property, as well as improves PDF attachments export.

Aspose.Words 25.4 introduces support for new paper sizes, enables advanced HTML export control, improves watermark handling, and enhances the usability of the LowCode API.

### AI-powered Features

#### Document AI Grammar Checking

* The ability to check the grammar of the provided document using OpenAI generative models has been introduced by adding a new [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/) method. <sup>25.1</sup>
* The AI-powered Grammar Checking feature has been updated to support all models available in the [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/) enumeration. <sup>25.3</sup>

#### Summarization Using Anthropic Generative Language Models <sup>25.2</sup>

Text summarization using Anthropic generative language models has been enabled by introducing a new public class [AnthropicAiModel](https://reference.aspose.com/words/cpp/aspose.words.ai/).

### Low Code

#### Low Code API Usability <sup>25.4</sup>

Significant improvements to the usability of the **LowCode API** have been introduced, simplifying document processing and reducing the need for repetitive code.

### Supported Formats <sup>25.2</sup>

Starting from version 25.2, compatibility with the new MsWorks load format for Microsoft Works documents has been added.

### Converting, Loading, and Saving Documents

#### Improved Saving to HTML and SVG Formats <sup>25.1</sup>

Saving to HTML and SVG formats has been enhanced by adding **IdPrefix** and **RemoveJavaScriptFromLinks** properties to both the [HtmlFixedSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlfixedsaveoptions/) and [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/) classes.

#### Set Image Resolution and OfficeMath Output Mode When Saving to Markdown <sup>25.1</sup>

- A new [ImageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imageresolution/) option has been added to the [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) class to set the image resolution.
- A new [OfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_officemathexportmode/) option and [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownofficemathexportmode/) enumeration have been and added to the [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) class to set OfficeMath output mode.
- The ability to set an image watermark from a stream has been introduced by adding a new overload to the [SetImage](https://reference.aspose.com/words/cpp/aspose.words/watermark/setimage/#watermarksetimageconst-systemsharedptrsystemiostream-const-systemsharedptrasposewordsimagewatermarkoptions-method) method. <sup>25.4</sup>

### Rendering

#### Improved Typographic Control <sup>25.2</sup>

The [NumberSpacing](https://reference.aspose.com/words/cpp/aspose.words/font/get_numberspacing/) property has been added for improved typographic control.

#### Controlling Font Selection for Ambiguous Characters <sup>25.3</sup>

A new public property [UpdateAmbiguousTextFont](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/get_updateambiguoustextfont/) has been added to the [SaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/) class to control the font selection according to the character code used.

#### Paper Size Options <sup>25.4</sup>

The ability to use JIS B4 and JIS B5 paper sizes has been introduced by adding new values to the [PaperSize](https://reference.aspose.com/words/cpp/aspose.words/papersize/) enumeration.

#### HTML Output Control <sup>25.4</sup>

The ability to remove JavaScript from hyperlink URLs during HTML export has been introduced by adding the [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlsaveoptions/get_removejavascriptfromlinks/) property.

### Other

* PDF logical structure has been improved with support for TOA, BIBLIOGRAPHY, and INDEX fields. <sup>25.2</sup>
* The [AddSingleLevelList](https://reference.aspose.com/words/cpp/aspose.words.lists/listcollection/addsinglelevellist/) method has been introduced for improved list handling. <sup>25.2</sup>
* A new property [AttachmentsEmbeddingMode](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/get_attachmentsembeddingmode/) has been added to replace **EmbedAttachments** to improve PDF attachments' export. Also, new values have been added to the [PdfCompliance](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfcompliance/) enumeration to support PDF/A version attachments. Additionally, attachments are now supported with encryption. <sup>25.3</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for C++ 25.1 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-1-release-notes/).

Learn more about [Aspose.Words for C++ 25.2 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-2-release-notes/).

Learn more about [Aspose.Words for C++ 25.3 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-3-release-notes/).

Learn more about [Aspose.Words for C++ 25.4 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words for C++ 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduces group shape insertion and StructuredDocumentTag insertion via DocumentBuilder, enhances radial chart rendering with graduations, improves digital signatures with XAdES-EPES support, adds Markdown underline recognition, and provides access to footnote/endnote separators.

Aspose.Words 24.10 introduces enhanced ActiveX control support with CommandButton creation, new shape visibility control, the ability to group shapes, improved Markdown export for tables, chart formatting for Pie and Doughnut charts, better Big5 encoding handling, and support for outdated Taiwanese fonts.

Aspose.Words 24.11 introduces AI-powered document summarization, enhanced rendering options, improved access to document properties and ActiveX control captioning.

Aspose.Words 24.12 introduces customizable data label placement, Google AI-powered text translation, enhanced Mail Merge cleanup options, and new LowCode processing classes.

### AI-powered Features

#### Document Summarization Using OpenAI and Google <sup>24.11</sup>

Support for document summarization using **OpenAI** and **Google** generative language models has been integrated.

#### Text translation using Google's generative language models <sup>24.12</sup>

The ability to translate text using Google's generative language models has been implemented in Aspose.Words by adding the [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) method and the [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) enumeration to the [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) namespace.

### Low Code <sup>24.12</sup>

New LowCode classes like [Comparer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/cpp/aspose.words.lowcode/merger/), [Replacer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/cpp/aspose.words.lowcode/splitter/) etc. has been introduced, offering a set of methods that strike the perfect balance between simplicity and flexibility for document processing.

### Rendering and Printing

#### Graduations on Radial Charts <sup>24.9</sup>

Rendering of graduations on radial charts has been implemented.

#### CommandButton ActiveX Controls <sup>24.10</sup>

The ability to create CommandButton ActiveX controls has been introduced by adding a new public method [InsertForms2OleControl](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertforms2olecontrol/) and a new public class **Forms2OleControl**.

#### Control Shape Visibility <sup>24.10</sup>

A new public property [Hidden](https://reference.aspose.com/words/cpp/aspose.words.drawing/shapebase/get_hidden/) has been added to control the visibility of shapes.

#### Changes in Pie and Doughnut Charts <sup>24.10</sup>

Several new public properties have been added to format Pie and Doughnut charts.

#### Control the Rendering of PDF Choice Form Field Borders <sup>24.11</sup>

A new option to control the rendering of PDF choice form field borders has been implemented by adding a new public option **RenderChoiceFormFieldBorder**.

#### Get and Set Format Codes for Chart Data <sup>24.11</sup>

The ability to get and set format codes for chart data has been added by implementing the **FormatCode** property in the [ChartXValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartyvaluecollection/) and [BubbleSizeCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/bubblesizecollection/) classes.

#### Render Histogram Charts with Bins and Labels <sup>24.11</sup>

Histogram chart rendering has been improved by allowing for a specified number of bins and labels.

#### Customize the Placement of Data Labels <sup>24.12</sup>

The ability to customize the placement of data labels has been added by introducing new properties to the [ChartDataLabel](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabel/) and [ChartDataLabelCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabelcollection/) classes.

### Converting, Loading and Saving Documents

#### Underline Formatting when Loading Markdown Files <sup>24.9</sup>

The option to recognize underline formatting when loading Markdown documents has been incorporated by adding a new public property **ImportUnderlineFormatting**.

#### Exporting tables as HTML when saving to Markdown <sup>24.10</sup>

An option to export tables as HTML when saving documents to Markdown format has been implemented by adding a new public property [ExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_exportashtml/) and an enumeration [MarkdownExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownexportashtml/).

#### Export PDF with Updated Logical Structure <sup>24.11</sup>

PDF export has been enhanced by including table title properties as PDF logical structure element titles.

### Mail Merge and Reporting

#### Remove Empty Tables during Mail Merge <sup>24.12</sup>

A new **RemoveEmptyTables** option has been added to the [MailMergeCleanupOptions](https://reference.aspose.com/words/cpp/aspose.words.mailmerging/mailmergecleanupoptions/) enumeration to refine Mail Merge output.

### Digital Signatures

#### Sign Documents with XAdES-EPES <sup>24.9</sup>

The ability to sign documents with XAdES-EPES level XML-DSig signatures has been introdused by adding a new public property **XmlDsigLevel** and a new public enumeration **XmlDsigLevel**.

### Other

* A new public method [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/) has been added to group shapes. <sup>24.9</sup>
* A new public method [InsertStructuredDocumentTag](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertstructureddocumenttag/) has been added to insert **StructuredDocumentTags** into a document. <sup>24.9</sup>
* Public access to footnote/endnote separators has been provided by adding a few public classes and properties. <sup>24.9</sup>
* The ability to group individual shapes, group shapes together, and directly group both shapes and group shapes has been introduced by adding the [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/) method. <sup>24.10</sup>
* Big5 encoding handling for TrueType cmap tables has been improved. <sup>24.10</sup>
* Support for outdated Taiwanese fonts has been enhanced. <sup>24.10</sup>
* To access extended document properties, read-only properties have been added to the **BuiltInDocumentProperties** class. <sup>24.11</sup>
* Setting captions for ActiveX controls has been enabled by adding a new public setter to the **Forms2OleControl.Caption** property. <sup>24.11</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for C++ 24.9 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-9-release-notes/).

Learn more about [Aspose.Words for C++ 24.10 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-10-release-notes/).

Learn more about [Aspose.Words for C++ 24.11 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-11-release-notes/).

Learn more about [Aspose.Words for C++ 24.12 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words for C++ 24.5, 24.6, 24.7

Aspose.Words 24.5 expands options for assemblies, improves rendering capabilities, and expands some other options.

Aspose.Words 24.6 improves rendering options, enhances search and compare functionality, and expands several other features.

Aspose.Words 24.7 changes how you work with ActiveX, expands rendering capabilities, as well as exporting to Markdown and XLSX formats.

### Supported Formats

Starting from version 24.7, export to PDF/UA-2 is supported to ensure accessibility for users with disabilities.

### Rendering and Printing

#### Changes in Charts, Shapes and DrawingML <sup>24.5</sup>

- DrawingML effects rendering for SVG graphics, extending previous functionality limited to images, has been implemented.
- Support for creating combo charts and adjusting properties such as gap width, overlap, and bubble scale within series groups has been introduced by adding the **ChartSeriesGroup** and **ChartSeriesGroupCollection** classes and the **SeriesGroups** property.
- Functionality to manipulate the SoftEdge effect of shapes has been implemented by adding the **SoftEdgeFormat** class.
- The ability to modify adjust values of shapes has been implemented by adding the **AdjustmentCollection** and **Adjustment** public classes and **Adjustments** property.

#### Changes in Charts, Shapes and Drawing <sup>24.6</sup>

- Charting capabilities have been enhanced. You can now create a wider variety of charts, including *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* charts, *Box & Whisker* charts, *Waterfalls*, and *Funnels*. This allows you to visualize your data in a more diverse and informative way.
- Color control for shadow formatting has been improved. You can gain more precise control over the appearance of your documents by accessing shadow colors.
- Performance boost for background rendering has been improved. You can significantly speed up the rendering of backgrounds containing small elements thanks to native tiling technology.
- Realistic gradients for shapes have been added. You can now create DML shapes with non-linear gradients, mimicking the visual style of Microsoft Word for a more polished look.

#### Chart Data Label Customization <sup>24.7</sup>

The ability to customize chart data labels such as **Orientation** and **Rotation** has been added.

#### Custom Number Styling for List Levels <sup>24.7</sup>

A setter for the public property [CustomNumberStyleFormat](https://reference.aspose.com/words/cpp/aspose.words.lists/listlevel/get_customnumberstyleformat/) has been added. You can now define a custom number styling for list levels.

#### Changes in working with ActiveX <sup>24.7</sup>

- The properties of ActiveX objects can now be modified, giving you more control over their behavior.
- The ability to modify the value of the radio button ActiveX control to enable dynamic interaction has been added.
- The ability to toggle an ActiveX checkbox to "checked" or "unchecked" has been added.

### Loading and Saving Documents

#### Exporting Links to Markdown Format <sup>24.7</sup>

The ability to control the export of links in Markdown format has been added through the implementation of the [LinkExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_linkexportmode/) property.

### Search and Compare

#### Advanced Comparison Options <sup>24.6</sup>

The ability to streamline data analysis workflows with improved comparison functionality has been added. This includes a new **IgnoreStoreItemId** option and a redesigned interface for advanced comparisons.

### Other

- The function to eliminate empty pages from a document has been implemented by adding the [RemoveBlankPages](https://reference.aspose.com/words/cpp/aspose.words/document/removeblankpages/) method. <sup>24.5</sup>
- The ability  to check for the presence of VBA macros without loading a document has been provided by adding the **HasMacros** property. <sup>24.5</sup>
- A new **DateTimeUtc** property has been added – this provides a more precise timestamp for comments, improving organization and traceability. <sup>24.6</sup>
- The datetime format is now automatically detected for seamless export to XLSX format. <sup>24.7</sup>
- The public property [IsProtected](https://reference.aspose.com/words/cpp/aspose.words.vba/vbaproject/get_isprotected/), which allows you to verify whether a VBA project is protected, has been added. <sup>24.7</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for C++ 24.5 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-5-release-notes/).

Learn more about [Aspose.Words for C++ 24.6 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-6-release-notes/).

Learn more about [Aspose.Words for C++ 24.7 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-7-release-notes/).

{{% /alert %}}

## Aspose.Words for C++ 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 improves the experience around managing stroke colors, enhances OLE objects, as well as introduces a new Bibliography Sources public API.

Aspose.Words 24.2 expanded Charts API and style management. This version of Aspose.Words also introduced the capability to specify SvgSaveOptions during rendering, more flexible control loading Markdown files, and working with reference text for footnotes and endnotes.

Aspose.Words 24.3 introduces Emulation of binary raster operations for WMF metafiles and also continues to expand the Charts API.

Aspose.Words 24.4 enhances some rendering options, as well as improves work with digital signatures.

### Rendering and Printing

#### Stroke Color Control <sup>24.1</sup>

The [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) class has been extended with a set of new public properties related to managing stroke colors: [ForeThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_forethemecolor/) and [BackThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_foretintandshade/) and [BackTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backtintandshade/).

#### DrawingML Charts API Extension <sup>24.2 / 24.3 / 24.4</sup>

The **DrawingML Charts API** continues to be expanded.

#### Embed Fonts Declared in @font-face Rules <sup>24.4</sup>

Added an ability to embed fonts declared in @font-face rules into the resulting document’s font definitions has been introduced by adding a new [SupportFontFaceRules](https://reference.aspose.com/words/cpp/aspose.words.loading/htmlloadoptions/get_supportfontfacerules/) property.

#### Work with Glow and Reflection Formatting <sup>24.4</sup>

The ability to work with glow and reflection formatting for a drawing object has been implemented.

### Loading and Saving Documents

#### Specify SvgSaveOptions During Rendering <sup>24.2</sup>

The capability to specify [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/) during rendering has been added using the [ShapeRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) and [OfficeMathRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) methods.

#### Preserve Empty Lines when Loading Markdown files <sup>24.2</sup>

The ability to preserve empty lines when loading Markdown files has been added.

### Other

- The capability to modify the text of the `TextBox` OLE control has been introduced by adding a new **Text** property to the new **TextBoxControl** class. <sup>24.1</sup>
- The Bibliography Sources public API was implemented through the adding a new namespace [Aspose.Words.Bibliography](https://reference.aspose.com/words/cpp/aspose.words.bibliography/) with its new classes and enumerations, and through the adding a new [Bibliography](https://reference.aspose.com/words/cpp/aspose.words/document/get_bibliography/) property to the [Document](https://reference.aspose.com/words/cpp/aspose.words/document/) class. <sup>24.1</sup>
- New public properties [Priority](https://reference.aspose.com/words/cpp/aspose.words/style/get_priority/), [UnhideWhenUsed](https://reference.aspose.com/words/cpp/aspose.words/style/get_unhidewhenused/), and [SemiHidden](https://reference.aspose.com/words/cpp/aspose.words/style/get_semihidden/) for enhanced style management have been added to the [Style](https://reference.aspose.com/words/cpp/aspose.words/style/) class. <sup>24.2</sup>
- The functionality to retrieve the actual reference mark text for footnotes and endnotes has been enhanced with the [ActualReferenceMark](https://reference.aspose.com/words/cpp/aspose.words.notes/footnote/get_actualreferencemark/) property and the [UpdateActualReferenceMarks](https://reference.aspose.com/words/cpp/aspose.words/document/updateactualreferencemarks/) method. <sup>24.2</sup>
- Emulation of binary raster operations for WMF metafiles has been implemented. <sup>24.3</sup>
- The capability to define signature options for documents within **SaveOptions** has been enabled by adding a new **DigitalSignatureDetails** class with new public members, as well as adding new properties to the [OoxmlSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/docsaveoptions/) and [OdtSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/odtsaveoptions/) classes. <sup>24.4</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for C++ 24.1 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-1-release-notes/).

Learn more about [Aspose.Words for C++ 24.2 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-2-release-notes/).

Learn more about [Aspose.Words for C++ 24.3 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-3-release-notes/).

Learn more about [Aspose.Words for C++ 24.4 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-4-release-notes/).

{{% /alert %}}

## See Also

{{% alert color="primary" %}}

This page contains the latest release news for the past 2 years. For details on earlier releases, see the [Release Notes'](https://releases.aspose.com/words/cpp/release-notes/) pages in the relevant sections.

{{% /alert %}}
