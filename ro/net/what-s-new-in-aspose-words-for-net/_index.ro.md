---
title: Ce este nou
second_title: Aspose.Words pentru .NET
articleTitle: Ce este nou în Aspose.Words pentru .NET
linktitle: Ce este nou în Aspose.Words pentru .NET
type: docs
description: "Aspose.Words pentru .NET extinde și îmbunătățește zilnic. Pe această pagină, puteți afla despre caracteristicile uriașe și cele mai interesante ale produsului."
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ro/net/what-s-new-in-aspose-words-for-net/
timestamp: 2025-06-23-21-02-49
---

Această pagină descrie cele mai interesante caracteristici noi Aspose.Words introduse în versiunile recente.

## Aspose.Words Pentru .NET 25.5, 25.6

Aspose.Words 25.5 îmbunătățește personalizarea graficului cu noi opțiuni de stil și îmbunătățește Markdown exportul oferind control asupra modului în care sunt tratate paragrafele goale.

Aspose.Words 25.6 îmbunătățește precizia de redare și caracteristicile de vizualizare prin introducerea opțiunilor avansate de export de imagini, îmbunătățirea manipulării MathML și o mai bună reprezentare a diagramelor.

### Conversia, încărcarea și salvarea documentelor

#### Exportați paragrafe goale în Markdown <sup>25.5</sup>

Abilitatea de a controla modul în care paragrafele goale sunt exportate în Markdown a fost introdusă prin adăugarea enumerării [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownemptyparagraphexportmode/) și a proprietății [EmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/emptyparagraphexportmode/).

#### Exportați documente cu mai multe pagini în formate de imagine Raster <sup>25.6</sup>

Capacitatea de a exporta documente cu mai multe pagini în formate de imagine raster (cum ar fi PNG și JPEG) cu [customizable layouts](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/)-orizontală, verticală sau grilă – a fost introdusă prin extinderea funcționalității de export de imagini.

### Redare

#### Setarea stilului graficului <sup>25.5</sup>

Abilitatea de a seta stilul graficului a fost introdusă prin adăugarea enumerării [ChartStyle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartstyle/) și a proprietății [Style](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/style/).

#### Redarea liniilor conectorului în expresii MathML  <sup>25.6</sup>

Redarea liniilor de conector în expresii MathML a fost implementată pentru a asigura o afișare mai precisă și mai consistentă vizual a formulelor matematice.

#### Redarea Legendelor pentru diagramele cascadei <sup>25.6</sup>

A fost introdusă redarea legendelor pentru ["Waterfall" charts](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriestype/), sporind transparența datelor și îmbunătățind interpretabilitatea acestor diagrame.

### Altele

* Capacitatea de a înfășura formule matematice care conțin mai multe tăieturi a fost îmbunătățită, îmbunătățind claritatea aspectului și lizibilitatea formulelor. <sup>25.6</sup>

{{% alert color="primary" %}}

Aflați mai multe despre [Aspose.Words pentru .NET 25.5 Note de lansare](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-5-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 25.6 Note de lansare](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words pentru .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 introduce verificarea gramaticală bazată pe AI și îmbunătățește salvarea documentelor cu opțiuni avansate pentru formatele HTML, SVG și Markdown.

Aspose.Words 25.2 introduce rezumarea textului cu modele Anthropic AI, adaugă suport pentru formatul MsWorks, îmbunătățește controlul tipografic și îmbunătățește structura PDF și manipularea listei.

Aspose.Words 25.3 îmbunătățește un verificator gramatical alimentat de AI și selecția fontului cu proprietatea UpdateAmbiguousTextFont, precum și îmbunătățește exportul de atașamente PDF.

Aspose.Words 25.4 introduce suport pentru noi dimensiuni de hârtie, permite controlul avansat al exporturilor HTML, îmbunătățește manipularea filigranului și îmbunătățește capacitatea de utilizare a LowCode API.

### AI - funcții alimentate

#### Document AI Verificarea Gramaticii

* Capacitatea de a verifica gramatica documentului furnizat folosind OpenAI modele generative a fost introdusă prin adăugarea unei noi metode [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/). <sup>25.1</sup>
* Funcția de verificare a gramaticii alimentată de AI a fost actualizată pentru a sprijini toate modelele disponibile în enumerarea [AiModelType](https://reference.aspose.com/words/net/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Rezumarea Folosind Anthropic Modele De Limbaj Generativ <sup>25.2</sup>

Rezumarea textului folosind Anthropic modele de limbaj generativ a fost activată prin introducerea unei noi clase publice [AnthropicAiModel](https://reference.aspose.com/words/net/aspose.words.ai/anthropicaimodel/).

### Low Code

#### Low Code API Utilizare <sup>25.4</sup>

Au fost introduse îmbunătățiri semnificative ale utilizabilității **LowCode API**, simplificând procesarea documentelor și reducând nevoia de cod repetitiv.

### Formate Acceptate <sup>25.2</sup>

Începând cu versiunea 25.2, a fost adăugată compatibilitatea cu noul format de încărcare MsWorks pentru documentele de lucru Microsoft.

### Conversia, încărcarea și salvarea documentelor

#### Salvarea îmbunătățită în formatele HTML și SVG <sup>25.1</sup>

Salvarea în formatele HTML și SVG a fost îmbunătățită prin adăugarea proprietăților **IdPrefix** și **RemoveJavaScriptFromLinks** atât la clasele [HtmlFixedSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlfixedsaveoptions/), cât și la [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/).

#### Setați rezoluția imaginii și OfficeMath modul de ieșire la salvarea în Markdown <sup>25.1</sup>

* O nouă opțiune [ImageResolution](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imageresolution/) a fost adăugată la clasa [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) pentru a seta rezoluția imaginii.
* O nouă opțiune [OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/officemathexportmode/) și [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownofficemathexportmode/) enumerare au fost și adăugate la clasa [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) pentru a seta OfficeMath modul de ieșire.
* Capacitatea de a seta un filigran de imagine dintr-un flux a fost introdusă prin adăugarea unei noi supraîncărcări la metoda [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage_2). <sup>25.4</sup>

### Redare

#### Control Tipografic Îmbunătățit <sup>25.2</sup>

Proprietatea [NumberSpacing](https://reference.aspose.com/words/net/aspose.words/font/numberspacing/) a fost adăugată pentru un control tipografic îmbunătățit.

#### Controlul selecției fonturilor pentru caractere ambigue <sup>25.3</sup>

O nouă proprietate publică [UpdateAmbiguousTextFont](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/updateambiguoustextfont/) a fost adăugată la clasa [SaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/) pentru a controla selecția fontului în funcție de codul de caractere utilizat.

#### Opțiuni Pentru Dimensiunea Hârtiei <sup>25.4</sup>

Capacitatea de a utiliza dimensiunile hârtiei JIS B4 și JIS B5 a fost introdusă prin adăugarea de noi valori la enumerarea [PaperSize](https://reference.aspose.com/words/net/aspose.words/papersize/).

#### HTML Controlul Ieșirii <sup>25.4</sup>

Abilitatea de a elimina JavaScript din hyperlink URLs în timpul exportului HTML a fost introdusă prin adăugarea proprietății [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/removejavascriptfromlinks/).

### Altele

* PDF structura logică a fost îmbunătățită cu suport pentru câmpurile TOA, BIBLIOGRAPHY și INDEX. <sup>25.2</sup>
* Metoda [AddSingleLevelList](https://reference.aspose.com/words/net/aspose.words.lists/listcollection/addsinglelevellist/) a fost introdusă pentru o mai bună gestionare a listelor. <sup>25.2</sup>
* O nouă proprietate [AttachmentsEmbeddingMode](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/attachmentsembeddingmode/) a fost adăugată pentru a înlocui **EmbedAttachments** pentru a îmbunătăți exportul de atașamente PDF. De asemenea, au fost adăugate noi valori la enumerarea [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) pentru a sprijini atașamentele versiunii PDF/A. În plus, atașamentele sunt acum acceptate cu criptare. <sup>25.3</sup>

{{% alert color="primary" %}}

Aflați mai multe despre [Aspose.Words pentru .NET 25.1 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-1-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 25.2 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-2-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 25.3 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-3-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 25.4 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words pentru .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduce group shape Inserare și StructuredDocumentTag Inserare prin DocumentBuilder, îmbunătățește randarea diagramelor radiale cu gradații, îmbunătățește semnăturile digitale cu suport XAdES-EPES, adaugă Markdown recunoașterea sublinierii și oferă acces la separatoarele de notă de subsol/notă finală.

Aspose.Words 24.10 introduce suport îmbunătățit pentru controlul ActiveX cu crearea CommandButton, Controlul vizibilității formei noi, capacitatea de a group shapes, export îmbunătățit Markdown pentru tabele, formatarea diagramelor pentru graficele Pie și Doughnut, o mai bună manipulare a codificării Big5 și suport pentru fonturile taiwaneze învechite.

Aspose.Words 24.11 introduce rezumatul documentelor alimentat de AI, opțiuni de redare îmbunătățite, acces îmbunătățit la proprietățile documentului și subtitrarea controlului ActiveX.

Aspose.Words 24.12 introduce plasarea personalizabilă a etichetelor de date, traducerea textului Google AI, opțiunile îmbunătățite de curățare Mail Merge și noile clase de procesare LowCode.

### AI - funcții alimentate

#### Rezumatul documentelor folosind OpenAI și Google <sup>24.11</sup>

Suportul pentru rezumarea documentelor folosind **OpenAI** și **Google** modele de limbaj generativ a fost integrat prin adăugarea spațiului de nume [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) cu membrii săi publici.

#### Traducerea textului folosind modelele de limbaj generativ Google <sup>24.12</sup>

Abilitatea de a traduce text folosind modelele de limbaj generativ Google a fost implementată în Aspose.Words prin adăugarea metodei [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) și a enumerării [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) la spațiul de nume [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Noi LowCode clase ca [Comparer](https://reference.aspose.com/words/net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/net/aspose.words.lowcode/splitter/) etc. a fost introdus, oferind un set de metode care ating echilibrul perfect între simplitate și flexibilitate pentru procesarea documentelor.

### Redare și imprimare

#### Gradații pe diagrame radiale <sup>24.9</sup>

A fost implementată redarea gradărilor pe diagrame radiale.

#### CommandButton ActiveX controale <sup>24.10</sup>

Abilitatea de a crea controale CommandButton ActiveX a fost introdusă prin adăugarea unei noi metode publice [InsertForms2OleControl](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertforms2olecontrol/) și a unei noi clase publice [Forms2OleControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/).

#### Controlați Vizibilitatea Formei <sup>24.10</sup>

O nouă proprietate publică [Hidden](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/hidden/) a fost adăugată pentru a controla vizibilitatea formelor.

#### Modificări în graficele Pie și Doughnut <sup>24.10</sup>

Mai multe proprietăți publice noi au fost adăugate la graficele format Pie și Doughnut.

#### Controlați redarea PDF frontiere câmp formular alegere <sup>24.11</sup>

O nouă opțiune pentru a controla redarea PDF choice form field borders a fost implementată prin adăugarea unei noi opțiuni publice [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/renderchoiceformfieldborder/).

#### Obțineți și setați codurile de Format pentru datele grafice <sup>24.11</sup>

Abilitatea de a obține și seta coduri de format pentru datele grafice a fost adăugată prin implementarea proprietății [FormatCode](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/formatcode/) în clasele [ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/) și [BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/).

#### Render diagrame histograma cu pubele și etichete <sup>24.11</sup>

Histograma diagramă De redare a fost îmbunătățită prin a permite un anumit număr de containere și etichete.

#### Personalizați plasarea etichetelor de date <sup>24.12</sup>

Abilitatea de a personaliza plasarea etichetelor de date a fost adăugată prin introducerea de noi proprietăți în clasele [ChartDataLabel](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabel/) și [ChartDataLabelCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Conversia, încărcarea și salvarea documentelor

#### Subliniați formatarea la încărcarea fișierelor Markdown <sup>24.9</sup>

Opțiunea de a recunoaște formatarea sublinierii la încărcarea documentelor Markdown a fost încorporată prin adăugarea unei noi proprietăți publice [ImportUnderlineFormatting](https://reference.aspose.com/words/net/aspose.words.loading/markdownloadoptions/importunderlineformatting/).

#### Exportarea tabelelor ca HTML la salvarea în Markdown <sup>24.10</sup>

O opțiune de a exporta tabele ca HTML la salvarea documentelor în format Markdown a fost implementată prin adăugarea unei noi proprietăți publice [ExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/exportashtml/) și a unei enumerări [MarkdownExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownexportashtml/).

#### Export PDF cu structură logică actualizată <sup>24.11</sup>

PDF exportul a fost îmbunătățit prin includerea proprietăților titlului tabelului ca PDF titluri de elemente de structură logică.

### Mail Merge și raportare

#### Eliminați tabelele goale în timpul Mail Merge <sup>24.12</sup>

O nouă opțiune **RemoveEmptyTables** a fost adăugată la enumerarea [MailMergeCleanupOptions](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmergecleanupoptions/) pentru a rafina ieșirea Mail Merge.

### Semnături Digitale

#### Semnați documente cu XAdES-EPES <sup>24.9</sup>

Abilitatea de a semna documente cu XAdES-EPES Nivel XML-DSig semnături a fost introdusă prin adăugarea unei noi proprietăți publice [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/signoptions/xmldsiglevel/) și a unei noi enumerări publice [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/xmldsiglevel/).

### Altele

* O nouă metodă publică [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/) a fost adăugată la group shapes. <sup>24.9</sup>
* O nouă metodă publică [InsertStructuredDocumentTag](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertstructureddocumenttag/) a fost adăugată pentru a insera **StructuredDocumentTags** într-un document. <sup>24.9</sup>
* Accesul Public la separatoarele de note de subsol/note de final a fost asigurat prin adăugarea câtorva clase și proprietăți publice. <sup>24.9</sup>
* Capacitatea de a grupa forme individuale, group shapes împreună și de a grupa direct ambele forme și group shapes a fost introdusă prin adăugarea metodei [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/#insertgroupshape_1). <sup>24.10</sup>
* Manipularea codificării Big5 pentru TrueType tabele cmap a fost îmbunătățită. <sup>24.10</sup>
* Suportul pentru fonturile taiwaneze învechite a fost îmbunătățit. <sup>24.10</sup>
* Pentru a accesa proprietățile extinse ale documentului, proprietățile numai în citire au fost adăugate la clasa [BuiltInDocumentProperties](https://reference.aspose.com/words/net/aspose.words.properties/builtindocumentproperties/). <sup>24.11</sup>
* Setarea subtitrărilor pentru controalele ActiveX a fost activată prin adăugarea unui nou setator public la proprietatea [Forms2OleControl.Caption](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Aflați mai multe despre [Aspose.Words pentru .NET 24.9 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-9-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 24.10 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-10-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 24.11 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-11-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 24.12 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words pentru .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 extinde opțiunile pentru ansambluri, îmbunătățește capacitățile de redare și extinde alte opțiuni.

Aspose.Words 24.6 îmbunătățește opțiunile de redare, îmbunătățește funcționalitatea de căutare și comparare și extinde alte câteva caracteristici.

Aspose.Words 24.7 modifică modul în care lucrați cu ActiveX, extinde capacitățile de redare, precum și exportul în formatele Markdown și XLSX.

Aspose.Words 24.8 îmbunătățește personalizarea diagramelor cu un control precis asupra etichetelor axelor, extinde gestionarea fonturilor, îmbunătățește manipularea structurii documentelor și adaugă noi capabilități pentru exportul HTML/XAML, funcționalitatea PDF, conversia documentelor și semnăturile digitale.

### Formate Acceptate

Începând cu versiunea 24.7, exportul în PDF/UA-2 este acceptat pentru a asigura accesibilitatea utilizatorilor cu dizabilități.

### Platforme <sup>24.5</sup>

.NET 7.0/8.0 ansamblurile au fost incluse în pachetul Aspose.Words NuGet.

### Redare și imprimare

#### Modificări în diagrame, forme și DrawingML <sup>24.5</sup>

* DrawingML a fost implementată redarea efectelor pentru SVG grafică, extinzând funcționalitatea anterioară limitată la imagini.
* Suportul pentru crearea diagramelor combinate și ajustarea proprietăților, cum ar fi lățimea decalajului, suprapunerea și scala de bule în cadrul grupurilor de serii, a fost introdus prin adăugarea claselor [ChartSeriesGroup](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroup/) și [ChartSeriesGroupCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroupcollection/) și a proprietății [SeriesGroups](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/seriesgroups/).
* Funcționalitatea de manipulare a efectului SoftEdge al formelor a fost implementată prin adăugarea clasei [SoftEdgeFormat](https://reference.aspose.com/words/net/aspose.words.drawing/softedgeformat/).
* Abilitatea de a modifica valorile de ajustare a formelor a fost implementată prin adăugarea claselor publice [AdjustmentCollection](https://reference.aspose.com/words/net/aspose.words.drawing/adjustmentcollection/) și [Adjustment](https://reference.aspose.com/words/net/aspose.words.drawing/adjustment/) și a proprietății [Adjustments](https://reference.aspose.com/words/net/aspose.words.drawing/shape/adjustments/).

#### Modificări în diagrame, forme și desen <sup>24.6</sup>

* Capacitățile de cartografiere au fost îmbunătățite. Acum Puteți crea o varietate mai mare de diagrame, inclusiv *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* diagrame, *Box & Whisker* diagrame, *Waterfalls* și *Funnels*. Acest lucru vă permite să vizualizați datele într-un mod mai divers și mai informativ.
* Controlul culorilor pentru formatarea umbrelor a fost îmbunătățit. Puteți obține un control mai precis asupra aspectului documentelor dvs. accesând culorile umbrelor.
* Creșterea performanței pentru redarea fundalului a fost îmbunătățită. Puteți accelera semnificativ redarea fundalurilor care conțin elemente mici datorită tehnologiei native de placare.
* Au fost adăugate gradiente realiste pentru forme. Acum Puteți crea DML forme cu gradiente neliniare, imitând stilul vizual al Microsoft Word pentru un aspect mai lustruit.

#### Personalizarea Etichetelor De Date Grafice <sup>24.7</sup>

A fost adăugată posibilitatea de a personaliza etichetele de date grafice, cum ar fi **Orientation** și **Rotation**.

#### Styling număr personalizat pentru nivelurile de listă <sup>24.7</sup>

A fost adăugat un setter pentru proprietatea publică [CustomNumberStyleFormat](https://reference.aspose.com/words/net/aspose.words.lists/listlevel/customnumberstyleformat/). Acum Puteți defini un stil de număr personalizat pentru nivelurile listei.

#### Modificări în lucrul cu ActiveX <sup>24.7</sup>

* Proprietățile obiectelor ActiveX pot fi acum modificate, oferindu-vă mai mult control asupra comportamentului lor.
* A fost adăugată posibilitatea de a modifica valoarea controlului butonului radio ActiveX pentru a activa interacțiunea dinamică.
* A fost adăugată posibilitatea de a comuta un ActiveX checkbox la "verificat" sau "debifat".

#### Controlul asupra axei diagramei bifați etichetele orientare și rotație <sup>24.8</sup>

A fost adăugat un control precis asupra orientării și rotației etichetelor de bifare a axei diagramei pentru o personalizare mai convenabilă a diagramei – clasa [AxisTickLabels](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/) a fost extinsă cu noi proprietăți [Orientation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/orientation/) și [Rotation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/rotation/).

#### Înlocuirea Backslash-ului cu semnul Yen <sup>24.8</sup>

Exportul compatibil cu HTML și XAML pentru înlocuirea caracterului backslash cu semnul Yen a fost îmbunătățit. Pentru a realiza acest lucru, proprietatea **ReplaceBackslashWithYenSign** a fost adăugată la clasele [HtmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/) și [XamlFlowSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xamlflowsaveoptions/).

#### Utilizarea etichetelor SDT ca nume de câmpuri de formular atunci când exportați în PDF <sup>24.8</sup>

PDF exportul cu suport pentru utilizarea etichetelor SDT ca nume de câmpuri de formular a fost îmbunătățit prin adăugarea unei noi proprietăți [UseSdtTagAsFormFieldName](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/usesdttagasformfieldname/) la clasa [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/).

### Conversia, încărcarea și salvarea documentelor

#### Exportarea linkurilor în format Markdown <sup>24.7</sup>

Capacitatea de a controla exportul de link-uri în format Markdown a fost adăugată prin implementarea proprietății [LinkExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/linkexportmode/).

#### LowCode 24.8 <sup>24.8</sup>

A fost introdusă o nouă clasă [LowCode.Converter](https://reference.aspose.com/words/net/aspose.words.lowcode/converter/), concepută pentru a oferi un set de metode pentru conversia diferitelor tipuri de documente cu o singură linie de cod.

### Căutați și comparați

#### Opțiuni Avansate De Comparație <sup>24.6</sup>
A fost adăugată capacitatea de a eficientiza fluxurile de lucru de analiză a datelor cu funcționalitate îmbunătățită de comparație. Aceasta include o nouă opțiune [IgnoreStoreItemId](https://reference.aspose.com/words/net/aspose.words.comparing/advancedcompareoptions/ignorestoreitemid/) și o interfață reproiectată pentru comparații avansate.

### Altele

* Funcția de eliminare a paginilor goale dintr-un document a fost implementată prin adăugarea metodei [RemoveBlankPages](https://reference.aspose.com/words/net/aspose.words/document/removeblankpages/). <sup>24.5</sup>
* Capacitatea de a verifica prezența macrocomenzilor VBA fără a încărca un document a fost furnizată prin adăugarea proprietății [HasMacros](https://reference.aspose.com/words/net/aspose.words/fileformatinfo/hasmacros/). <sup>24.5</sup>
* Păstrarea numerotare sursă în timp ce inserarea unui document folosind LINQ motor de raportare este acum susținută. <sup>24.5</sup>
* A fost adăugată o nouă proprietate [DateTimeUtc](https://reference.aspose.com/words/net/aspose.words/comment/datetimeutc/) - Aceasta oferă un marcaj de timp mai precis pentru comentarii, îmbunătățind organizarea și trasabilitatea. <sup>24.6</sup>
* Motorul de raportare LINQ a fost îmbunătățit. S-a făcut eliminarea selectivă a paragrafelor goale și definirea mesajelor personalizate pentru membrii obiectelor lipsă, ceea ce a dus la rapoarte mai curate și mai informative. <sup>24.6</sup>
* Formatul datetime este acum detectat automat pentru export fără sudură în format XLSX. <sup>24.7</sup>
* Proprietatea publică [IsProtected](https://reference.aspose.com/words/net/aspose.words.vba/vbaproject/isprotected/), care vă permite să verificați dacă un proiect VBA este protejat, a fost adăugat. <sup>24.7</sup>
* Informațiile despre fonturi au fost extinse cu proprietatea **EmbeddingLicensingRights** adăugată la clasele [FontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/fontinfo/) și [PhysicalFontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* A fost adăugată o modalitate de a șterge eficient anteturile și subsolurile secțiunilor, păstrând în același timp filigranele, pentru a lucra mai precis cu structura documentelor. Pentru a șterge anteturile și subsolurile secțiunilor, utilizați noua metodă publică [ClearHeadersFooters](https://reference.aspose.com/words/net/aspose.words/section/clearheadersfooters/). <sup>24.8</sup>
* Semnarea digitală a documentelor XPS folosind [XpsSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/) a fost activată – o nouă proprietate [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/digitalsignaturedetails/) a fost adăugată în acest scop. <sup>24.8</sup>

{{% alert color="primary" %}}

Aflați mai multe despre [Aspose.Words pentru .NET 24.5 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-5-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 24.6 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-6-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 24.7 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-7-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 24.8 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words pentru .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 îmbunătățește experiența în ceea ce privește gestionarea culorilor cursei, îmbunătățește obiectele OLE și raportarea LINQ, precum și introduce un nou `Bibliography Sources` public API.

Aspose.Words 24.2 diagrame extinse API, gestionarea stilului și LINQ opțiuni. Această versiune a Aspose.Words a introdus, de asemenea, capacitatea de a specifica SvgSaveOptions în timpul redării, controlul mai flexibil al încărcării fișierelor Markdown și lucrul cu textul de referință pentru notele de subsol și notele de final.

Aspose.Words 24.3 introduce un nou TIFF cititor / scriitor și emularea operațiilor raster binare pentru WMF metafișiere. Aspose.Words 24.3 continuă, de asemenea, să extindă graficele API.

Aspose.Words 24.4 îmbunătățește formatele de salvare, unele opțiuni de redare, precum și îmbunătățește lucrul cu semnăturile digitale.

### Formate Acceptate <sup>24.4</sup>

Formatul modern de imagine **WebP** este acum acceptat în Aspose.Words pentru .NET Framework 4.6.2 și mai sus. Acum Puteți citi și insera imagini WebP în documente, precum și puteți salva imagini în format WebP.

Vă rugăm să rețineți că WebP este disponibil în prezent numai în .NET Standard și .NET Framework V4.6.2 și mai sus.

### Redare și imprimare

#### Controlul Culorii Cursei <sup>24.1</sup>

Clasa [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) a fost extinsă cu un set de noi proprietăți publice legate de gestionarea culorilor stroke: [ForeThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/forethemecolor/) și [BackThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/foretintandshade/) și [BackTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backtintandshade/).

#### DrawingML Grafice API Extensie <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** continuă să fie extins.

#### Încorporați fonturile declarate în @font-face reguli <sup>24.4</sup>

Adaugata o capacitate de a încorpora fonturile declarate în @font-face Reguli în definițiile font documentului rezultat a fost introdus prin adăugarea unui nou [SupportFontFaceRules](https://reference.aspose.com/words/net/aspose.words.loading/htmlloadoptions/supportfontfacerules/) proprietate.

#### Lucrați cu formatarea strălucirii și reflecției <sup>24.4</sup>

A fost implementată capacitatea de a lucra cu formatarea strălucirii și reflexiei pentru un obiect de desen.

### Încărcarea și salvarea documentelor

#### Specificați SvgSaveOptions În Timpul Redării <sup>24.2</sup>

Capacitatea de a specifica [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/) în timpul randării a fost adăugată folosind [ShapeRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) și [OfficeMathRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) metode.

#### Păstrați liniile goale la încărcarea fișierelor Markdown <sup>24.2</sup>

A fost adăugată posibilitatea de a păstra liniile goale la încărcarea fișierelor Markdown.

#### Un Nou TIFF Cititor / Scriitor <sup>24.3</sup>

A fost dezvoltat un nou cititor/scriitor TIFF pentru Aspose.Words pentru .NET Standard, .NET 6 și mai târziu. Aspose.Words pentru .NET 24.3 s-a adăugat suport pentru citirea imaginilor TIFF cu tipurile de compresie JPEG și vechi JPEG și, de asemenea, a îmbunătățit semnificativ calitatea operațiilor de citire și scriere.

### Altele

* Capacitatea de a modifica textul controlului `TextBox` OLE a fost introdusă prin adăugarea unei noi proprietăți [Text](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/text/) la noua clasă [TextBoxControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/). <sup>24.1</sup>
* Bibliografia publică API a fost implementată prin adăugarea unui nou spațiu de nume [Aspose.Words.Bibliography](https://reference.aspose.com/words/net/aspose.words.bibliography/) cu noile sale clase și enumerări și prin adăugarea unei noi proprietăți [Bibliography](https://reference.aspose.com/words/net/aspose.words/document/bibliography/) la clasa [Document](https://reference.aspose.com/words/net/aspose.words/document/). <sup>24.1</sup>
* A fost furnizat un API pentru a limita accesul la membrii de tip folosind sintaxa șablonului pentru `LINQ Reporting Engine`. <sup>24.1</sup>
* Noile proprietăți publice [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) și [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) pentru gestionarea îmbunătățită a stilului au fost adăugate la clasa [Style](https://reference.aspose.com/words/net/aspose.words/style/). <sup>24.2</sup>
* Funcționalitatea de a prelua textul real al marcajului de referință pentru notele de subsol și notele de final a fost îmbunătățită cu proprietatea [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) și metoda [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* Compatibilitatea cu graficele `Word 2016` pentru `LINQ Reporting Engine` a fost activată. <sup>24.2</sup>
* A fost implementată emularea operațiilor raster binare pentru WMF metafișiere. <sup>24.3</sup>
* Capacitatea de a defini opțiunile de semnătură pentru documentele din **SaveOptions** a fost activată prin adăugarea unei noi clase [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/digitalsignaturedetails/) cu noi Membri publici, precum și prin adăugarea de noi proprietăți la clasele [OoxmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/docsaveoptions/) și [OdtSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Aflați mai multe despre [Aspose.Words pentru .NET 24.1 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-1-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 24.2 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-2-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 24.3 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-3-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 24.4 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words pentru .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 extinde opțiunile de redare, emularea De redare metafile și markdown opțiuni de salvare.

Aspose.Words 23.10 îmbunătățește redarea, extinde opțiunile pentru încărcarea și salvarea documentelor și permite utilizatorilor să îmbine documente în moduri noi.

Aspose.Words 23.11 îmbunătățește lucrul cu revizii, XLSX format și fonturi pe legenda diagramei cu opțiuni suplimentare.

Aspose.Words 23.12 introduce noi proprietăți și enumerări pentru lucrul cu documentele PDF și OOXML, precum și suport pentru imaginile WebP.

### Redare și imprimare

#### Personalizarea titlurilor axelor în DrawingML diagrame <sup>23.9</sup>

Capacitatea de a personaliza titlurile Axei în graficele DrawingML a fost introdusă prin implementarea unei noi clase publice [ChartAxisTitle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxistitle/) și [Title](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxis/title/) proprietate.

#### Determinarea poziției verticale a fonturilor într - un paragraf <sup>23.9</sup>

Acum este posibil să se definească poziția verticală a fonturilor într-un paragraf folosind noua proprietate publică [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/paragraphformat/baselinealignment/) și Noua enumerare [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/baselinealignment/).

#### Controlul Culorilor Din Prim Plan <sup>23.10</sup>

Capacitatea de a prelua culoarea din prim plan fără modificatori a fost adăugată la clasele [Fill](https://reference.aspose.com/words/net/aspose.words.drawing/fill/) și [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) prin proprietatea **BaseForeColor**.

#### Extinderea funcționalității diagramelor <sup>23.10</sup>

Funcționalitatea claselor [ChartDataPointCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseries/) și [ChartFormat](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartformat/) a fost extinsă cu noi metode și proprietăți.

#### Reglați automat și potriviți o imagine într-o formă <sup>23.10</sup>

O modalitate simplă de a regla și potrivi automat o imagine într-o anumită formă a fost furnizată prin noua metodă [FitImageToShape](https://reference.aspose.com/words/net/aspose.words.drawing/imagedata/fitimagetoshape/).

#### Formatarea implicită a fontului pentru DrawingML intrările din legenda diagramei <sup>23.11</sup>

Abilitatea de a specifica formatarea implicită a fontului pentru intrările de legendă ale graficelor DrawingML a fost adăugată prin proprietatea [Font](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartlegend/font/). Această caracteristică facilitează un aspect mai raționalizat și mai consistent pentru elementele graficului, îmbunătățind estetica generală a documentului.

#### Specificați aspectul paginii la deschiderea PDF În Reader <sup>23.12</sup>

Abilitatea de a specifica aspectul paginii care va fi utilizat la deschiderea unui document într-un cititor PDF a fost adăugată prin introducerea unei noi proprietăți [PageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/pagelayout/) la clasa [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) și introducerea unei noi enumerări [PdfPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfpagelayout/).

### Încărcarea și salvarea documentelor

#### Specificarea unui nume de Folder pentru a construi imaginea URIs în Markdown <sup>23.9</sup>

Clasa [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) a fost extinsă prin includerea proprietății [ImagesFolderAlias](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imagesfolderalias/), care permite specificarea numelui folderului folosit pentru a construi imaginea URIs scrisă în documentul Markdown.

#### Reduceți Dimensiunea De Ieșire PDF <sup>23.10</sup>

Au fost implementate diferite optimizări de redare PDF pentru a reduce dimensiunea ieșirii atunci când se utilizează setările [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/).

#### Recunoașteți Hyperlink-urile la încărcarea documentelor TXT <sup>23.10</sup>

Caracteristica de recunoaștere a hyperlink-urilor la încărcarea documentelor TXT a fost implementată prin adăugarea unei noi proprietăți [DetectHyperlinks](https://reference.aspose.com/words/net/aspose.words.loading/txtloadoptions/detecthyperlinks/).

### Altele

* A fost implementată emularea De redare Metafile pentru a determina dimensiunea rasterizării, în special pentru WMF lățimea stiloului și EMF lățimea stiloului cosmetic. Pentru a realiza acest lucru, proprietatea **ScaleWmfFontsToMetafileSize** a fost înlocuită cu proprietatea [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpage/) și proprietatea [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpageresolution/) a fost adăugată. <sup>23.9</sup>
* O metodă simplificată pentru inserarea unui document într-un alt document la poziția curentă a cursorului a fost introdusă folosind metoda [InsertDocumentInline](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertdocumentinline/). <sup>23.10</sup>
* Abilitatea de a accesa și modifica proprietățile stilului a fost adăugată prin introducerea noii proprietăți [Locked](https://reference.aspose.com/words/net/aspose.words/style/locked/). <sup>23.10</sup>
* Un parametru de tip generic a fost adăugat la metodele clasei [CompositeNode](https://reference.aspose.com/words/net/aspose.words/compositenode/). <sup>23.10</sup>
* O modalitate de a controla când o anumită revizuire ar trebui acceptată/respinsă sau nu a fost implementată prin utilizarea metodelor [Accept](https://reference.aspose.com/words/net/aspose.words/revisioncollection/accept/) și [Reject](https://reference.aspose.com/words/net/aspose.words/revisioncollection/reject/). Această îmbunătățire oferă utilizatorilor un control mai fin asupra procesului de revizuire. <sup>23.11</sup>
* Abilitatea de a scrie toate secțiunile unui document pe aceeași foaie de lucru XLSX a fost furnizată prin noul tip de enumerare [XlsxSectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsectionmode/) și noua proprietate [SectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsaveoptions/sectionmode/). <sup>23.11</sup>
* O modalitate de a controla modul în care vor fi utilizate extensiile de format ZIP64 pentru documentele OOXML a fost implementată prin noua proprietate Zip64Mode a clasei `OoxmlSaveOptions` și Noua enumerare Zip64Mode. <sup>23.12</sup>
* A fost introdus suport pentru imaginea WebP. Vă rugăm să rețineți că această caracteristică este disponibilă numai pentru .NetStandart și .NET6+ versiuni. <sup>23.12</sup>

{{% alert color="primary" %}}

Aflați mai multe despre [Aspose.Words pentru .NET 23.9 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-9-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 23.10 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-10-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 23.11 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-11-release-notes/).

Aflați mai multe despre [Aspose.Words pentru .NET 23.12 Notă De Lansare](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-12-release-notes/).

{{% /alert %}}

## Vezi Și

{{% alert color="primary" %}}

Această pagină conține cele mai recente știri de lansare din ultimii 2 ani. Pentru detalii despre versiunile anterioare, consultați [Note De Lansare](https://releases.aspose.com/words/net/release-notes/) paginile din secțiunile relevante.

{{% /alert %}}
