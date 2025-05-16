---
title: Wat is er nieuw
second_title: Aspose.Words voor .NET
articleTitle: Wat is er nieuw in Aspose.Words voor .NET
linktitle: Wat is er nieuw in Aspose.Words voor .NET
type: docs
description: "Aspose.Words voor .NET breidt en verbetert dagelijks. Op deze pagina kunt u meer te weten komen over de enorme en meest interessante functies van het product."
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nl/net/what-s-new-in-aspose-words-for-net/
timestamp: 2025-04-16-07-02-05
---

Deze pagina beschrijft de meest interessante nieuwe Aspose.Words - functies die zijn geïntroduceerd in recente releases.

## Aspose.Words voor .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 introduceert grammaticacontrole op basis van AI en verbetert het opslaan van documenten met geavanceerde opties voor HTML, SVG en Markdown formaten.

Aspose.Words 25.2 introduceert tekstsamenvatting met Anthropic AI modellen, voegt MsWorks formaatondersteuning toe, verbetert typografische controle en verbetert PDF structuur en lijstverwerking.

Aspose.Words 25.3 verbetert een door AI aangedreven grammaticacontrole en lettertypeselectie met de eigenschap UpdateAmbiguousTextFont, en verbetert de export van PDF bijlagen.

Aspose.Words 25.4 introduceert ondersteuning voor nieuwe papierformaten, maakt geavanceerde HTML exportcontrole mogelijk, verbetert de behandeling van watermerken en verbetert de bruikbaarheid van de LowCode API.

### AI-aangedreven functies

#### Document AI Grammaticacontrole

* De mogelijkheid om de grammatica van het verstrekte document te controleren met behulp van OpenAI generatieve modellen is geïntroduceerd door een nieuwe [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/) methode toe te voegen. <sup>25.1</sup>
* De door AI aangedreven Grammaticacontrolefunctie is bijgewerkt om alle modellen te ondersteunen die beschikbaar zijn in de [AiModelType](https://reference.aspose.com/words/net/aspose.words.ai/aimodeltype/)-opsomming. <sup>25.3</sup>

#### Samenvatting Met Behulp Van Anthropic Generatieve Taalmodellen <sup>25.2</sup>

Tekstsamenvatting met behulp van Anthropic generatieve taalmodellen is mogelijk gemaakt door een nieuwe openbare klasse [AnthropicAiModel](https://reference.aspose.com/words/net/aspose.words.ai/anthropicaimodel/) in te voeren.

### Low Code

#### Low Code API bruikbaarheid <sup>25.4</sup>

De bruikbaarheid van **LowCode API** is aanzienlijk verbeterd, waardoor de documentverwerking wordt vereenvoudigd en de noodzaak van herhalende code wordt verminderd.

### Ondersteunde Formaten <sup>25.2</sup>

Vanaf versie 25.2 is compatibiliteit met de nieuwe MsWorks load-indeling voor Microsoft werkdocumenten toegevoegd.

### Documenten converteren, laden en opslaan

#### Verbeterde opslag naar HTML en SVG indelingen <sup>25.1</sup>

Opslaan in HTML en SVG formaten is verbeterd door **IdPrefix** en **RemoveJavaScriptFromLinks** eigenschappen toe te voegen aan zowel de [HtmlFixedSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlfixedsaveoptions/) als [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/) klassen.

#### Stel afbeeldingsresolutie en OfficeMath uitvoermodus in bij opslaan op Markdown <sup>25.1</sup>

* Er is een nieuwe optie [ImageResolution](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imageresolution/) toegevoegd aan de klasse [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) om de afbeeldingsresolutie in te stellen.
* Een nieuwe [OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/officemathexportmode/) optie en [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownofficemathexportmode/) opsomming zijn toegevoegd aan de [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) klasse om OfficeMath output mode in te stellen.
* De mogelijkheid om een beeldwatermerk van een stroom in te stellen is geïntroduceerd door een nieuwe overbelasting toe te voegen aan de methode [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage_2). <sup>25.4</sup>

### Rendering

#### Verbeterde Typografische Controle <sup>25.2</sup>

De eigenschap [NumberSpacing](https://reference.aspose.com/words/net/aspose.words/font/numberspacing/) is toegevoegd voor verbeterde typografische controle.

#### Controle van de lettertypeselectie voor dubbelzinnige tekens <sup>25.3</sup>

Er is een nieuwe openbare eigenschap [UpdateAmbiguousTextFont](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/updateambiguoustextfont/) toegevoegd aan de klasse [SaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/) om de lettertypeselectie te regelen volgens de gebruikte tekencode.

#### Opties Voor Papierformaat <sup>25.4</sup>

De mogelijkheid om JIS B4 en JIS B5 papierformaten te gebruiken is geïntroduceerd door nieuwe waarden toe te voegen aan de [PaperSize](https://reference.aspose.com/words/net/aspose.words/papersize/) opsomming.

#### HTML Uitvoercontrole <sup>25.4</sup>

De mogelijkheid om JavaScript van hyperlink URLs te verwijderen tijdens HTML export is geïntroduceerd door de eigenschap [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/removejavascriptfromlinks/) toe te voegen.

### Ander

* PDF logische structuur is verbeterd met ondersteuning voor TOA, BIBLIOGRAPHY en INDEX velden. <sup>25.2</sup>
* De [AddSingleLevelList](https://reference.aspose.com/words/net/aspose.words.lists/listcollection/addsinglelevellist/) methode is geïntroduceerd voor verbeterde lijstverwerking. <sup>25.2</sup>
* Er is een nieuwe eigenschap [AttachmentsEmbeddingMode](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/attachmentsembeddingmode/) toegevoegd om **EmbedAttachments** te vervangen om de export van PDF bijlagen te verbeteren. Ook zijn er nieuwe waarden toegevoegd aan de [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) opsomming om PDF/A versiebijlagen te ondersteunen. Bovendien worden bijlagen nu ondersteund met encryptie. <sup>25.3</sup>

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor .NET 25.1 vrijgave](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-1-release-notes/).

Lees meer over [Aspose.Words voor .NET 25.2 vrijgave](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-2-release-notes/).

Lees meer over [Aspose.Words voor .NET 25.3 vrijgave](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-3-release-notes/).

Lees meer over [Aspose.Words voor .NET 25.4 vrijgave](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words voor .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduceert group shape invoeging en StructuredDocumentTag invoeging via DocumentBuilder, verbetert de weergave van radiale grafieken met graduaties, verbetert digitale handtekeningen met XAdES-EPES ondersteuning, voegt Markdown onderstrepingherkenning toe en biedt toegang tot voetnoot/eindnoot scheidingstekens.

Aspose.Words 24.10 introduceert verbeterde ActiveX control-ondersteuning met CommandButton creatie, nieuwe shape visibility control, de mogelijkheid om group shapes, verbeterde Markdown export voor tabellen, grafiekopmaak voor Pie en Doughnut grafieken, betere Big5-codering en ondersteuning voor verouderde Taiwanese lettertypen.

Aspose.Words 24.11 introduceert AI-aangedreven document samenvatting, verbeterde rendering opties, verbeterde toegang tot document eigenschappen en ActiveX control Ondertiteling.

Aspose.Words 24.12 introduceert aanpasbare data label plaatsing, Google AI-aangedreven tekstvertaling, verbeterde Mail Merge opschoonopties en nieuwe LowCode verwerkingsklassen.

### AI-aangedreven functies

#### Samenvatting van documenten met behulp van OpenAI en Google <sup>24.11</sup>

Ondersteuning voor documentsamenvatting met behulp van **OpenAI** en **Google** generatieve taalmodellen is geïntegreerd door de [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) naamruimte toe te voegen aan zijn openbare leden.

#### Tekstvertaling met behulp van Google ' s generatieve taalmodellen <sup>24.12</sup>

De mogelijkheid om tekst te vertalen met behulp van Google ' s generatieve taalmodellen is geïmplementeerd in Aspose.Words door de [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) methode en de [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) opsomming toe te voegen aan de [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) naamruimte.

### Low Code <sup>24.12</sup>

Nieuwe LowCode klassen zoals [Comparer](https://reference.aspose.com/words/net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/net/aspose.words.lowcode/splitter/) enz. is geïntroduceerd en biedt een reeks methoden die de perfecte balans vinden tussen eenvoud en flexibiliteit voor documentverwerking.

### Rendering en afdrukken

#### Graduaties op radiale grafieken <sup>24.9</sup>

De weergave van graduaties op radiale grafieken is geïmplementeerd.

#### CommandButton ActiveX besturingselementen <sup>24.10</sup>

De mogelijkheid om CommandButton ActiveX besturingselementen te maken is geïntroduceerd door een nieuwe openbare methode [InsertForms2OleControl](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertforms2olecontrol/) en een nieuwe openbare klasse [Forms2OleControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/) toe te voegen.

#### Control Shape Visibility <sup>24.10</sup>

Er is een nieuwe openbare eigenschap [Hidden](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/hidden/) toegevoegd om de zichtbaarheid van shapes te regelen.

#### Veranderingen in Pie en Doughnut grafieken <sup>24.10</sup>

Er zijn verschillende nieuwe openbare eigenschappen toegevoegd om Pie en Doughnut grafieken op te maken.

#### De weergave van PDF Keuzeveldranden bepalen <sup>24.11</sup>

Er is een nieuwe optie geïmplementeerd om de weergave van PDF keuzeveldranden voor formuliervelden te beheren door een nieuwe openbare optie [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/renderchoiceformfieldborder/) toe te voegen.

#### Formaatcodes voor Grafiekgegevens ophalen en instellen <sup>24.11</sup>

De mogelijkheid om formaatcodes voor grafiekgegevens te verkrijgen en in te stellen is toegevoegd door de eigenschap [FormatCode](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/formatcode/) in de klassen [ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/) en [BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/) te implementeren.

#### Histogramdiagrammen weergeven met bakken en Labels <sup>24.11</sup>

De weergave van histogrammen is verbeterd door een bepaald aantal bakken en labels toe te staan.

#### De plaatsing van Gegevenslabels aanpassen <sup>24.12</sup>

De mogelijkheid om de plaatsing van gegevenslabels aan te passen is toegevoegd door nieuwe eigenschappen toe te voegen aan de klassen [ChartDataLabel](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabel/) en [ChartDataLabelCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Documenten converteren, laden en opslaan

#### Onderstrepen opmaak bij het laden van Markdown bestanden <sup>24.9</sup>

De optie om onderstreping te herkennen bij het laden van Markdown documenten is opgenomen door een nieuwe openbare eigenschap [ImportUnderlineFormatting](https://reference.aspose.com/words/net/aspose.words.loading/markdownloadoptions/importunderlineformatting/) toe te voegen.

#### Tabellen exporteren als HTML bij opslaan naar Markdown <sup>24.10</sup>

Een optie om tabellen als HTML te exporteren bij het opslaan van documenten in Markdown - indeling is geïmplementeerd door een nieuwe openbare eigenschap [ExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/exportashtml/) en een opsomming [MarkdownExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownexportashtml/) toe te voegen.

#### PDF exporteren met bijgewerkte logische structuur <sup>24.11</sup>

De export van PDF is verbeterd door eigenschappen van tabeltitels op te nemen als titels van logische structuurelementen van PDF.

### Mail Merge en rapportage

#### Lege tabellen verwijderen tijdens Mail Merge <sup>24.12</sup>

Een nieuwe **RemoveEmptyTables** optie is toegevoegd aan de [MailMergeCleanupOptions](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmergecleanupoptions/) opsomming om Mail Merge output te verfijnen.

### Digitale Handtekeningen

#### Documenten ondertekenen met XAdES-EPES <sup>24.9</sup>

De mogelijkheid om documenten te ondertekenen met XAdES-EPES Niveau XML-DSig handtekeningen is geïntroduceerd door het toevoegen van een nieuwe openbare eigenschap [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/signoptions/xmldsiglevel/) en een nieuwe openbare opsomming [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/xmldsiglevel/).

### Ander

* Er is een nieuwe openbare methode [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/) toegevoegd aan group shapes. <sup>24.9</sup>
* Er is een nieuwe openbare methode [InsertStructuredDocumentTag](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertstructureddocumenttag/) toegevoegd om **StructuredDocumentTags** in een document in te voegen. <sup>24.9</sup>
* Openbare toegang tot voetnoot / eindnoot scheidingstekens is verschaft door het toevoegen van een paar openbare klassen en eigenschappen. <sup>24.9</sup>
* De mogelijkheid om afzonderlijke vormen, group shapes samen te groeperen en beide vormen en group shapes rechtstreeks te groeperen, is geïntroduceerd door de methode [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/#insertgroupshape_1) toe te voegen. <sup>24.10</sup>
* Big5 encoding handling voor TrueType cmap tabellen is verbeterd. <sup>24.10</sup>
* Ondersteuning voor verouderde Taiwanese lettertypen is verbeterd. <sup>24.10</sup>
* Voor toegang tot uitgebreide Documenteigenschappen zijn alleen-lezen eigenschappen toegevoegd aan de klasse [BuiltInDocumentProperties](https://reference.aspose.com/words/net/aspose.words.properties/builtindocumentproperties/). <sup>24.11</sup>
* Het instellen van bijschriften voor ActiveX besturingselementen is ingeschakeld door een nieuwe openbare setter toe te voegen aan de eigenschap [Forms2OleControl.Caption](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor .NET 24.9 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-9-release-notes/).

Lees meer over [Aspose.Words voor .NET 24.10 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-10-release-notes/).

Lees meer over [Aspose.Words voor .NET 24.11 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-11-release-notes/).

Lees meer over [Aspose.Words voor .NET 24.12 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words voor .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 breidt opties voor assemblies uit, verbetert de rendermogelijkheden en breidt enkele andere opties uit.

Aspose.Words 24.6 verbetert de weergaveopties, verbetert de Zoek-en vergelijkingsfunctionaliteit en breidt verschillende andere functies uit.

Aspose.Words 24.7 wijzigt de manier waarop u met ActiveX werkt, breidt de weergavemogelijkheden uit en exporteert naar Markdown en XLSX indelingen.

Aspose.Words 24.8 verbetert de aanpassing van grafieken met nauwkeurige controle over aslabels, breidt het lettertypebeheer uit, verbetert de afhandeling van documentstructuren en voegt nieuwe mogelijkheden toe voor HTML/XAML export, PDF functionaliteit, documentconversie en digitale handtekeningen.

### Ondersteunde Formaten

Vanaf versie 24.7 wordt exporteren naar PDF/UA-2 ondersteund om toegankelijkheid voor gebruikers met een handicap te garanderen.

### Platform <sup>24.5</sup>

.NET 7.0/8.0 assemblies zijn opgenomen in het Aspose.Words NuGet pakket.

### Rendering en afdrukken

#### Wijzigingen in grafieken, vormen en DrawingML <sup>24.5</sup>

* DrawingML effecten rendering voor SVG graphics, uitbreiding van de vorige functionaliteit beperkt tot afbeeldingen, is geïmplementeerd.
* Ondersteuning voor het maken van combo-diagrammen en het aanpassen van eigenschappen zoals gap width, overlap en bubble scale binnen reeksgroepen is geïntroduceerd door de [ChartSeriesGroup](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroup/) en [ChartSeriesGroupCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroupcollection/) klassen en de [SeriesGroups](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/seriesgroups/) eigenschap toe te voegen.
* Functionaliteit om het SoftEdge effect van shapes te manipuleren is geïmplementeerd door de [SoftEdgeFormat](https://reference.aspose.com/words/net/aspose.words.drawing/softedgeformat/) klasse toe te voegen.
* De mogelijkheid om waarden van shapes aan te passen te wijzigen is geïmplementeerd door de eigenschap [AdjustmentCollection](https://reference.aspose.com/words/net/aspose.words.drawing/adjustmentcollection/) en [Adjustment](https://reference.aspose.com/words/net/aspose.words.drawing/adjustment/) openbare klassen en [Adjustments](https://reference.aspose.com/words/net/aspose.words.drawing/shape/adjustments/) toe te voegen.

#### Wijzigingen in grafieken, vormen en tekening <sup>24.6</sup>

* De kaartmogelijkheden zijn verbeterd. U kunt nu een grotere verscheidenheid aan grafieken maken, waaronder *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* grafieken, *Box & Whisker* grafieken, *Waterfalls* en *Funnels*. Hierdoor kunt u uw gegevens op een meer diverse en informatieve manier visualiseren.
* Kleurcontrole voor schaduwopmaak is verbeterd. U kunt nauwkeuriger controle krijgen over het uiterlijk van uw documenten door toegang te krijgen tot schaduwkleuren.
* Performance boost voor achtergrond rendering is verbeterd. U kunt het renderen van achtergronden met kleine elementen aanzienlijk versnellen dankzij native tegeltechnologie.
* Er zijn realistische gradiënten voor vormen toegevoegd. U kunt nu DML-vormen maken met niet-lineaire verlopen, waarbij de visuele stijl van Microsoft Word wordt nagebootst voor een meer gepolijste look.

#### Aanpassing Van Diagramgegevens <sup>24.7</sup>

De mogelijkheid om diagramgegevenslabels zoals **Orientation** en **Rotation** Aan te passen is toegevoegd.

#### Aangepaste nummer Styling Voor Lijstniveaus <sup>24.7</sup>

Er is een setter voor de openbare eigenschap [CustomNumberStyleFormat](https://reference.aspose.com/words/net/aspose.words.lists/listlevel/customnumberstyleformat/) toegevoegd. U kunt nu een aangepaste nummerstyling definiëren voor lijstniveaus.

#### Wijzigingen in het werken met ActiveX <sup>24.7</sup>

* De eigenschappen van ActiveX objecten kunnen nu worden gewijzigd, waardoor u meer controle over hun gedrag krijgt.
* De mogelijkheid om de waarde van het keuzerondje ActiveX te wijzigen om dynamische interactie mogelijk te maken, is toegevoegd.
* De mogelijkheid om een ActiveX checkbox om te schakelen naar "aangevinkt" of "niet aangevinkt" is toegevoegd.

#### Controle over de Grafiekas Tick Labels oriëntatie en rotatie <sup>24.8</sup>

Nauwkeurige controle over de oriëntatie en rotatie van de diagramas tick labels is toegevoegd voor handiger aanpassing van de grafiek – de [AxisTickLabels](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/) klasse is uitgebreid met nieuwe [Orientation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/orientation/) en [Rotation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/rotation/) eigenschappen.

#### De Backslash vervangen door het Yen teken <sup>24.8</sup>

De backwards compatible HTML en XAML export voor het vervangen van het backslash teken door het Yen teken is verbeterd. Om dit te bereiken is de eigenschap **ReplaceBackslashWithYenSign** toegevoegd aan de klassen [HtmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/) en [XamlFlowSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xamlflowsaveoptions/).

#### SDT Tags gebruiken als Formulierveldnamen bij exporteren naar PDF <sup>24.8</sup>

PDF exporteren met ondersteuning voor het gebruik van SDT tags als formulierveldnamen is verbeterd door een nieuwe eigenschap [UseSdtTagAsFormFieldName](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/usesdttagasformfieldname/) toe te voegen aan de [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) - klasse.

### Documenten converteren, laden en opslaan

#### Koppelingen exporteren naar Markdown - indeling <sup>24.7</sup>

De mogelijkheid om de export van koppelingen in Markdown - indeling te beheren is toegevoegd door de implementatie van de eigenschap [LinkExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/linkexportmode/).

#### LowCode 24.8 <sup>24.8</sup>

Er is een nieuwe [LowCode.Converter](https://reference.aspose.com/words/net/aspose.words.lowcode/converter/) - Klasse geïntroduceerd, ontworpen om een reeks methoden te bieden voor het converteren van verschillende documenttypen met één enkele regel code.

### Zoeken en vergelijken

#### Geavanceerde Vergelijkingsopties <sup>24.6</sup>
De mogelijkheid om data-analyse workflows te stroomlijnen met verbeterde vergelijkingsfunctionaliteit is toegevoegd. Dit omvat een nieuwe optie [IgnoreStoreItemId](https://reference.aspose.com/words/net/aspose.words.comparing/advancedcompareoptions/ignorestoreitemid/) en een vernieuwde interface voor geavanceerde vergelijkingen.

### Ander

* De functie om lege pagina ' s uit een document te verwijderen is geïmplementeerd door de methode [RemoveBlankPages](https://reference.aspose.com/words/net/aspose.words/document/removeblankpages/) toe te voegen. <sup>24.5</sup>
* De mogelijkheid om te controleren op de aanwezigheid van VBA macro ' s zonder een document te laden, is geleverd door de eigenschap [HasMacros](https://reference.aspose.com/words/net/aspose.words/fileformatinfo/hasmacros/) toe te voegen. <sup>24.5</sup>
* Het behouden van bronnummering tijdens het invoegen van een document met behulp van de LINQ Rapportageengine wordt nu ondersteund. <sup>24.5</sup>
* Er is een nieuwe eigenschap [DateTimeUtc](https://reference.aspose.com/words/net/aspose.words/comment/datetimeutc/) toegevoegd – Dit biedt een nauwkeuriger tijdstempel voor opmerkingen, waardoor de organisatie en traceerbaarheid worden verbeterd. <sup>24.6</sup>
* De LINQ Reporting Engine is verbeterd. Selectieve verwijdering van lege alinea ' s en definitie van aangepaste berichten voor ontbrekende objectleden zijn gemaakt, wat leidt tot schonere en meer informatieve rapporten. <sup>24.6</sup>
* De DateTime-indeling wordt nu automatisch gedetecteerd voor naadloze export naar XLSX - indeling. <sup>24.7</sup>
* De openbare eigenschap [IsProtected](https://reference.aspose.com/words/net/aspose.words.vba/vbaproject/isprotected/), waarmee u kunt controleren of een VBA - project is beschermd, is toegevoegd. <sup>24.7</sup>
* Lettertypeinformatie is uitgebreid met de eigenschap **EmbeddingLicensingRights** toegevoegd aan de klassen [FontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/fontinfo/) en [PhysicalFontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* Er is een manier toegevoegd om sectiekoppen en voetteksten efficiënt te wissen met behoud van watermerken om nauwkeuriger te werken met documentstructuur. Als u sectiekoppen en voetteksten wilt wissen, gebruikt u de nieuwe openbare methode [ClearHeadersFooters](https://reference.aspose.com/words/net/aspose.words/section/clearheadersfooters/). <sup>24.8</sup>
* Digitale ondertekening van XPS documenten met behulp van [XpsSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/) is ingeschakeld – hiervoor is een nieuwe eigenschap [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/digitalsignaturedetails/) toegevoegd. <sup>24.8</sup>

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor .NET 24.5 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-5-release-notes/).

Lees meer over [Aspose.Words voor .NET 24.6 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-6-release-notes/).

Lees meer over [Aspose.Words voor .NET 24.7 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-7-release-notes/).

Lees meer over [Aspose.Words voor .NET 24.8 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words voor .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 verbetert de ervaring met het beheren van lijnkleuren, verbetert OLE objecten en LINQ rapportage, en introduceert een nieuwe `Bibliography Sources` public API.

Aspose.Words 24.2 Uitgebreide grafieken API, stijlbeheer en LINQ opties. Deze versie van Aspose.Words introduceerde ook de mogelijkheid om SvgSaveOptions te specificeren tijdens het renderen, flexibeler controle laden van Markdown bestanden en werken met referentietekst voor voetnoten en eindnoten.

Aspose.Words 24.3 introduceert een nieuwe TIFF Reader/Writer en emulatie van binaire rasterbewerkingen voor WMF metafiles. Aspose.Words 24.3 blijft ook de grafieken API uitbreiden.

Aspose.Words 24.4 verbetert de opslagindelingen, sommige weergaveopties en verbetert het werken met digitale handtekeningen.

### Ondersteunde Formaten <sup>24.4</sup>

De moderne **WebP** afbeeldingsindeling wordt nu ondersteund in Aspose.Words voor .NET Framework 4.6.2 en hoger. U kunt nu WebP - afbeeldingen in documenten lezen en invoegen, evenals afbeeldingen opslaan in WebP - indeling.

Houd er rekening mee dat WebP momenteel alleen beschikbaar is in .NET Standard en .NET Framework v4.6.2 en hoger.

### Rendering en afdrukken

#### Stroke Color Control <sup>24.1</sup>

De klasse [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) is uitgebreid met een reeks nieuwe openbare eigenschappen met betrekking tot het beheren van lijnkleuren: [ForeThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/forethemecolor/) en [BackThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/foretintandshade/) en [BackTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backtintandshade/).

#### DrawingML Grafieken API Extensie <sup>24.2 / 24.3 / 24.4</sup>

De **DrawingML Charts API** wordt nog steeds uitgebreid.

#### Lettertypen insluiten die zijn gedeclareerd in @font-face regels <sup>24.4</sup>

Toegevoegd een mogelijkheid om lettertypen gedeclareerd in @font-face Regels in te sluiten in de lettertypedefinities van het resulterende document is geïntroduceerd door een nieuwe eigenschap [SupportFontFaceRules](https://reference.aspose.com/words/net/aspose.words.loading/htmlloadoptions/supportfontfacerules/) toe te voegen.

#### Werken met Glow en Reflection formatteren <sup>24.4</sup>

De mogelijkheid om te werken met gloed en reflectie opmaak voor een tekening object is geïmplementeerd.

### Documenten laden en opslaan

#### SvgSaveOptions Opgeven Tijdens Het Renderen <sup>24.2</sup>

De mogelijkheid om [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/) te specificeren tijdens het renderen is toegevoegd met behulp van de [ShapeRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) en [OfficeMathRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) methoden.

#### Lege regels behouden bij het laden van Markdown bestanden <sup>24.2</sup>

De mogelijkheid om lege regels te behouden bij het laden van Markdown - bestanden is toegevoegd.

#### Een Nieuwe TIFF Lezer / Schrijver <sup>24.3</sup>

Een nieuwe TIFF reader/writer voor Aspose.Words voor .NET Standard, .NET 6 en later is ontwikkeld. Aspose.Words voor .NET 24.3 ondersteuning toegevoegd voor het lezen van TIFF afbeeldingen met JPEG en Oude JPEG compressietypen, en ook de kwaliteit van lees-en schrijfbewerkingen aanzienlijk verbeterd.

### Ander

* De mogelijkheid om de tekst van het besturingselement `TextBox` OLE te wijzigen is geïntroduceerd door een nieuwe eigenschap [Text](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/text/) toe te voegen aan de nieuwe klasse [TextBoxControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/). <sup>24.1</sup>
* De Bibliografie bronnen public API werd geïmplementeerd door het toevoegen van een nieuwe naamruimte [Aspose.Words.Bibliography](https://reference.aspose.com/words/net/aspose.words.bibliography/) met zijn nieuwe klassen en opsommingen, en door het toevoegen van een nieuwe [Bibliography](https://reference.aspose.com/words/net/aspose.words/document/bibliography/) eigenschap aan de [Document](https://reference.aspose.com/words/net/aspose.words/document/) klasse. <sup>24.1</sup>
* Een API om de toegang tot het type leden met behulp van sjabloon syntaxis voor de `LINQ Reporting Engine` te beperken is verstrekt. <sup>24.1</sup>
* Nieuwe openbare eigenschappen [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) en [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) voor verbeterd stijlbeheer zijn toegevoegd aan de [Style](https://reference.aspose.com/words/net/aspose.words/style/) - klasse. <sup>24.2</sup>
* De functionaliteit voor het ophalen van de eigenlijke referentiemarkeertekst voor voetnoten en eindnoten is verbeterd met de Eigenschap [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) en de methode [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* Compatibiliteit met `Word 2016` grafieken voor de `LINQ Reporting Engine` is ingeschakeld. <sup>24.2</sup>
* Emulatie van binaire rasterbewerkingen voor WMF metafiles is geïmplementeerd. <sup>24.3</sup>
* De mogelijkheid om handtekeningopties voor documenten binnen **SaveOptions** te definiëren is ingeschakeld door een nieuwe [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/digitalsignaturedetails/) - klasse met nieuwe openbare leden toe te voegen, evenals door nieuwe eigenschappen toe te voegen aan de [OoxmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/docsaveoptions/) en [OdtSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/odtsaveoptions/) - klassen. <sup>24.4</sup>

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor .NET 24.1 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-1-release-notes/).

Lees meer over [Aspose.Words voor .NET 24.2 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-2-release-notes/).

Lees meer over [Aspose.Words voor .NET 24.3 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-3-release-notes/).

Lees meer over [Aspose.Words voor .NET 24.4 vrijgave](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words voor .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 breidt rendering opties, metafile rendering emulatie en markdown save Opties uit.

Aspose.Words 23.10 verbetert rendering, breidt opties voor het laden en opslaan van documenten uit en stelt gebruikers in staat om documenten op nieuwe manieren samen te voegen.

Aspose.Words 23.11 verbetert het werk met revisies, XLSX opmaak en lettertypen op grafieklegende met extra opties.

Aspose.Words 23.12 introduceert nieuwe eigenschappen en opsommingen voor het werken met PDF en OOXML documenten, evenals ondersteuning voor WebP afbeeldingen.

### Rendering en afdrukken

#### Titels van Assen aanpassen in DrawingML grafieken <sup>23.9</sup>

De mogelijkheid om astitels in DrawingML - diagrammen aan te passen is geïntroduceerd door de implementatie van een nieuwe eigenschap openbare klassen [ChartAxisTitle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxistitle/) en [Title](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxis/title/).

#### De verticale positie van lettertypen binnen een alinea bepalen <sup>23.9</sup>

Het is nu mogelijk om de verticale positie van lettertypen binnen een alinea te definiëren met behulp van de nieuwe eigenschap public [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/paragraphformat/baselinealignment/) en de nieuwe [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/baselinealignment/) opsomming.

#### Voorgrondkleurcontrole <sup>23.10</sup>

De mogelijkheid om de voorgrondkleur op te halen zonder modifiers is toegevoegd aan de [Fill](https://reference.aspose.com/words/net/aspose.words.drawing/fill/) en [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) klassen via de **BaseForeColor** eigenschap.

#### Uitbreiding van de functionaliteit van grafieken <sup>23.10</sup>

De functionaliteit van de klassen [ChartDataPointCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseries/) en [ChartFormat](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartformat/) is uitgebreid met nieuwe methoden en eigenschappen.

#### Een afbeelding automatisch aanpassen en in een vorm passen <sup>23.10</sup>

Een eenvoudige manier om een afbeelding automatisch aan te passen en in een bepaalde vorm te passen, is geboden via de nieuwe [FitImageToShape](https://reference.aspose.com/words/net/aspose.words.drawing/imagedata/fitimagetoshape/) - methode.

#### Standaard Lettertypeopmaak voor DrawingML Grafiekleggingsvermeldingen <sup>23.11</sup>

De mogelijkheid om standaard lettertypeopmaak op te geven voor legenda-items van DrawingML - diagrammen is toegevoegd via de eigenschap [Font](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartlegend/font/). Deze functie vergemakkelijkt een meer gestroomlijnde en consistente weergave voor grafiekelementen, waardoor de algehele documentesthetiek wordt verbeterd.

#### Paginalay-out opgeven bij het openen van PDF in Reader <sup>23.12</sup>

De mogelijkheid om de pagina-indeling op te geven die moet worden gebruikt bij het openen van een document in een PDF reader is toegevoegd door de introductie van een nieuwe [PageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/pagelayout/) eigenschap aan de [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) klasse en de introductie van een nieuwe [PdfPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfpagelayout/) opsomming.

### Documenten laden en opslaan

#### Een mapnaam opgeven om Afbeelding URIs in Markdownte construeren <sup>23.9</sup>

De klasse [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) is uitgebreid met de eigenschap [ImagesFolderAlias](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imagesfolderalias/), waarmee de naam kan worden opgegeven van de map die wordt gebruikt om afbeelding URIs te construeren die in het Markdown document is geschreven.

#### PDF Uitvoergrootte Verkleinen <sup>23.10</sup>

Er zijn verschillende PDF rendering optimalisaties geïmplementeerd om de uitvoergrootte te verminderen bij het gebruik van [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) instellingen.

#### Hyperlinks herkennen bij het laden van TXT documenten <sup>23.10</sup>

De functie om hyperlinks te herkennen bij het laden van TXT documenten is geïmplementeerd door een nieuwe [DetectHyperlinks](https://reference.aspose.com/words/net/aspose.words.loading/txtloadoptions/detecthyperlinks/) eigenschap toe te voegen.

### Ander

* Metafile rendering emulatie om rasterisatie grootte te bepalen is geïmplementeerd, specifiek voor WMF pen breedte en EMF cosmetische pen breedte. Om dit te bereiken werd de eigenschap **ScaleWmfFontsToMetafileSize** vervangen door de Eigenschap [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpage/) en werd de eigenschap [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpageresolution/) toegevoegd. <sup>23.9</sup>
* Een vereenvoudigde methode voor het invoegen van een document in een ander document op de huidige cursorpositie is geïntroduceerd met behulp van de methode [InsertDocumentInline](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertdocumentinline/). <sup>23.10</sup>
* De mogelijkheid om stijleigenschappen te openen en te wijzigen is toegevoegd door de introductie van de nieuwe eigenschap [Locked](https://reference.aspose.com/words/net/aspose.words/style/locked/). <sup>23.10</sup>
* Een generieke type parameter is toegevoegd aan de methoden van de [CompositeNode](https://reference.aspose.com/words/net/aspose.words/compositenode/) klasse. <sup>23.10</sup>
* Een manier om te controleren wanneer een bepaalde herziening moet worden geaccepteerd / afgewezen of niet is geïmplementeerd met behulp van de [Accept](https://reference.aspose.com/words/net/aspose.words/revisioncollection/accept/) en [Reject](https://reference.aspose.com/words/net/aspose.words/revisioncollection/reject/) methoden. Deze verbetering geeft gebruikers een betere controle over het revisieproces. <sup>23.11</sup>
* De mogelijkheid om alle secties van een document op hetzelfde XLSX werkblad te schrijven is beschikbaar via het nieuwe [XlsxSectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsectionmode/) opsommingstype en de nieuwe [SectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsaveoptions/sectionmode/) eigenschap. <sup>23.11</sup>
* Een manier om te bepalen hoe ZIP64 - opmaakextensies worden gebruikt voor OOXML - documenten is geïmplementeerd via de nieuwe Zip64Mode-eigenschap van de `OoxmlSaveOptions` - klasse en de nieuwe Zip64Mode-opsomming. <sup>23.12</sup>
* Ondersteuning voor WebP image is geïntroduceerd. Houd er rekening mee dat deze functie alleen beschikbaar is voor .NetStandart en .NET6+ versies. <sup>23.12</sup>

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor .NET 23.9 vrijgave](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-9-release-notes/).

Lees meer over [Aspose.Words voor .NET 23.10 vrijgave](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-10-release-notes/).

Lees meer over [Aspose.Words voor .NET 23.11 vrijgave](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-11-release-notes/).

Lees meer over [Aspose.Words voor .NET 23.12 vrijgave](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words voor .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 verbetert de mogelijkheid om te werken met grafiekreeksgegevens en de mogelijkheid om te werken met ODT documenten, evenals het verbeteren van kop-en voetteksten en hun tekstomloop.

Aspose.Words 23.6 breidt weergaveopties uit, voegt een nieuwe exportnotatie toe, verbetert LINQ rapportage en LowCode tools.

Aspose.Words 23.7 verbetert de rapportagemogelijkheden, voegt een nieuwe exportindeling toe en introduceert wijzigingen in het werken met tabellen en digitale handtekeningen.

Aspose.Words 23.8 breidt de mogelijkheden van verschillende indelingen uit, verbetert de weergave en voegt nieuwe opties toe voor het werken met velden.

### Ondersteunde Formaten

* Vanaf versie 23.6 is het mogelijk om een document op te slaan in XLSX - indeling. Nu kunt u uw documenten converteren naar Excel-formaat. <sup>23.6</sup>
* Vanaf versie 23.7 is het mogelijk om een documentpagina of-vorm op te slaan in EPS - Indeling. <sup>23.7</sup>

### Nieuwe Formaatfuncties

* De functionaliteit voor het automatisch genereren van inhoudsopgave (TOC) voor MOBI documenten is geïntroduceerd. <sup>23.8</sup>
* De [PdfEncryptionDetails](https://reference.aspose.com/words/net/aspose.words.saving/pdfencryptiondetails/pdfencryptiondetails/) constructor is uitgebreid met [PdfPermissions](https://reference.aspose.com/words/net/aspose.words.saving/pdfpermissions/). <sup>23.8</sup>
* Het vormgeven van verticale tekst voor EMF metafiles is geïmplementeerd. <sup>23.8</sup>

### Rendering en afdrukken

#### Gegevens van Grafiekreeksen ophalen en wijzigen <sup>23.5</sup>

De functie voor het verkrijgen en wijzigen van gegevens over grafiekreeksen werd geleverd door het toevoegen van:

* nieuwe klassen: [ChartXValue](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartmultilevelvalue/)
* nieuwe typen enum: [ChartXValueType](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluetype/)

#### Ondersteuning voor geavanceerde typografie <sup>23.6</sup>

Ondersteuning voor geavanceerde typografie in WMF, EMF en EMF+ rendering is toegevoegd.

#### Gekleurde inhoud op de pagina <sup>23.6</sup>

De openbare eigenschap [PageInfo.Colored](https://reference.aspose.com/words/net/aspose.words.rendering/pageinfo/colored/), die aangeeft of de pagina gekleurd is of niet, is toegevoegd.

#### Opmaak voor Grafiekgegevenslabels <sup>23.6</sup>

De mogelijkheid om opvul -, lijn-en bijletteropmaak in te stellen voor grafiekgegevenslabels is geïmplementeerd.

### Mail Merge en rapportage

#### Dynamische HTML invoeging voor LINQ rapportage-Engine <sup>23.6</sup>

Een nieuwe manier van dynamische HTML invoeging voor LINQ Reporting Engine is toegevoegd.

#### Mustache Tags Ondersteuning <sup>23.7</sup>

Mustache tags worden nu ondersteund in de [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/getregionshierarchy/) en [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/getfieldnamesforregion/#getfieldnamesforregion) methoden.

#### LINQ Syntaxisupdates Voor Het Rapporteren Van Engine Template <sup>23.7</sup>

De LINQ Reporting Engine template syntaxis ondersteunt nu de `ElementAt` en ElementAtOrDefault extensie methoden.

#### De grootte van gerenderde afbeeldingen opgeven <sup>23.8</sup>

Er is een nieuwe openbare eigenschap [ImageSize](https://reference.aspose.com/words/net/aspose.words.saving/imagesaveoptions/imagesize/) geïntroduceerd voor het opgeven van de grootte van gerenderde afbeeldingen in pixel.

#### Witruimtes behouden voor JSON tekenreekswaarden - LINQ <sup>23.8</sup>

Er is een optie toegevoegd aan de LINQ Reporting Engine om witruimtes voor JSON string waarden te behouden.

### LowCode <sup>23.6</sup>

Er zijn nieuwe LowCode - methoden toegevoegd om verschillende soorten documenten samen te voegen tot één uitvoerdocument.

### Ander

* Ondersteuning voor tekstwrapping in kop-en voetteksten is geïmplementeerd. <sup>23.5</sup>
* De mogelijkheid om digitale handtekeningen uit ODT documenten te verwijderen is toegevoegd via de [RemoveAllSignatures](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignatureutil/removeallsignatures/) methode. <sup>23.5</sup>
* De openbare eigenschap [PhoneticGuide](https://reference.aspose.com/words/net/aspose.words/run/phoneticguide/) om de basis-en robijntekst van de fonetische gids [Run](https://reference.aspose.com/words/net/aspose.words/run/) te verkrijgen, is toegevoegd. <sup>23.5</sup>
* De mogelijkheid om een digitale handtekeningwaarde op te halen uit een digitaal ondertekend document als een byte array is toegevoegd door een nieuwe eigenschap [SignatureValue](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignature/signaturevalue/) in te voeren. <sup>23.7</sup>
* De klassen [Row](https://reference.aspose.com/words/net/aspose.words.tables/row/) en [Cell](https://reference.aspose.com/words/net/aspose.words.tables/cell/) zijn uitgebreid met nieuwe openbare leden– [Row.NextRow](https://reference.aspose.com/words/net/aspose.words.tables/row/nextrow/), [Row.PreviousRow](https://reference.aspose.com/words/net/aspose.words.tables/row/previousrow/), [Cell.NextCell](https://reference.aspose.com/words/net/aspose.words.tables/cell/nextcell/), en [Cell.PreviousCell](https://reference.aspose.com/words/net/aspose.words.tables/cell/previouscell/). <sup>23.7</sup>
* Ondersteuning voor CITATION en BIBLIOGRAPHY velden is toegevoegd. <sup>23.8</sup>

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor .NET 23.5 vrijgave](/words/net/aspose-words-for-net-23-5-release-notes/).

Lees meer over [Aspose.Words voor .NET 23.6 vrijgave](/words/net/aspose-words-for-net-23-6-release-notes/).

Lees meer over [Aspose.Words voor .NET 23.7 vrijgave](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-7-release-notes/).

Lees meer over [Aspose.Words voor .NET 23.8 vrijgave](/words/net/aspose-words-for-net-23-8-release-notes/).

{{% /alert %}}

## Zie Ook

{{% alert color="primary" %}}

Deze pagina bevat het laatste release nieuws van de afgelopen 2 jaar. Voor meer informatie over eerdere releases, zie de [Release Notes'](https://releases.aspose.com/words/net/release-notes/) pagina ' s in de relevante secties.

{{% /alert %}}
