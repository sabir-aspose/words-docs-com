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
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/what-s-new-in-aspose-words-for-net/
timestamp: 2026-04-15-11-12-25
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page explains what’s new in recent Aspose.Words for .NET releases.

{{% /alert %}}

This page describes the most interesting new Aspose.Words features introduced in recent releases.

## Aspose.Words for .NET 26.1, 26.2, 26.3, 26.4

Aspose.Words 26.1 expands platform support with .NET 10.0, introduces Docling JSON export, enhances AI and document merging capabilities, and significantly improves PDF compliance, accessibility, and rendering accuracy for fields and mathematical equations.

Aspose.Words 26.2 improves chart customization, enhances the visual quality of mathematical equations, and aligns table layout behavior more closely with modern Microsoft Word rendering logic.

Aspose.Words for .NET 26.3 introduces improvements to AI integration, enhances document optimization capabilities, and updates font fallback handling for improved rendering of CJK Unified Ideographs Extension G range.

Aspose.Words 26.4 introduces improvements in PDF export, chart rendering capabilities, and reporting engine diagnostics, enhancing document structure fidelity, visualization accuracy, and debugging experience.

### AI-powered Features

#### Direct Instantiation of Google AI Models <sup>26.1</sup>

The ability to work directly with Google AI models has been introduced by enabling [direct instantiation of the GoogleAiModel class](https://reference.aspose.com/words/net/aspose.words.ai/googleaimodel/googleaimodel/) in the **Aspose.Words.AI** namespace.

#### Improved OpenAiModel Capabilities <sup>26.3</sup>

The ability to create an instance of the [OpenAiModel](https://reference.aspose.com/words/net/aspose.words.ai/openaimodel/) class directly has been introduced, simplifying the integration of OpenAI-based AI features into document processing workflows.

### Supported Formats

#### New Docling JSON Export Format <sup>26.1</sup>

The ability to export documents to the **Docling JSON format** has been introduced.

### Platforms

#### Support for the .NET 10.0 Target Framework <sup>26.1</sup>

The ability to target the **.NET 10.0 framework** has been introduced by providing a dedicated Aspose.Words build.

### Converting, Loading, and Saving Documents

#### PDF AcroForm Tagging <sup>26.1</sup>

The ability to improve PDF accessibility has been introduced by adding support for tagging **PDF AcroForms**, making exported documents more accessible to assistive technologies.

#### Improved PDF Logical Structure <sup>26.4</sup>

The ability to improve PDF logical structure by exporting node custom IDs to custom attributes during PDF export has been introduced.

### Rendering

#### Extended PDF Conformance Standards <sup>26.1</sup>

The **PdfSaveOptions** functionality has been extended by the [PreserveFormFields](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/preserveformfields/) property to be compatible with all PDF compliance standards (including PDF/A and PDF/UA).

#### Rendering MathML using an East Asian Font <sup>26.1</sup>

The ability to correctly render **MathML** content with **East Asian characters** has been introduced, while preserving Latin and Hebrew text when an East Asian font is specified.

#### EQ-matrix MathML Elements Rendering <sup>26.2</sup>

The rendering of EQ-matrix MathML elements has been improved to achieve higher visual fidelity in mathematical content.

#### Orientation And Rotation of Chart Titles and Axis Titles <sup>26.2</sup>

The ability to control the [orientation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/charttitle/orientation/) and [rotation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/charttitle/rotation/) of chart titles and axis titles has been introduced, allowing more flexible and precise chart layout customization.

#### Font Fallback Table for CJK Unified Ideographs Extension G range <sup>26.3</sup>

Rendering accuracy has been improved by updating the Microsoft Office font fallback table for the CJK Unified Ideographs Extension G range, ensuring more reliable font substitution when rendering documents containing these characters.

#### Enhanced Chart Rendering <sup>26.4</sup>

The ability to enhance chart rendering has been introduced by adding support for funnel chart [data labels](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/), applying chart style settings to leader line rendering, and using locale IDs when rendering default axis titles in DrawingML charts.

### Other

* The handling of adjacent tables has been updated by implementing the latest Microsoft Word logic for merging or separating tables during layout processing. <sup>26.2</sup>
* The document optimization capabilities have been improved by extending the [JoinRunsWithSameFormatting](https://reference.aspose.com/words/net/aspose.words/document/joinrunswithsameformatting/) method, enabling more comprehensive content merging. <sup>26.3</sup>
* The ability to improve report generation diagnostics in LINQ Reporting Engine has been introduced by providing detailed error information during the report building stage. <sup>26.4</sup>

{{% alert color="primary" %}}

Learn more about [Aspose.Words for .NET 26.1 Release Notes](https://releases.aspose.com/words/net/release-notes/2026/aspose-words-for-net-26-1-release-notes/).

Learn more about [Aspose.Words for .NET 26.2 Release Notes](https://releases.aspose.com/words/net/release-notes/2026/aspose-words-for-net-26-2-release-notes/).

Learn more about [Aspose.Words for .NET 26.3 Release Notes](https://releases.aspose.com/words/net/release-notes/2026/aspose-words-for-net-26-3-release-notes/).

Learn more about [Aspose.Words for .NET 26.4 Release Notes](https://releases.aspose.com/words/net/release-notes/2026/aspose-words-for-net-26-4-release-notes/).

{{% /alert %}}

## Aspose.Words for .NET 25.9, 25.10, 25.11, 25.12

Aspose.Words 25.9 enhances document loading reliability, expands shape and text formatting, improves Markdown export with math support, and strengthens font handling diagnostics.

Aspose.Words 25.10 introduces enhancements to text and PDF exports, improves accessibility compliance, and adds new options for resource management during Markdown export.

Aspose.Words 25.11 expands AI integration capabilities, enhances Markdown export, and introduces advanced control over print operations.

Aspose.Words 25.12 improves rendering accuracy across PDF, HTML-Fixed, and SVG formats, adds support for Variable Fonts and Funnel charts, and enhances text orientation handling in field rendering.

### AI-powered Features

#### Сonfigure AI Model Service Endpoints <sup>25.11</sup>

The ability to configure [AI model](https://reference.aspose.com/words/net/aspose.words.ai/aimodel/) service endpoints has been introduced by adding support for specifying [custom URLs](https://reference.aspose.com/words/net/aspose.words.ai/aimodel/url/) and [request timeouts](https://reference.aspose.com/words/net/aspose.words.ai/aimodel/timeout/), allowing greater flexibility in AI-powered integrations.

### Converting, Loading, and Saving Documents

#### Control How Corrupted Documents Are Opened <sup>25.9</sup>

The ability to control how corrupted documents are opened has been introduced by adding a new [RecoveryMode](https://reference.aspose.com/words/net/aspose.words.loading/loadoptions/recoverymode/) option.

#### Export Mathematical Equations to LaTeX Expression

The ability to export mathematical equations (Office Math) to LaTeX expressions has been introduced:

* For export to Markdown format using the [MarkdownSaveOptions.OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/officemathexportmode/) property. <sup>25.9</sup>
* For export to TXT format using the [TxtSaveOptions.OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/txtsaveoptions/officemathexportmode/) property. <sup>25.10</sup>

#### Improved Document Conversion Fidelity to Markdown <sup>25.11</sup>

The fidelity of document conversion to Markdown has been improved by enabling the [export of OfficeMath objects](https://reference.aspose.com/words/net/aspose.words.saving/markdownofficemathexportmode/) into LaTeX format, ensuring compatibility with MarkItDown renderers.

#### Control Floating Shape Tagging When Exporting to PDF <sup>25.10</sup>

A new save option [ExportFloatingShapesAsInlineTag](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/exportfloatingshapesasinlinetag/) has been added to provide precise control over the tagging of floating shapes as either inline or block-level elements, improving layout accuracy and accessibility.

#### Control How Images and Other External Resources are Exported to Markdown <sup>25.10</sup>

A new [resource-saving callback](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/resourcesavingcallback/) has been implemented to give developers greater flexibility in controlling how images and other external resources are exported.

#### PDF/UA Export & Accessibility <sup>25.10</sup>

Compliance with PDF/UA standards has been improved by correctly tagging horizontal rules as artifacts, enhancing a better experience for users of assistive technologies.

#### Handle Relative Hyperlinks When Exporting to PDF <sup>25.12</sup>

The ability to correctly resolve and handle relative hyperlinks when exporting to PDF has been introduced by adding Base URI processing during document export.

### Rendering

#### Fine-tune Shadow Effects <sup>25.9</sup>

The ability to fine-tune [shadow effects](https://reference.aspose.com/words/net/aspose.words.drawing/shadowformat/) has been enhanced by introducing new public properties.

#### Improve Diagnostics for Font Substitution <sup>25.9</sup>
The ability to improve diagnostics and error handling for [font substitution](https://reference.aspose.com/words/net/aspose.words/fontsubstitutionwarninginfo/) has been implemented by adding typed warnings.

#### Support for Variable Fonts When Saving Documents to SVG and Html-Fixed <sup>25.12</sup>

Robust support for Variable Fonts when saving documents to SVG and Html-Fixed formats has been added, ensuring that different font variations (including weight, width, and other parameters) defined within a single font file render correctly.

#### Render Funnel Charts <sup>25.12</sup>

The ability to render Funnel charts in documents has been added.

#### Render VerticalFarEast and HorizontalRotatedFarEast Text Orientations in EQ-field <sup>25.12</sup>

The ability to render **VerticalFarEast** and **HorizontalRotatedFarEast** text orientations in EQ-field elements has been introduced.

### Other

* new advanced print control options have been added: <sup>25.11</sup>

    * [A new callback interface](https://reference.aspose.com/words/net/aspose.words.rendering/asposewordsprintdocument/), similar to `IWarningCallback`, has been introduced to allow programmatic control over page skipping during print operations.
    * A new public property has been added to accurately [retrieve the actual number of pages](https://reference.aspose.com/words/net/aspose.words.rendering/asposewordsprintdocument/totalpagesprinted/) rendered by a print job.
    * The ability to specify distinct target printers for [color and monochrome](https://reference.aspose.com/words/net/aspose.words.rendering/asposewordsprintdocument/colormode/) (black & white) pages within a single print job has also been introduced.

{{% alert color="primary" %}}

Learn more about [Aspose.Words for .NET 25.9 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-9-release-notes/).

Learn more about [Aspose.Words for .NET 25.10 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-10-release-notes/).

Learn more about [Aspose.Words for .NET 25.11 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-11-release-notes/).

Learn more about [Aspose.Words for .NET 25.12 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-12-release-notes/).

{{% /alert %}}

## Aspose.Words for .NET 25.5, 25.6, 25.7, 25.8

Aspose.Words 25.5 enhances chart customization with new styling options and improves Markdown export by offering control over how empty paragraphs are handled.

Aspose.Words 25.6 enhances rendering precision and visualization features by introducing advanced image export options, improved MathML handling, and better chart representation.

Aspose.Words 25.7 introduces AI enhancements with support for self-hosted LLMs, more precise control during text replacement, flexible table row visibility, and richer typography with OpenType Font Variations.

Aspose.Words 25.8 expands capabilities for Markdown import/export, enhances Find and Replace with an option to ignore Office Math objects, introduces print job page tracking, and provides greater control over page extraction.

### AI-powered Features

#### Integrating a Self-Hosted LLM <sup>25.7</sup>

The ability to integrate and use self-hosted LLM (Large Language Model) has been introduced, providing greater privacy and control over AI-powered document features.

### Converting, Loading, and Saving Documents

#### Export Empty Paragraphs to Markdown <sup>25.5</sup>

The ability to control how empty paragraphs are exported to Markdown has been introduced by adding the [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownemptyparagraphexportmode/) enumeration and the [EmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/emptyparagraphexportmode/) property.

#### Export Multi-page Documents to Raster Image Formats <sup>25.6</sup>

The ability to export multi-page documents to raster image formats (such as PNG and JPEG) with [customizable layouts](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) – Horizontal, Vertical, or Grid – has been introduced by extending image export functionality.

#### Export Non-compatible Tables to Raw HTML <sup>25.8</sup>

The ability to control how non-compatible tables are rendered when exporting to raw HTML has been introduced by adding the new [MarkdownExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownexportashtml/) enumeration.

#### Specify Character for Soft Line Breaks When Importing to Markdown <sup>25.8</sup>

The ability to specify a character for soft line breaks when importing to Markdown has been introduced by adding the new [SoftLineBreakCharacter](https://reference.aspose.com/words/net/aspose.words.loading/markdownloadoptions/softlinebreakcharacter/) property.

### Rendering

#### Setting the Chart Style <sup>25.5</sup>

The ability to set the chart style has been introduced by adding the [ChartStyle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartstyle/) enumeration and the [Style](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/style/) property.

#### Rendering Connector Lines in MathML Expressions <sup>25.6</sup>

The rendering of connector lines in MathML expressions has been implemented to ensure more accurate and visually consistent display of mathematical formulas.

#### Rendering Legends for Waterfall Charts <sup>25.6</sup>

The rendering of legends for ["Waterfall" charts](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriestype/) has been introduced, increasing data transparency and improving the interpretability of these charts.

#### Support for OpenType Font Variations <sup>25.7</sup>

Initial support for OpenType Font Variations has been implemented, allowing for more flexible and expressive typographic rendering.

### Other

* The ability to wrap mathematical formulas containing multiple slashes has been enhanced, improving layout clarity and formula legibility. <sup>25.6</sup>
* A new [ReplacingArgs.MatchEndNode](https://reference.aspose.com/words/net/aspose.words.replacing/replacingargs/matchendnode/) property has been added to enable more precise control during text replacement operations across document content. <sup>25.7</sup>
* The ability to programmatically show or hide specific table rows has been introduced by adding the [Row.Hidden](https://reference.aspose.com/words/net/aspose.words.tables/row/hidden/) property. <sup>25.7</sup>
* A new [IgnoreOfficeMath](https://reference.aspose.com/words/net/aspose.words.replacing/findreplaceoptions/ignoreofficemath/) property has been added to ignore Office Math objects when searching and replacing. <sup>25.8</sup>
* A new [PagesRemaining](https://reference.aspose.com/words/net/aspose.words.rendering/asposewordsprintdocument/pagesremaining/) property has been added to check the number of pages remaining in a print job. <sup>25.8</sup>
* New options have been added to the [PageExtractOptions](https://reference.aspose.com/words/net/aspose.words/pageextractoptions/) class to provide more control over the page extraction process. <sup>25.8</sup>


{{% alert color="primary" %}}

Learn more about [Aspose.Words for .NET 25.5 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-5-release-notes/).

Learn more about [Aspose.Words for .NET 25.6 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-6-release-notes/).

Learn more about [Aspose.Words for .NET 25.7 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-7-release-notes/).

Learn more about [Aspose.Words for .NET 25.8 Release Notes](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-8-release-notes/).

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

## See Also

{{% alert color="primary" %}}

This page contains the latest release news for the past 2 years. For details on earlier releases, see the [Release Notes'](https://releases.aspose.com/words/net/release-notes/) pages in the relevant sections.

{{% /alert %}}