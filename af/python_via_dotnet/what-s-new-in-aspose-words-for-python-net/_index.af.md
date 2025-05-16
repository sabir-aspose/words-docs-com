---
title: Wat is nuut
second_title: Aspose.Words vir Python via .NET
articleTitle: Wat is nuut in Aspose.Words vir Python via .NET
linktitle: Wat is nuut in Aspose.Words vir Python via .NET
type: docs
description: "Aspose.Words vir Python via .NET brei en verbeter daagliks. Op hierdie bladsy kan jy leer oor die groot en interessantste kenmerke van die produk."
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /af/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-04-16-07-02-05
---

Hierdie bladsy beskryf die interessantste nuwe Aspose.Words funksies wat in onlangse vrystellings bekendgestel is.

## Aspose.Words vir Python via .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 stel AI-aangedrewe grammatika-kontrole bekend en verbeter dokumentbesparing met gevorderde opsies vir HTML, SVG en Markdown formate.

Aspose.Words 25.2 stel teksopsomming bekend met Anthropic AI modelle, voeg MsWorks formaatondersteuning by, verbeter tipografiese beheer en verbeter PDF struktuur en lyshantering.

Aspose.Words 25.3 verbeter'n AI-aangedrewe grammatika-kontroleerder en lettertipe-keuse met die UpdateAmbiguousTextFont eienskap, sowel as verbeter PDF aanhangsels uitvoer.

Aspose.Words 25.4 stel ondersteuning vir nuwe papier groottes, in staat stel om gevorderde HTML uitvoer beheer, en verbeter watermerk hantering.

### AI - aangedrewe Funksies

#### Dokument AI Grammatika Kontrole

* Die vermoë om die grammatika van die verskaf dokument te kontroleer met behulp van OpenAI generatiewe modelle is ingestel deur die toevoeging van'n nuwe [check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/) metode. <sup>25.1</sup>
* Die AI-aangedrewe Grammatika-Kontrolefunksie is opgedateer om alle modelle beskikbaar in die [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/) - opsomming te ondersteun. <sup>25.3</sup>

#### Opsomming Met Behulp Van Anthropic Generatiewe Taalmodelle <sup>25.2</sup>

Teks opsomming met behulp van Anthropic generatiewe taal modelle is in staat gestel deur die bekendstelling van'n nuwe openbare klas [AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/).

### Ondersteunde Formate <sup>25.2</sup>

Vanaf weergawe 25.2 is verenigbaarheid met die nuwe MsWorks laai formaat vir Microsoft Werk dokumente bygevoeg.

### Omskakeling, Laai En Stoor Van Dokumente

#### Verbeterde Stoor na HTML En SVG Formate <sup>25.1</sup>

Stoor na HTML en SVG formate is verbeter deur die toevoeging van **id_prefix** en **remove_java_script_from_links** eienskappe aan beide die [HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/) en [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) klasse.

#### Stel Beeldresolusie en OfficeMath Afvoermodus Wanneer Gestoor word na Markdown <sup>25.1</sup>

* 'n nuwe [image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/) opsie is bygevoeg om die [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) klas om die beeld resolusie stel.
* 'n nuwe [office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/) opsie en [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/) opsomming is en bygevoeg om die [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) klas OfficeMath uitset af te stel.

### Lewering

#### Verbeterde Tipografiese Beheer <sup>25.2</sup>

Die [number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/) eienskap is bygevoeg vir verbeterde tipografiese beheer.

#### Beheer Font Seleksie vir Dubbelsinnige Karakters <sup>25.3</sup>

'n nuwe openbare eiendom [update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/) is by die [SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/) klas gevoeg om die lettertipe te kies volgens die gebruikte karakterkode.

#### Papiergrootte Opsies <sup>25.4</sup>

Die vermoë om JIS B4 en JIS B5 papier groottes te gebruik is ingestel deur nuwe waardes by die [PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/) opsomming te voeg.

#### HTML Uitset Beheer <sup>25.4</sup>

Die vermoë om JavaScript uit hiperskakel URLs te verwyder tydens HTML uitvoer is ingestel deur die [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/) eienskap by te voeg.

### Ander

* PDF logiese struktuur is verbeter met ondersteuning vir TOA, BIBLIOGRAPHY, en INDEX velde. <sup>25.2</sup>
* Die [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate) metode is bekendgestel vir verbeterde lys hantering. <sup>25.2</sup>
* 'n nuwe eienskap [attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/) is bygevoeg om **EmbedAttachments** te vervang om PDF aanhangsels se uitvoer te verbeter. Nuwe waardes is ook by die [PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/) opsomming gevoeg om PDF/A weergawe aanhangsels te ondersteun. Daarbenewens word aanhangsels nou ondersteun met kodering. <sup>25.3</sup>
* Die vermoë om'n beeld watermerk van'n stroom stel is ingestel deur die toevoeging van'n nuwe oorlading om die [SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions) metode. <sup>25.4</sup>

{{% alert color="primary" %}}

Leer meer oor [Aspose.Words vir Python via .NET 25.1 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 25.2 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 25.3 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 25.4 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words vir Python via .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 stel group shape invoeging en StructuredDocumentTag invoeging via DocumentBuilder bekend, verbeter radiale kaartweergawe met grade, verbeter digitale handtekeninge met XAdES-EPES ondersteuning, voeg Markdown onderstreepherkenning by en bied toegang tot voetnoot/eindnoot skeiers.

Aspose.Words 24.10 stel verbeterde ActiveX beheer ondersteuning met CommandButton skepping, nuwe vorm sigbaarheid beheer, die vermoë om group shapes, verbeterde Markdown uitvoer vir tabelle, grafiek formatering vir Pie en Doughnut kaarte, beter Big5 kodering hantering, en ondersteuning vir verouderde Taiwanese lettertipes.

Aspose.Words 24.11 stel AI-aangedrewe dokumentopsomming, verbeterde weergawe opsies, verbeterde toegang tot dokument eienskappe en ActiveX beheer onderskrifte.

Aspose.Words 24.12 stel aanpasbare data etiket plasing, Google AI-aangedrewe teks vertaling, en verbeterde nuwe LowCode verwerking klasse.

### AI - aangedrewe Funksies

#### Dokumentopsomming met behulp van OpenAI En Google <sup>24.11</sup>

Ondersteuning vir dokumentopsomming met behulp van **OpenAI** en **Google** generatiewe taalmodelle is geïntegreer deur die [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) naamruimte by sy openbare lede te voeg.

#### Teksvertaling met Behulp Van Google se generatiewe taalmodelle <sup>24.12</sup>

Die vermoë om teks te vertaal met Behulp van Google se generatiewe taalmodelle is geïmplementeer in Aspose.Words deur die [translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/) metode en die [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) opsomming by die [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) naamruimte te voeg.

### Low Code <sup>24.12</sup>

Nuwe LowCode klasse soos [Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) en so aan. is bekendgestel, wat'n stel metodes bied wat die perfekte balans tussen eenvoud en buigsaamheid vir dokumentverwerking vind.

### Rendering En Drukwerk

#### Grade Op Radiale Kaarte <sup>24.9</sup>

Die lewering van grade op radiale kaarte is geïmplementeer.

#### CommandButton ActiveX Beheer <sup>24.10</sup>

Die vermoë om CommandButton ActiveX kontroles te skep is ingestel deur die toevoeging van'n nuwe openbare metode [insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/) en'n nuwe openbare klas [Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/).

#### Beheer Vorm Sigbaarheid <sup>24.10</sup>

'n nuwe openbare eiendom [hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/) is bygevoeg om die sigbaarheid van vorms te beheer.

#### Veranderinge in Pie En Doughnut Kaarte <sup>24.10</sup>

Verskeie nuwe openbare eiendomme is bygevoeg om Pie en Doughnut kaarte te formateer.

#### Beheer Die Weergawe van PDF Keuse Vorm Veld Grense <sup>24.11</sup>

'n nuwe opsie om die weergawe van PDF keuse vorm veld grense te beheer is geïmplementeer deur die toevoeging van'n nuwe openbare opsie [render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/).

#### Kry En Stel Formaatkodes Vir Grafiekdata In <sup>24.11</sup>

Die vermoë om formaat kodes vir grafiek data te kry en te stel is bygevoeg deur die implementering van die [format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/) eienskap in die [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), en [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/) klasse.

#### Gee Histogramkaarte met Bakkies en Etikette <sup>24.11</sup>

Histogramkaartvertoning is verbeter deur'n spesifieke aantal bakkies en etikette toe te laat.

#### Pas Die Plasing Van Datatikette aan <sup>24.12</sup>

Die vermoë om die plasing van data etikette aan te pas is bygevoeg deur die bekendstelling van nuwe eienskappe om th [ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/) en [ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/) klasse.

### Omskakeling, Laai En Stoor Van Dokumente

#### Onderstreep Formatering wanneer Markdown Lêers Gelaai Word <sup>24.9</sup>

Die opsie om onderstreepte opmaak te herken wanneer Markdown dokumente gelaai word, is opgeneem deur'n nuwe openbare eiendom [import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/) by te voeg.

#### Uitvoer tabelle as HTML wanneer stoor na Markdown <sup>24.10</sup>

'n opsie om tabelle as HTML uit te voer wanneer dokumente in Markdown formaat gestoor word, is geïmplementeer deur'n nuwe openbare eiendom [export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/) en'n opsomming [MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/) by te voeg.

#### Uitvoer PDF met Opgedateerde Logiese Struktuur <sup>24.11</sup>

PDF uitvoer is verbeter deur die insluiting van tabel titel eienskappe as PDF logiese struktuur element titels.

### Digitale Handtekeninge

#### Teken Dokumente met XAdES-EPES <sup>24.9</sup>

Die vermoë om dokumente met XAdES-EPES vlak XML-DSig handtekeninge te onderteken is gebruik deur'n nuwe openbare eiendom [xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/) en'n nuwe openbare opsomming [XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/) by te voeg.

### Ander

* 'n nuwe openbare metode [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/) is by group shapes gevoeg. <sup>24.9</sup>
* 'n nuwe openbare metode [insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/) is bygevoeg om **StructuredDocumentTags** in'n dokument in te voeg. <sup>24.9</sup>
* Openbare toegang tot voetnoot/eindnoot skeiers is verskaf deur die toevoeging van'n paar openbare klasse en eiendomme. <sup>24.9</sup>
* Die vermoë om individuele vorms, group shapes saam te groepeer en beide vorms en group shapes direk te groepeer, is ingestel deur die [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist) metode by te voeg. <sup>24.10</sup>
* Big5 kodering hantering vir TrueType cmap tabelle is verbeter. <sup>24.10</sup>
* Ondersteuning vir verouderde Taiwanese lettertipes is verbeter. <sup>24.10</sup>
* Om toegang tot uitgebreide dokument eienskappe, lees-alleen eienskappe is bygevoeg om die [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/) klas. <sup>24.11</sup>
* Die opstel van onderskrifte vir ActiveX kontroles is geaktiveer deur'n nuwe openbare setter by die [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/) eienskap te voeg. <sup>24.11</sup>

{{% alert color="primary" %}}

Leer meer oor [Aspose.Words vir Python via .NET 24.9 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 24.10 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 24.11 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 24.12 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words vir Python via .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 brei opsies vir samestellings uit, verbeter weergawevermoëns en brei'n paar ander opsies uit.

Aspose.Words 24.6 verbeter weergawe opsies, verbeter soek en vergelyk funksionaliteit, en brei verskeie ander funksies uit.

Aspose.Words 24.7 verander hoe jy met ActiveX werk, brei weergawevermoëns uit, sowel as uitvoer na Markdown en XLSX formate.

Aspose.Words 24.8 verbeter grafiek aanpassing met presiese beheer oor as etikette, brei lettertipe bestuur, verbeter dokument struktuur hantering, en voeg nuwe vermoëns vir HTML/XAML uitvoer, PDF funksionaliteit, dokument omskakeling, en digitale handtekeninge.

### Ondersteunde Formate

Vanaf weergawe 24.7 word uitvoer na PDF/UA-2 ondersteun om toeganklikheid vir gebruikers met gestremdhede te verseker.

### Rendering En Drukwerk

#### Veranderinge in Kaarte, Vorms en DrawingML <sup>24.5</sup>

* DrawingML effekte weergawe vir SVG grafiese, uitbreiding van vorige funksionaliteit beperk tot beelde, is geïmplementeer.
* Ondersteuning vir die skep van kombinasie kaarte en die aanpassing van eienskappe soos gaping breedte, oorvleueling, en borrel skaal binne reeks groepe is bekendgestel deur die toevoeging van die [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/) en [ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/) klasse en die [series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/) eiendom.
* Funksionaliteit om die SoftEdge effek van vorms te manipuleer is geïmplementeer deur die [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/) klas by te voeg.
* Die vermoë om aan te pas waardes van vorms is geïmplementeer deur die toevoeging van die **AdjustmentCollection** en **Adjustment** openbare klasse en [adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/) eiendom.

#### Veranderinge In Kaarte, Vorms en Tekeninge <sup>24.6</sup>

- Grafiese vermoëns is verbeter. Jy kan nou'n groter verskeidenheid kaarte skep, insluitend *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* kaarte, *Box & Whisker* kaarte, *Waterfalls*, en *Funnels*. Dit laat jou toe om jou data op'n meer diverse en insiggewende manier te visualiseer.
- Kleurbeheer vir skadu-opmaak is verbeter. U kan meer presiese beheer oor die voorkoms van u dokumente verkry deur toegang tot skadu-kleure te verkry.
- Prestasieverbetering vir agtergrondweergawe is verbeter. U kan die weergawe van agtergronde wat klein elemente bevat aansienlik versnel danksy inheemse teëltegnologie.
- Realistiese gradiënte vir vorms is bygevoeg. Jy kan nou DML vorms met nie-lineêre gradiënte skep, wat die visuele styl van Microsoft Word naboots vir'n meer gepoleerde voorkoms.

#### Grafiek Data Etiket Aanpassing <sup>24.7</sup>

Die vermoë om grafiek data etikette soos **Orientation** en **Rotation** aan te pas is bygevoeg.

#### Pasgemaakte Nommerstyling vir Lysvlakke <sup>24.7</sup>

'n stel vir die openbare eiendom [custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/) is bygevoeg. U kan nou'n pasgemaakte nommerstilering vir lysvlakke definieer.

#### Veranderinge in die werk met ActiveX <sup>24.7</sup>

- Die eienskappe van ActiveX voorwerpe kan nou verander word, wat jou meer beheer oor hul gedrag gee.
- Die vermoë om die waarde van die radio knoppie ActiveX beheer te verander om dinamiese interaksie in staat te stel is bygevoeg.
- Die vermoë om'n ActiveX checkbox te skakel na "gekontroleer" of "ongekontroleerd" is bygevoeg.

#### Beheer Oor Die Grafiek As Merk Etikette Oriëntasie En Rotasie <sup>24.8</sup>

Presiese beheer oor die oriëntasie en rotasie van grafiek as tik etikette is bygevoeg vir meer gerieflike grafiek aanpassing – die [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) klas is uitgebrei met nuwe [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) en [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/) eienskappe.

#### Vervang Die Agterste Skraal met Die Jen-Teken <sup>24.8</sup>

Die agteruit versoenbaar HTML en XAML uitvoer vir die vervanging van die agterste skraal karakter met die Jen teken is verbeter. Om dit te bereik, is die **replace_backslash_with_yen_sign** eienskap by die [HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/) en [XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/) klasse gevoeg.

#### Gebruik SDT Tags As Vorm Veld Name wanneer Uitvoer na PDF <sup>24.8</sup>

PDF uitvoer met ondersteuning vir die gebruik van SDT tags as vorm veld name is verbeter deur die toevoeging van'n nuwe [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) eienskap om die [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) klas.

### Omskakeling, Laai En Stoor Van Dokumente

#### Uitvoer Van Skakels na Markdown Formaat <sup>24.7</sup>

Die vermoë om die uitvoer van skakels in Markdown formaat te beheer is bygevoeg deur die implementering van die [link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/) eiendom.

#### LowCode 24.8 <sup>24.8</sup>

'n nuwe [LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/) klas, ontwerp om'n stel van metodes vir die omskakeling van verskeie dokument tipes met'n enkele reël van die kode te voorsien, is ingestel.

### Soek en Vergelyk

#### Gevorderde Vergelykingsopsies <sup>24.6</sup>

Die vermoë om data-analise werkstrome te stroomlyn met verbeterde vergelyking funksionaliteit is bygevoeg. Dit sluit'n nuwe [ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/) opsie en'n herontwerpte koppelvlak vir gevorderde vergelykings in.

### Ander

* Die funksie om leë bladsye uit'n dokument te verwyder is geïmplementeer deur die [remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/) metode by te voeg. <sup>24.5</sup>
* Die vermoë om te kyk vir die teenwoordigheid van VBA makros sonder om'n dokument te laai is verskaf deur die toevoeging van die [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/) eienskap. <sup>24.5</sup>
* Die behoud van bron nommering terwyl die invoeging van'n dokument met behulp van die LINQ Verslagdoening Enjin word nou ondersteun. <sup>24.5</sup>
* 'n nuwe [date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/) eienskap is bygevoeg - dit bied'n meer presiese tydstempel vir kommentaar, die verbetering van organisasie en naspeurbaarheid. <sup>24.6</sup>
* Die datum tyd formaat is nou outomaties opgespoor vir naatlose uitvoer na XLSX formaat. <sup>24.7</sup>
* Die openbare eiendom [is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/), wat jou toelaat om te verifieer of'n VBA projek beskerm word, is bygevoeg. <sup>24.7</sup>
* Lettertipe inligting is uitgebrei met die **embedding_licensing_rights** eienskap bygevoeg om die [FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/) en [PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/) klasse. <sup>24.8</sup>
* 'n manier om afdelingsopskrifte en-voetskrifte doeltreffend skoon te maak terwyl watermerke bewaar word, is bygevoeg om meer akkuraat met dokumentstruktuur te werk. Gebruik die nuwe openbare metode [clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default) om snitopskrifte en-voetskrifte skoon te maak. <sup>24.8</sup>
* Digitale ondertekening van XPS dokumente met behulp van [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/) is geaktiveer – 'n nuwe eienskap [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/) is bygevoeg vir hierdie doel. <sup>24.8</sup>

{{% alert color="primary" %}}

Leer meer oor [Aspose.Words vir Python via .NET 24.5 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 24.6 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 24.7 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 24.8 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words vir Python via .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 verbeter die ervaring rondom die bestuur van stroke kleure, verbeter OLE voorwerpe, sowel as stel'n nuwe `Bibliography Sources` openbare API.

Aspose.Words 24.2 uitgebreide Kaarte API en stylbestuur. Hierdie weergawe van Aspose.Words het ook die vermoë om SvgSaveOptions tydens weergawe te spesifiseer, meer buigsame beheer laai Markdown lêers, en werk met verwysing teks vir voetnotas en eindnotas.

Aspose.Words 24.3 stel'n nuwe TIFF Leser/Skrywer en Emulasie van binêre raster operasies vir WMF meta lêers. Aspose.Words 24.3 gaan ook voort om die Kaarte API uit te brei.

Aspose.Words 24.4 verbeter stoorformate, sommige weergawes, sowel as verbeter werk met digitale handtekeninge.

### Ondersteunde Formate <sup>24.4</sup>

Die moderne **WebP** beeld formaat word nou ondersteun in Aspose.Words vir .NET Framework 4.6.2 en hoër. Jy kan nou WebP beelde in dokumente lees en invoeg, asook beelde in WebP formaat stoor.

Let asseblief daarop dat WebP tans slegs beskikbaar is in .NET Standard en .NET Framework v4.6.2 en hoër.

### Rendering En Drukwerk

#### Stroke Kleur Beheer <sup>24.1</sup>

Die [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) klas is uitgebrei met'n stel van nuwe openbare eienskappe wat verband hou met die bestuur van beroerte kleure: [fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/) en [back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/), [fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/) en [back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### DrawingML Kaarte API Uitbreiding <sup>24.2 / 24.3 / 24.4</sup>

Die **DrawingML Charts API** word steeds uitgebrei.

#### Insluit Lettertipes Verklaar in @font-face Reëls <sup>24.4</sup>

Bygevoeg'n vermoë om lettertipes verklaar in @font-face reëls in die gevolglike dokument se lettertipe definisies is ingestel deur die toevoeging van'n nuwe [support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/) eiendom.

#### Werk Met Gloei en Refleksie Formatering <sup>24.4</sup>

Die vermoë om te werk met gloei en refleksie formatering vir'n tekening voorwerp is geïmplementeer.

### Laai En Stoor Dokumente

#### Spesifiseer SvgSaveOptions Tydens Lewering <sup>24.2</sup>

Die vermoë om [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) tydens weergawe te spesifiseer is bygevoeg met behulp van die [ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) en [OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) metodes.

#### Bewaar Leë Lyne wanneer Markdown lêers Gelaai Word <sup>24.2</sup>

Die vermoë om leë lyne te bewaar wanneer Markdown lêers gelaai word, is bygevoeg.

#### 'n Nuwe TIFF Leser / Skrywer <sup>24.3</sup>

'n nuwe TIFF leser/skrywer vir Aspose.Words is ontwikkel. Aspose.Words vir .NET 24.3 bygevoeg ondersteuning vir die lees van TIFF beelde met JPEG en Ou JPEG kompressie tipes, en ook aansienlik verbeter die gehalte van lees en skryf bedrywighede.

### Ander

* Die vermoë om die teks van die `TextBox` OLE beheer te verander is ingestel deur die toevoeging van'n nuwe **Text** eienskap om die nuwe **TextBoxControl** klas. <sup>24.1</sup>
* Die Bibliografie Sources public API is geïmplementeer deur die toevoeging van'n nuwe naamruimte [Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/) met sy nuwe klasse en opsommings, en deur die toevoeging van'n nuwe [bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/) eienskap aan die [Document](https://reference.aspose.com/words/python-net/aspose.words/document/) klas. <sup>24.1</sup>
* Nuwe openbare eiendomme [priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/), [unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/), en [semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/) vir verbeterde stylbestuur is by die [Style](https://reference.aspose.com/words/python-net/aspose.words/style/) klas gevoeg. <sup>24.2</sup>
* Die funksie om die werklike verwysingsmerk teks vir voetnotas en eindnotas te haal is verbeter met die [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/) eienskap en die [update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default) metode. <sup>24.2</sup>
* Emulasie van binêre raster operasies vir WMF metafiles is geïmplementeer. <sup>24.3</sup>
* Die vermoë om handtekening opsies vir dokumente binne **SaveOptions** te definieer is in staat gestel deur die toevoeging van'n nuwe [DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/) klas met nuwe openbare lede, sowel as die toevoeging van nuwe eienskappe aan die [OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/) en [OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/) klasse. <sup>24.4</sup>

{{% alert color="primary" %}}

Leer meer oor [Aspose.Words vir Python via .NET 24.1 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 24.2 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 24.3 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 24.4 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words vir Python via .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 brei weergawe opsies, metafile weergawe emulasie, en markdown stoor opsies.

Aspose.Words 23.10 verbeter weergawe, brei opsies uit vir die laai en stoor van dokumente, en laat gebruikers toe om dokumente op nuwe maniere saam te voeg.

Aspose.Words 23.11 verbeter die werk met hersienings, XLSX formaat en lettertipes op grafieklegende met bykomende opsies.

Aspose.Words 23.12 stel nuwe eienskappe en opsommings bekend vir die werk met PDF en OOXML dokumente, sowel as ondersteuning vir WebP beelde.

### Rendering En Drukwerk

#### Aanpas Asse Titels in DrawingML Kaarte <sup>23.9</sup>

Die vermoë om axis titels in DrawingML kaarte aan te pas is bekendgestel deur die implementering van'n nuwe openbare klas [ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/) en [title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/) eiendom.

####  Bepaling van Die Vertikale Posisie van Lettertipes binne'n Paragraaf <sup>23.9</sup>

Dit is nou moontlik om die vertikale posisie van lettertipes binne'n paragraaf te definieer deur die nuwe openbare [baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/) eienskap en die nuwe [BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/) opsomming te gebruik.

#### Voorgrond Kleur Beheer <sup>23.10</sup>

Die vermoë om die voorgrond kleur te haal sonder veranderlikes is bygevoeg om die [Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/) en [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) klasse via die **BaseForeColor** eiendom.

#### Uitbreiding Van Die Funksionaliteit Van Kaarte <sup>23.10</sup>

Die funksionaliteit van die [ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/), en [ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/) klasse is uitgebrei met nuwe metodes en eienskappe.

#### Pas'n Prent outomaties aan en Pas dit In'n Vorm <sup>23.10</sup>

'n eenvoudige manier om'n beeld outomaties in'n spesifieke vorm aan te pas en te pas, is deur die nuwe [fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default) metode voorsien.

#### Verstek Skrif Tipe Formatering vir DrawingML Grafiek Legende Inskrywings <sup>23.11</sup>

Die vermoë om standaard lettertipe opmaak vir legend inskrywings van DrawingML kaarte spesifiseer is bygevoeg via die [font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/) eiendom. Hierdie kenmerk vergemaklik'n meer gestroomlynde en konsekwente voorkoms vir kaartelemente, wat die algehele dokumentestetika verbeter.

#### Spesifiseer Bladsyuitleg wanneer PDF In Reader Oopgemaak Word <sup>23.12</sup>

Die vermoë om die bladsy uitleg te spesifiseer wat gebruik moet word wanneer'n dokument in'n PDF leser oopgemaak word, is bygevoeg deur die bekendstelling van'n nuwe [page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/) eienskap aan die [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) klas en die bekendstelling van'n nuwe [PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/) opsomming.

### Laai En Stoor Dokumente

#### Spesifiseer'n Gidsnaam Om Beeld URIs In MarkdownTe Bou <sup>23.9</sup>

Die [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) klas is uitgebrei deur die [images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/) eienskap, wat toelaat om die naam van die gids wat gebruik word om beeld URIs geskryf in die Markdown dokument te bou spesifiseer.

#### Verminder PDF Uitset Grootte <sup>23.10</sup>

Verskeie PDF vertoon optimalisaties om uitset grootte te verminder wanneer die gebruik van [optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/) instellings geïmplementeer is.

#### Herken Hiperskakels wanneer TXT Dokumente Gelaai Word <sup>23.10</sup>

Die funksie om hiperskakels te herken wanneer TXT dokumente gelaai word, is geïmplementeer deur'n nuwe [detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/) eienskap by te voeg.

### Ander

- Metafile rendering emulasie om rasterisering grootte te bepaal is geïmplementeer, spesifiek vir WMF pen breedte en EMF kosmetiese pen breedte. Om dit te bereik, is die **ScaleWmfFontsToMetafileSize** eienskap vervang met die [emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/) eienskap en die [emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/) eienskap is bygevoeg. <sup>23.9</sup>
- 'n vereenvoudigde metode vir die invoeging van een dokument in'n ander dokument by die huidige wyser posisie is ingestel met behulp van die [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions) metode. <sup>23.10</sup>
- Die vermoë om toegang tot en styl eienskappe te verander is bygevoeg deur die bekendstelling van die nuwe [locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/) eiendom. <sup>23.10</sup>
- 'n generiese tipe parameter is bygevoeg om die metodes van die [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/) klas. <sup>23.10</sup>
- Die vermoë om alle afdelings van'n dokument op dieselfde XLSX werkblad te skryf is verskaf deur die nuwe [XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/) opsomming tipe en die nuwe [section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/) eienskap. <sup>23.11</sup>
* 'n manier om te beheer hoe ZIP64 formaat uitbreidings gebruik sal word vir OOXML dokumente is geïmplementeer deur die nuwe Zip64Mode eienskap van die `OoxmlSaveOptions` klas en die nuwe Zip64Mode opsomming. <sup>23.12</sup>
* Ondersteuning vir WebP beeld is ingestel. Let asseblief daarop dat hierdie funksie slegs beskikbaar is vir.NetStandart en .NET6+ weergawes. <sup>23.12</sup>

{{% alert color="primary" %}}

Leer meer oor [Aspose.Words vir Python via .NET 23.9 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 23.10 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 23.11 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

Leer meer oor [Aspose.Words vir .NET 23.12 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words vir Python via .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 verbeter die vermoë om met grafiekreeksdata te werk en die vermoë om met ODT dokumente te werk, asook om koptekste/voetskrifte en hul teksverpakking te verbeter.

Aspose.Words 23.6 brei weergawes uit, voeg'n nuwe uitvoerformaat by, verbeter LINQ verslagdoening en LowCode gereedskap.

Aspose.Words 23.7 verbeter verslagdoening vermoëns, voeg'n nuwe uitvoer formaat, en stel veranderinge aan die werk met tabelle en digitale handtekeninge.

Aspose.Words 23.8 brei die vermoëns van verskillende formate uit, verbeter weergawe en voeg nuwe opsies by om met velde te werk.

### Ondersteunde Formate

* Begin met weergawe 23.6, is dit moontlik om'n dokument in XLSX formaat te stoor. Nou kan jy jou dokumente omskep In Excel-formaat. <sup>23.6</sup>

* Begin met weergawe 23.7, is dit moontlik om'n dokument bladsy of vorm in EPS formaat te stoor. <sup>23.7</sup>

### Nuwe Formaat Kenmerke

- Die funksie om Outomaties Inhoudsopgawe (TOC) vir MOBI dokumente te genereer, is bekendgestel. <sup>23.8</sup>
- Die [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) konstruktor is uitgebrei met [PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions). <sup>23.8</sup>
- Die vorming van vertikale teks vir EMF metafiles is geïmplementeer. <sup>23.8</sup>

### Lewering

#### Kry En Wysig Grafiekreeksdata <sup>23.5</sup>

Die funksie om te kry en te verander grafiek reeks data is verskaf deur die toevoeging van:

- nuwe klasse: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- nuwe enum tipes: [ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### Ondersteuning Vir Gevorderde Tipografie <sup>23.6</sup>

Ondersteuning vir Gevorderde Tipografie in WMF, EMF en EMF+ weergawe is bygevoeg.

#### Gekleurde Inhoud op Die Bladsy <sup>23.6</sup>

Die openbare eiendom [PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/), wat aandui of die bladsy gekleurd is of nie, is bygevoeg.

#### Formatering vir Grafiek Data Etikette <sup>23.6</sup>

Die vermoë om vul, beroerte, en oproep formatering vir grafiek data etikette is geïmplementeer.

### Mail Merge En Verslagdoening

#### Dinamiese HTML Invoeging vir LINQ Verslagdoening Enjin <sup>23.6</sup>

'n nuwe manier van dinamiese HTML invoeging vir LINQ Verslagdoening Enjin is bygevoeg.

#### Mustache Tags Ondersteuning <sup>23.7</sup>

Mustache tags word nou ondersteun in die [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/) en [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/) metodes.

#### Spesifiseer Die Grootte Van Gerenderde Beelde <sup>23.8</sup>

'n nuwe openbare eiendom [image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/) vir die spesifisering van die grootte van weergegee beelde in pixel is bekendgestel.

#### Bewaar Witruimtes vir JSON String Waardes - LINQ <sup>23.8</sup>

'n opsie is bygevoeg om die LINQ Verslagdoening Enjin witruimtes vir JSON string waardes te bewaar.

### LowCode <sup>23.6</sup>

Nuwe LowCode metodes wat bedoel is om verskillende tipes dokumente saam te smelt in'n enkele uitset dokument is bygevoeg.

### Ander

- Ondersteuning vir teks wrap in kop/voet is geïmplementeer. <sup>23.5</sup>
- Die vermoë om digitale handtekeninge uit ODT dokumente te verwyder is bygevoeg deur die [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str) metode. <sup>23.5</sup>
- Die openbare eiendom [phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/) om die basis-en robyn teks van die fonetiese gids [Run](https://reference.aspose.com/words/python-net/aspose.words/run/) te verkry, is bygevoeg. <sup>23.5</sup>
- Die vermoë om'n digitale handtekening waarde van'n digitaal onderteken dokument as'n byte skikking is bygevoeg deur die bekendstelling van'n nuwe [signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/) eiendom. <sup>23.7</sup>
- Die [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/) en [Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/) klasse is uitgebrei met nuwe openbare lede– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), en [Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/). <sup>23.7</sup>

{{% alert color="primary" %}}

Leer meer oor [Aspose.Words vir Python via .NET 23.5 Vrystelling Notas](/words/python-net/aspose-words-for-python-via-dotnet-23-5-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 23.6 Vrystelling Notas](/words/python-net/aspose-words-for-python-via-dotnet-23-6-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 23.7 Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

Leer meer oor [Aspose.Words vir Python via .NET 23.8 Vrystelling Notas](/words/python-net/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## Sien Ook

{{% alert color="primary" %}}

Hierdie bladsy bevat die jongste nuus oor die afgelope 2 jaar. Vir besonderhede oor vorige vrystellings, sien die [Vrystelling Notas](https://releases.aspose.com/words/python/release-notes/) bladsye in die relevante afdelings.

{{% /alert %}}
