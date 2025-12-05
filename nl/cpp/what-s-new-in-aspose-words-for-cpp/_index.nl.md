---
title: Wat is er nieuw
second_title: Aspose.Words voor C++
articleTitle: Wat is er nieuw in Aspose.Words voor C++
linktitle: Wat is er nieuw in Aspose.Words voor C++
type: docs
description: "Aspose.Words voor C++ breidt en verbetert dagelijks. Op deze pagina kunt u meer te weten komen over de enorme en meest interessante functies van het product."
weight: 2
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nl/cpp/what-s-new-in-aspose-words-for-cpp/
timestamp: 2025-06-23-19-12-25
---

Deze pagina beschrijft de meest interessante nieuwe Aspose.Words - functies die zijn geïntroduceerd in recente releases.

## Aspose.Words voor C++ 25.5

Aspose.Words 25.5 verbetert de aanpassing van grafieken met nieuwe stylingopties en verbetert de export van Markdown door controle te bieden over hoe lege alinea ' s worden verwerkt.

### Documenten converteren, laden en opslaan

#### Lege alinea ' s exporteren naar Markdown <sup>25.5</sup>

De mogelijkheid om te bepalen hoe lege alinea ' s worden geëxporteerd naar Markdown is geïntroduceerd door de [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownemptyparagraphexportmode/) opsomming en de [EmptyParagraphExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_emptyparagraphexportmode/) eigenschap toe te voegen.

### Rendering

#### De grafiekstijl instellen <sup>25.5</sup>

De mogelijkheid om de grafiekstijl in te stellen is geïntroduceerd door de [ChartStyle](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartstyle/) opsomming en de [Style](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chart/get_style/) eigenschap toe te voegen.

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor C++ 25.5 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-5-release-notes/).

{{% /alert %}}

## Aspose.Words voor C++ 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 introduceert grammaticacontrole op basis van AI en verbetert het opslaan van documenten met geavanceerde opties voor HTML, SVG en Markdown formaten.

Aspose.Words 25.2 introduceert tekstsamenvatting met Anthropic AI modellen, voegt MsWorks formaatondersteuning toe, verbetert typografische controle en verbetert PDF structuur en lijstverwerking.

Aspose.Words 25.3 verbetert een door AI aangedreven grammaticacontrole en lettertypeselectie met de eigenschap UpdateAmbiguousTextFont, en verbetert de export van PDF bijlagen.

Aspose.Words 25.4 introduceert ondersteuning voor nieuwe papierformaten, maakt geavanceerde HTML exportcontrole mogelijk, verbetert de behandeling van watermerken en verbetert de bruikbaarheid van de LowCode API.

### AI-aangedreven functies

#### Document AI Grammaticacontrole

* De mogelijkheid om de grammatica van het verstrekte document te controleren met behulp van OpenAI generatieve modellen is geïntroduceerd door een nieuwe [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/) methode toe te voegen. <sup>25.1</sup>
* De door AI aangedreven Grammaticacontrolefunctie is bijgewerkt om alle modellen te ondersteunen die beschikbaar zijn in de [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/)-opsomming. <sup>25.3</sup>

#### Samenvatting Met Behulp Van Anthropic Generatieve Taalmodellen <sup>25.2</sup>

Tekstsamenvatting met behulp van Anthropic generatieve taalmodellen is mogelijk gemaakt door een nieuwe openbare klasse [AnthropicAiModel](https://reference.aspose.com/words/cpp/aspose.words.ai/) in te voeren.

### Low Code

#### Low Code API bruikbaarheid <sup>25.4</sup>

De bruikbaarheid van **LowCode API** is aanzienlijk verbeterd, waardoor de documentverwerking wordt vereenvoudigd en de noodzaak van herhalende code wordt verminderd.

### Ondersteunde Formaten <sup>25.2</sup>

Vanaf versie 25.2 is compatibiliteit met de nieuwe MsWorks load-indeling voor Microsoft werkdocumenten toegevoegd.

### Documenten converteren, laden en opslaan

#### Verbeterde opslag naar HTML en SVG indelingen <sup>25.1</sup>

Opslaan in HTML en SVG formaten is verbeterd door **IdPrefix** en **RemoveJavaScriptFromLinks** eigenschappen toe te voegen aan zowel de [HtmlFixedSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlfixedsaveoptions/) als [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/) klassen.

#### Stel afbeeldingsresolutie en OfficeMath uitvoermodus in bij opslaan op Markdown <sup>25.1</sup>

- Er is een nieuwe optie [ImageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imageresolution/) toegevoegd aan de klasse [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) om de afbeeldingsresolutie in te stellen.
- Een nieuwe [OfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_officemathexportmode/) optie en [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownofficemathexportmode/) opsomming zijn toegevoegd aan de [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) klasse om OfficeMath output mode in te stellen.
- De mogelijkheid om een beeldwatermerk van een stroom in te stellen is geïntroduceerd door een nieuwe overbelasting toe te voegen aan de methode [SetImage](https://reference.aspose.com/words/cpp/aspose.words/watermark/setimage/#watermarksetimageconst-systemsharedptrsystemiostream-const-systemsharedptrasposewordsimagewatermarkoptions-method). <sup>25.4</sup>

### Rendering

#### Verbeterde Typografische Controle <sup>25.2</sup>

De eigenschap [NumberSpacing](https://reference.aspose.com/words/cpp/aspose.words/font/get_numberspacing/) is toegevoegd voor verbeterde typografische controle.

#### Controle van de lettertypeselectie voor dubbelzinnige tekens <sup>25.3</sup>

Er is een nieuwe openbare eigenschap [UpdateAmbiguousTextFont](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/get_updateambiguoustextfont/) toegevoegd aan de klasse [SaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/) om de lettertypeselectie te regelen volgens de gebruikte tekencode.

#### Opties Voor Papierformaat <sup>25.4</sup>

De mogelijkheid om JIS B4 en JIS B5 papierformaten te gebruiken is geïntroduceerd door nieuwe waarden toe te voegen aan de [PaperSize](https://reference.aspose.com/words/cpp/aspose.words/papersize/) opsomming.

#### HTML Uitvoercontrole <sup>25.4</sup>

De mogelijkheid om JavaScript van hyperlink URLs te verwijderen tijdens HTML export is geïntroduceerd door de eigenschap [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlsaveoptions/get_removejavascriptfromlinks/) toe te voegen.

### Ander

* PDF logische structuur is verbeterd met ondersteuning voor TOA, BIBLIOGRAPHY en INDEX velden. <sup>25.2</sup>
* De [AddSingleLevelList](https://reference.aspose.com/words/cpp/aspose.words.lists/listcollection/addsinglelevellist/) methode is geïntroduceerd voor verbeterde lijstverwerking. <sup>25.2</sup>
* Er is een nieuwe eigenschap [AttachmentsEmbeddingMode](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/get_attachmentsembeddingmode/) toegevoegd om **EmbedAttachments** te vervangen om de export van PDF bijlagen te verbeteren. Ook zijn er nieuwe waarden toegevoegd aan de [PdfCompliance](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfcompliance/) opsomming om PDF/A versiebijlagen te ondersteunen. Bovendien worden bijlagen nu ondersteund met encryptie. <sup>25.3</sup>

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor C++ 25.1 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-1-release-notes/).

Lees meer over [Aspose.Words voor C++ 25.2 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-2-release-notes/).

Lees meer over [Aspose.Words voor C++ 25.3 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-3-release-notes/).

Lees meer over [Aspose.Words voor C++ 25.4 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words voor C++ 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduceert group shape invoeging en StructuredDocumentTag invoeging via DocumentBuilder, verbetert de weergave van radiale grafieken met graduaties, verbetert digitale handtekeningen met XAdES-EPES ondersteuning, voegt Markdown onderstrepingherkenning toe en biedt toegang tot voetnoot/eindnoot scheidingstekens.

Aspose.Words 24.10 introduceert verbeterde ActiveX control-ondersteuning met CommandButton creatie, nieuwe shape visibility control, de mogelijkheid om group shapes, verbeterde Markdown export voor tabellen, grafiekopmaak voor Pie en Doughnut grafieken, betere Big5-codering en ondersteuning voor verouderde Taiwanese lettertypen.

Aspose.Words 24.11 introduceert AI-aangedreven document samenvatting, verbeterde rendering opties, verbeterde toegang tot document eigenschappen en ActiveX control Ondertiteling.

Aspose.Words 24.12 introduceert aanpasbare data label plaatsing, Google AI-aangedreven tekstvertaling, verbeterde Mail Merge opschoonopties en nieuwe LowCode verwerkingsklassen.

### AI-aangedreven functies

#### Samenvatting van documenten met behulp van OpenAI en Google <sup>24.11</sup>

Ondersteuning voor documentsamenvatting met behulp van **OpenAI** en **Google** generatieve taalmodellen is geïntegreerd.

#### Tekstvertaling met behulp van Google ' s generatieve taalmodellen <sup>24.12</sup>

De mogelijkheid om tekst te vertalen met behulp van Google ' s generatieve taalmodellen is geïmplementeerd in Aspose.Words door de [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) methode en de [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) opsomming toe te voegen aan de [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) naamruimte.

### Low Code <sup>24.12</sup>

Nieuwe LowCode klassen zoals [Comparer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/cpp/aspose.words.lowcode/merger/), [Replacer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/cpp/aspose.words.lowcode/splitter/) enz. is geïntroduceerd en biedt een reeks methoden die de perfecte balans vinden tussen eenvoud en flexibiliteit voor documentverwerking.

### Rendering en afdrukken

#### Graduaties op radiale grafieken <sup>24.9</sup>

De weergave van graduaties op radiale grafieken is geïmplementeerd.

#### CommandButton ActiveX besturingselementen <sup>24.10</sup>

De mogelijkheid om CommandButton ActiveX besturingselementen te maken is geïntroduceerd door een nieuwe openbare methode [InsertForms2OleControl](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertforms2olecontrol/) en een nieuwe openbare klasse **Forms2OleControl** toe te voegen.

#### Control Shape Visibility <sup>24.10</sup>

Er is een nieuwe openbare eigenschap [Hidden](https://reference.aspose.com/words/cpp/aspose.words.drawing/shapebase/get_hidden/) toegevoegd om de zichtbaarheid van shapes te regelen.

#### Veranderingen in Pie en Doughnut grafieken <sup>24.10</sup>

Er zijn verschillende nieuwe openbare eigenschappen toegevoegd om Pie en Doughnut grafieken op te maken.

#### De weergave van PDF Keuzeveldranden bepalen <sup>24.11</sup>

Er is een nieuwe optie geïmplementeerd om de weergave van PDF keuzeveldranden voor formuliervelden te beheren door een nieuwe openbare optie **RenderChoiceFormFieldBorder** toe te voegen.

#### Formaatcodes voor Grafiekgegevens ophalen en instellen <sup>24.11</sup>

De mogelijkheid om formaatcodes voor grafiekgegevens te verkrijgen en in te stellen is toegevoegd door de eigenschap **FormatCode** in de klassen [ChartXValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartyvaluecollection/) en [BubbleSizeCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/bubblesizecollection/) te implementeren.

#### Histogramdiagrammen weergeven met bakken en Labels <sup>24.11</sup>

De weergave van histogrammen is verbeterd door een bepaald aantal bakken en labels toe te staan.

#### De plaatsing van Gegevenslabels aanpassen <sup>24.12</sup>

De mogelijkheid om de plaatsing van gegevenslabels aan te passen is toegevoegd door nieuwe eigenschappen toe te voegen aan de klassen [ChartDataLabel](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabel/) en [ChartDataLabelCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabelcollection/).

### Documenten converteren, laden en opslaan

#### Onderstrepen opmaak bij het laden van Markdown bestanden <sup>24.9</sup>

De optie om onderstreping te herkennen bij het laden van Markdown documenten is opgenomen door een nieuwe openbare eigenschap **ImportUnderlineFormatting** toe te voegen.

#### Tabellen exporteren als HTML bij opslaan naar Markdown <sup>24.10</sup>

Een optie om tabellen als HTML te exporteren bij het opslaan van documenten in Markdown - indeling is geïmplementeerd door een nieuwe openbare eigenschap [ExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_exportashtml/) en een opsomming [MarkdownExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownexportashtml/) toe te voegen.

#### PDF exporteren met bijgewerkte logische structuur <sup>24.11</sup>

De export van PDF is verbeterd door eigenschappen van tabeltitels op te nemen als titels van logische structuurelementen van PDF.

### Mail Merge en rapportage

#### Lege tabellen verwijderen tijdens Mail Merge <sup>24.12</sup>

Een nieuwe **RemoveEmptyTables** optie is toegevoegd aan de [MailMergeCleanupOptions](https://reference.aspose.com/words/cpp/aspose.words.mailmerging/mailmergecleanupoptions/) opsomming om Mail Merge output te verfijnen.

### Digitale Handtekeningen

#### Documenten ondertekenen met XAdES-EPES <sup>24.9</sup>

De mogelijkheid om documenten te ondertekenen met handtekeningen van XAdES-EPES Niveau XML-DSig is geïntroduceerd door een nieuwe openbare eigenschap **XmlDsigLevel** en een nieuwe openbare opsomming **XmlDsigLevel** toe te voegen.

### Ander

* Er is een nieuwe openbare methode [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/) toegevoegd aan group shapes. <sup>24.9</sup>
* Er is een nieuwe openbare methode [InsertStructuredDocumentTag](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertstructureddocumenttag/) toegevoegd om **StructuredDocumentTags** in een document in te voegen. <sup>24.9</sup>
* Openbare toegang tot voetnoot / eindnoot scheidingstekens is verschaft door het toevoegen van een paar openbare klassen en eigenschappen. <sup>24.9</sup>
* De mogelijkheid om afzonderlijke vormen, group shapes samen te groeperen en beide vormen en group shapes rechtstreeks te groeperen, is geïntroduceerd door de methode [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/) toe te voegen. <sup>24.10</sup>
* Big5 encoding handling voor TrueType cmap tabellen is verbeterd. <sup>24.10</sup>
* Ondersteuning voor verouderde Taiwanese lettertypen is verbeterd. <sup>24.10</sup>
* Voor toegang tot uitgebreide Documenteigenschappen zijn alleen-lezen eigenschappen toegevoegd aan de klasse **BuiltInDocumentProperties**. <sup>24.11</sup>
* Het instellen van bijschriften voor ActiveX besturingselementen is ingeschakeld door een nieuwe openbare setter toe te voegen aan de eigenschap **Forms2OleControl.Caption**. <sup>24.11</sup>

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor C++ 24.9 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-9-release-notes/).

Lees meer over [Aspose.Words voor C++ 24.10 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-10-release-notes/).

Lees meer over [Aspose.Words voor C++ 24.11 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-11-release-notes/).

Lees meer over [Aspose.Words voor C++ 24.12 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words Voor C++ 24.5, 24.6, 24.7

Aspose.Words 24.5 breidt opties voor assemblies uit, verbetert de rendermogelijkheden en breidt enkele andere opties uit.

Aspose.Words 24.6 verbetert de weergaveopties, verbetert de Zoek-en vergelijkingsfunctionaliteit en breidt verschillende andere functies uit.

Aspose.Words 24.7 wijzigt de manier waarop u met ActiveX werkt, breidt de weergavemogelijkheden uit en exporteert naar Markdown en XLSX indelingen.

### Ondersteunde Formaten

Vanaf versie 24.7 wordt exporteren naar PDF/UA-2 ondersteund om toegankelijkheid voor gebruikers met een handicap te garanderen.

### Rendering en afdrukken

#### Wijzigingen in grafieken, vormen en DrawingML <sup>24.5</sup>

- DrawingML effecten rendering voor SVG graphics, uitbreiding van de vorige functionaliteit beperkt tot afbeeldingen, is geïmplementeerd.
- Ondersteuning voor het maken van combo-diagrammen en het aanpassen van eigenschappen zoals gap width, overlap en bubble scale binnen reeksgroepen is geïntroduceerd door de **ChartSeriesGroup** en **ChartSeriesGroupCollection** klassen en de **SeriesGroups** eigenschap toe te voegen.
- Functionaliteit om het SoftEdge effect van shapes te manipuleren is geïmplementeerd door de **SoftEdgeFormat** klasse toe te voegen.
- De mogelijkheid om waarden van shapes aan te passen te wijzigen is geïmplementeerd door de eigenschap **AdjustmentCollection** en **Adjustment** openbare klassen en **Adjustments** toe te voegen.

#### Wijzigingen in grafieken, vormen en tekening <sup>24.6</sup>

- De kaartmogelijkheden zijn verbeterd. U kunt nu een grotere verscheidenheid aan grafieken maken, waaronder *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* grafieken, *Box & Whisker* grafieken, *Waterfalls* en *Funnels*. Hierdoor kunt u uw gegevens op een meer diverse en informatieve manier visualiseren.
- Kleurcontrole voor schaduwopmaak is verbeterd. U kunt nauwkeuriger controle krijgen over het uiterlijk van uw documenten door toegang te krijgen tot schaduwkleuren.
- Performance boost voor achtergrond rendering is verbeterd. U kunt het renderen van achtergronden met kleine elementen aanzienlijk versnellen dankzij native tegeltechnologie.
- Er zijn realistische gradiënten voor vormen toegevoegd. U kunt nu DML-vormen maken met niet-lineaire verlopen, waarbij de visuele stijl van Microsoft Word wordt nagebootst voor een meer gepolijste look.

#### Aanpassing Van Diagramgegevens <sup>24.7</sup>

De mogelijkheid om diagramgegevenslabels zoals **Orientation** en **Rotation** Aan te passen is toegevoegd.

#### Aangepaste nummer Styling Voor Lijstniveaus <sup>24.7</sup>

Er is een setter voor de openbare eigenschap [CustomNumberStyleFormat](https://reference.aspose.com/words/cpp/aspose.words.lists/listlevel/get_customnumberstyleformat/) toegevoegd. U kunt nu een aangepaste nummerstyling definiëren voor lijstniveaus.

#### Wijzigingen in het werken met ActiveX <sup>24.7</sup>

- De eigenschappen van ActiveX objecten kunnen nu worden gewijzigd, waardoor u meer controle over hun gedrag krijgt.
- De mogelijkheid om de waarde van het keuzerondje ActiveX te wijzigen om dynamische interactie mogelijk te maken, is toegevoegd.
- De mogelijkheid om een ActiveX checkbox om te schakelen naar "aangevinkt" of "niet aangevinkt" is toegevoegd.

### Documenten laden en opslaan

#### Koppelingen exporteren naar Markdown - indeling <sup>24.7</sup>

De mogelijkheid om de export van koppelingen in Markdown - indeling te beheren is toegevoegd door de implementatie van de eigenschap [LinkExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_linkexportmode/).

### Zoeken en vergelijken

#### Geavanceerde Vergelijkingsopties <sup>24.6</sup>

De mogelijkheid om data-analyse workflows te stroomlijnen met verbeterde vergelijkingsfunctionaliteit is toegevoegd. Dit omvat een nieuwe optie **IgnoreStoreItemId** en een vernieuwde interface voor geavanceerde vergelijkingen.

### Ander

- De functie om lege pagina ' s uit een document te verwijderen is geïmplementeerd door de methode [RemoveBlankPages](https://reference.aspose.com/words/cpp/aspose.words/document/removeblankpages/) toe te voegen. <sup>24.5</sup>
- De mogelijkheid om te controleren op de aanwezigheid van VBA macro ' s zonder een document te laden, is geleverd door de eigenschap **HasMacros** toe te voegen. <sup>24.5</sup>
- Er is een nieuwe eigenschap **DateTimeUtc** toegevoegd – Dit biedt een nauwkeuriger tijdstempel voor opmerkingen, waardoor de organisatie en traceerbaarheid worden verbeterd. <sup>24.6</sup>
- De DateTime-indeling wordt nu automatisch gedetecteerd voor naadloze export naar XLSX - indeling. <sup>24.7</sup>
- De openbare eigenschap [IsProtected](https://reference.aspose.com/words/cpp/aspose.words.vba/vbaproject/get_isprotected/), waarmee u kunt controleren of een VBA - project is beschermd, is toegevoegd. <sup>24.7</sup>

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor C++ 24.5 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-5-release-notes/).

Lees meer over [Aspose.Words voor C++ 24.6 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-6-release-notes/).

Lees meer over [Aspose.Words voor C++ 24.7 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-7-release-notes/).

{{% /alert %}}

## Aspose.Words voor C++ 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 verbetert de ervaring met het beheren van lijnkleuren, verbetert OLE objecten en introduceert een nieuwe Bibliografie bronnen openbaar API.

Aspose.Words 24.2 Uitgebreide grafieken API en stijlbeheer. Deze versie van Aspose.Words introduceerde ook de mogelijkheid om SvgSaveOptions te specificeren tijdens het renderen, flexibeler controle laden van Markdown bestanden en werken met referentietekst voor voetnoten en eindnoten.

Aspose.Words 24.3 introduceert emulatie van binaire rasterbewerkingen voor WMF metafiles en blijft ook de grafieken API uitbreiden.

Aspose.Words 24.4 verbetert sommige weergaveopties en verbetert het werken met digitale handtekeningen.

### Rendering en afdrukken

#### Stroke Color Control <sup>24.1</sup>

De klasse [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) is uitgebreid met een reeks nieuwe openbare eigenschappen met betrekking tot het beheren van lijnkleuren: [ForeThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_forethemecolor/) en [BackThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_foretintandshade/) en [BackTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backtintandshade/).

#### DrawingML Grafieken API Extensie <sup>24.2 / 24.3 / 24.4</sup>

De **DrawingML Charts API** wordt nog steeds uitgebreid.

#### Lettertypen insluiten die zijn gedeclareerd in @font-face regels <sup>24.4</sup>

Toegevoegd een mogelijkheid om lettertypen gedeclareerd in @font-face Regels in te sluiten in de lettertypedefinities van het resulterende document is geïntroduceerd door een nieuwe eigenschap [SupportFontFaceRules](https://reference.aspose.com/words/cpp/aspose.words.loading/htmlloadoptions/get_supportfontfacerules/) toe te voegen.

#### Werken met Glow en Reflection formatteren <sup>24.4</sup>

De mogelijkheid om te werken met gloed en reflectie opmaak voor een tekening object is geïmplementeerd.

### Documenten laden en opslaan

#### SvgSaveOptions Opgeven Tijdens Het Renderen <sup>24.2</sup>

De mogelijkheid om [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/) te specificeren tijdens het renderen is toegevoegd met behulp van de [ShapeRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) en [OfficeMathRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) methoden.

#### Lege regels behouden bij het laden van Markdown bestanden <sup>24.2</sup>

De mogelijkheid om lege regels te behouden bij het laden van Markdown - bestanden is toegevoegd.

### Ander

- De mogelijkheid om de tekst van het besturingselement `TextBox` OLE te wijzigen is geïntroduceerd door een nieuwe eigenschap **Text** toe te voegen aan de nieuwe klasse **TextBoxControl**. <sup>24.1</sup>
- De Bibliografie bronnen public API werd geïmplementeerd door het toevoegen van een nieuwe naamruimte [Aspose.Words.Bibliography](https://reference.aspose.com/words/cpp/aspose.words.bibliography/) met zijn nieuwe klassen en opsommingen, en door het toevoegen van een nieuwe [Bibliography](https://reference.aspose.com/words/cpp/aspose.words/document/get_bibliography/) eigenschap aan de [Document](https://reference.aspose.com/words/cpp/aspose.words/document/) klasse. <sup>24.1</sup>
- Nieuwe openbare eigenschappen [Priority](https://reference.aspose.com/words/cpp/aspose.words/style/get_priority/), [UnhideWhenUsed](https://reference.aspose.com/words/cpp/aspose.words/style/get_unhidewhenused/) en [SemiHidden](https://reference.aspose.com/words/cpp/aspose.words/style/get_semihidden/) voor verbeterd stijlbeheer zijn toegevoegd aan de [Style](https://reference.aspose.com/words/cpp/aspose.words/style/) - klasse. <sup>24.2</sup>
- De functionaliteit voor het ophalen van de eigenlijke referentiemarkeertekst voor voetnoten en eindnoten is verbeterd met de Eigenschap [ActualReferenceMark](https://reference.aspose.com/words/cpp/aspose.words.notes/footnote/get_actualreferencemark/) en de methode [UpdateActualReferenceMarks](https://reference.aspose.com/words/cpp/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
- Emulatie van binaire rasterbewerkingen voor WMF metafiles is geïmplementeerd. <sup>24.3</sup>
- De mogelijkheid om handtekeningopties voor documenten binnen **SaveOptions** te definiëren is ingeschakeld door een nieuwe **DigitalSignatureDetails** - klasse met nieuwe openbare leden toe te voegen, evenals door nieuwe eigenschappen toe te voegen aan de [OoxmlSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/docsaveoptions/) en [OdtSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/odtsaveoptions/) - klassen. <sup>24.4</sup>

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor C++ 24.1 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-1-release-notes/).

Lees meer over [Aspose.Words voor C++ 24.2 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-2-release-notes/).

Lees meer over [Aspose.Words voor C++ 24.3 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-3-release-notes/).

Lees meer over [Aspose.Words voor C++ 24.4 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words voor C++ 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 breidt rendering opties, metafile rendering emulatie en markdown save Opties uit.

Aspose.Words 23.10 verbetert rendering, breidt opties voor het laden en opslaan van documenten uit en stelt gebruikers in staat om documenten op nieuwe manieren samen te voegen.

Aspose.Words 23.11 verbetert het werk met revisies, XLSX opmaak en lettertypen op grafieklegende met extra opties.

Aspose.Words 23.12 introduceert nieuwe eigenschappen en opsommingen voor het werken met PDF en OOXML documenten, evenals ondersteuning voor WebP afbeeldingen.

### Rendering en afdrukken

#### Titels van Assen aanpassen in DrawingML grafieken <sup>23.9</sup>

De mogelijkheid om astitels in DrawingML - diagrammen aan te passen is geïntroduceerd door de implementatie van een nieuwe eigenschap openbare klasse **ChartAxisTitle** en [Title](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartaxis/get_title/).

#### De verticale positie van lettertypen binnen een alinea bepalen <sup>23.9</sup>

Het is nu mogelijk om de verticale positie van lettertypen binnen een alinea te definiëren met behulp van de nieuwe eigenschap public [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/paragraphformat/get_baselinealignment/) en de nieuwe [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/baselinealignment/) opsomming.

#### Voorgrondkleurcontrole <sup>23.10</sup>

De mogelijkheid om de voorgrondkleur op te halen zonder modifiers is toegevoegd aan de [Fill](https://reference.aspose.com/words/cpp/aspose.words.drawing/fill/) en [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) klassen via de **BaseForeColor** eigenschap.

#### Uitbreiding van de functionaliteit van grafieken <sup>23.10</sup>

De functionaliteit van de klassen [ChartDataPointCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartseries/) en [ChartFormat](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartformat/) is uitgebreid met nieuwe methoden en eigenschappen.

#### Een afbeelding automatisch aanpassen en in een vorm passen <sup>23.10</sup>

Een eenvoudige manier om een afbeelding automatisch aan te passen en in een bepaalde vorm te passen, is geboden via de nieuwe [FitImageToShape](https://reference.aspose.com/words/cpp/aspose.words.drawing/imagedata/fitimagetoshape/) - methode.

#### Standaard Lettertypeopmaak voor DrawingML Grafiekleggingsvermeldingen <sup>23.11</sup>

De mogelijkheid om standaard lettertypeopmaak op te geven voor legenda-items van DrawingML - diagrammen is toegevoegd via de eigenschap [Font](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartlegend/get_font/). Deze functie vergemakkelijkt een meer gestroomlijnde en consistente weergave voor grafiekelementen, waardoor de algehele documentesthetiek wordt verbeterd.

#### Paginalay-out opgeven bij het openen van PDF in Reader <sup>23.12</sup>

De mogelijkheid om de pagina-indeling op te geven die moet worden gebruikt bij het openen van een document in een PDF reader is toegevoegd door de introductie van een nieuwe **PageLayout** eigenschap in de [PdfSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/) klasse en de introductie van een nieuwe **PdfPageLayout** opsomming.

### Documenten laden en opslaan

#### Een mapnaam opgeven om Afbeelding URIs in Markdownte construeren <sup>23.9</sup>

De klasse [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) is uitgebreid met de eigenschap [ImagesFolderAlias](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imagesfolderalias/), waarmee de naam kan worden opgegeven van de map die wordt gebruikt om afbeelding URIs te construeren die in het Markdown document is geschreven.

#### PDF Uitvoergrootte Verkleinen <sup>23.10</sup>

Er zijn verschillende PDF rendering optimalisaties geïmplementeerd om de uitvoergrootte te verminderen bij het gebruik van [OptimizeOutput](https://reference.aspose.com/words/cpp/aspose.words.saving/fixedpagesaveoptions/get_optimizeoutput/) instellingen.

#### Hyperlinks herkennen bij het laden van TXT documenten <sup>23.10</sup>

De functie om hyperlinks te herkennen bij het laden van TXT documenten is geïmplementeerd door een nieuwe [DetectHyperlinks](https://reference.aspose.com/words/cpp/aspose.words.loading/txtloadoptions/get_detecthyperlinks/) eigenschap toe te voegen.

### Ander

- Metafile rendering emulatie om rasterisatie grootte te bepalen is geïmplementeerd, specifiek voor WMF pen breedte en EMF cosmetische pen breedte. Om dit te bereiken werd de eigenschap **ScaleWmfFontsToMetafileSize** vervangen door de Eigenschap [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpage/) en werd de eigenschap [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpageresolution/) toegevoegd. <sup>23.9</sup>
* Een vereenvoudigde methode voor het invoegen van een document in een ander document op de huidige cursorpositie is geïntroduceerd met behulp van de methode [InsertDocumentInline](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertdocumentinline/). <sup>23.10</sup>
* De mogelijkheid om stijleigenschappen te openen en te wijzigen is toegevoegd door de introductie van de nieuwe eigenschap [Locked](https://reference.aspose.com/words/cpp/aspose.words/style/get_locked/). <sup>23.10</sup>
* Een generieke type parameter is toegevoegd aan de methoden van de [CompositeNode](https://reference.aspose.com/words/cpp/aspose.words/compositenode/) klasse. <sup>23.10</sup>
* Een manier om te controleren wanneer een bepaalde herziening moet worden geaccepteerd / afgewezen of niet is geïmplementeerd met behulp van de [Accept](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/accept/) en [Reject](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/reject/) methoden. Deze verbetering geeft gebruikers een betere controle over het revisieproces. <sup>23.11</sup>
* De mogelijkheid om alle secties van een document op hetzelfde XLSX werkblad te schrijven is beschikbaar via het nieuwe [XlsxSectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsectionmode/) opsommingstype en de nieuwe [SectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsaveoptions/get_sectionmode/) eigenschap. <sup>23.11</sup>
* Een manier om te bepalen hoe ZIP64 - opmaakextensies worden gebruikt voor OOXML - documenten is geïmplementeerd via de nieuwe Zip64Mode-eigenschap van de `OoxmlSaveOptions` - klasse en de nieuwe Zip64Mode-opsomming. <sup>23.12</sup>
* Ondersteuning voor WebP image is geïntroduceerd. Houd er rekening mee dat deze functie alleen beschikbaar is voor .NetStandart en .NET6+ versies. <sup>23.12</sup>

{{% alert color="primary" %}}

Lees meer over [Aspose.Words voor C++ 23.9 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-9-release-notes/).
Lees meer over [Aspose.Words voor C++ 23.10 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-10-release-notes/).
Lees meer over [Aspose.Words voor C++ 23.11 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-11-release-notes/).
Lees meer over [Aspose.Words voor C++ 23.12 Release Notes](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-12-release-notes/).

{{% /alert %}}

## Zie Ook

{{% alert color="primary" %}}

Deze pagina bevat het laatste release nieuws van de afgelopen 2 jaar. Voor meer informatie over eerdere releases, zie de [Release Notes'](https://releases.aspose.com/words/cpp/release-notes/) pagina ' s in de relevante secties.

{{% /alert %}}
