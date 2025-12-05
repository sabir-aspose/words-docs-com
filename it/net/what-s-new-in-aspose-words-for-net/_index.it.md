---
title: Cosa c'è di nuovo
second_title: Aspose.Wordsper .NET
articleTitle: Cosa c'è di nuovo in Aspose.Wordsper .NET
linktitle: Cosa c'è di nuovo in Aspose.Wordsper .NET
type: docs
description: "Aspose.Wordsper .NET si espande e migliora ogni giorno. In questa pagina, puoi conoscere le caratteristiche enormi e più interessanti del prodotto."
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /it/net/what-s-new-in-aspose-words-for-net/
timestamp: 2025-06-23-21-02-49
---

Questa pagina descrive le nuove funzionalità Aspose.Words più interessanti introdotte nelle ultime versioni.

## Aspose.Wordsper .NET 25.5, 25.6

Aspose.Words 25.5 migliora la personalizzazione del grafico con nuove opzioni di stile e migliora l'esportazione di Markdown offrendo il controllo su come vengono gestiti i paragrafi vuoti.

Aspose.Words 25.6 migliora la precisione di rendering e le funzionalità di visualizzazione introducendo opzioni avanzate di esportazione delle immagini, una migliore gestione di MathML e una migliore rappresentazione dei grafici.

### Conversione, caricamento e salvataggio di documenti

#### Esporta paragrafi vuoti in Markdown <sup>25.5</sup>

La possibilità di controllare il modo in cui i paragrafi vuoti vengono esportati in Markdown è stata introdotta aggiungendo l'enumerazione [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownemptyparagraphexportmode/) e la proprietà [EmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/emptyparagraphexportmode/).

#### Esportare documenti multipagina in formati di immagine Raster <sup>25.6</sup>

La possibilità di esportare documenti multipagina in formati di immagine raster (come PNG e JPEG) con [customizable layouts](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/)-Orizzontale, verticale o Griglia – è stata introdotta estendendo la funzionalità di esportazione delle immagini.

### Rendering

#### Impostazione dello stile grafico <sup>25.5</sup>

La possibilità di impostare lo stile del grafico è stata introdotta aggiungendo l'enumerazione [ChartStyle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartstyle/) e la proprietà [Style](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/style/).

#### Rendering delle linee del connettore nelle espressioni MathML  <sup>25.6</sup>

Il rendering delle linee del connettore nelle espressioni MathML è stato implementato per garantire una visualizzazione più accurata e visivamente coerente delle formule matematiche.

#### Legende di rendering per grafici a cascata <sup>25.6</sup>

È stato introdotto il rendering delle legende per ["Waterfall" charts](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriestype/), aumentando la trasparenza dei dati e migliorando l'interpretabilità di questi grafici.

### Altri

* La possibilità di avvolgere formule matematiche contenenti più barre è stata migliorata, migliorando la chiarezza del layout e la leggibilità della formula. <sup>25.6</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Words per .NET 25.5 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-5-release-notes/).

Scopri di più su [Aspose.Words per .NET 25.6 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-6-release-notes/).

{{% /alert %}}

## Aspose.Wordsper .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 introduce il controllo grammaticale basato su AI e migliora il salvataggio dei documenti con opzioni avanzate per i formati HTML, SVG e Markdown.

Aspose.Words 25.2 introduce il riepilogo del testo con i modelli Anthropic AI, aggiunge il supporto al formato MsWorks, migliora il controllo tipografico e migliora la struttura e la gestione degli elenchi PDF.

Aspose.Words 25.3 migliora un correttore grammaticale alimentato da AI e la selezione dei caratteri con la proprietà UpdateAmbiguousTextFont, oltre a migliorare l'esportazione degli allegati PDF.

Aspose.Words 25.4 introduce il supporto per nuovi formati di carta, abilita il controllo avanzato delle esportazioni HTML, migliora la gestione della filigrana e migliora l'usabilità del LowCode API.

### AI-Funzioni alimentate

#### Controllo grammaticale del documento AI

* La possibilità di controllare la grammatica del documento fornito utilizzando i modelli generativi OpenAI è stata introdotta aggiungendo un nuovo metodo [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/). <sup>25.1</sup>
* La funzione di controllo grammaticale alimentata da AI è stata aggiornata per supportare tutti i modelli disponibili nell'enumerazione [AiModelType](https://reference.aspose.com/words/net/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Riassunto utilizzando Anthropic Modelli di linguaggio generativo <sup>25.2</sup>

Il riepilogo del testo utilizzando i modelli di linguaggio generativo Anthropic è stato abilitato introducendo una nuova classe pubblica [AnthropicAiModel](https://reference.aspose.com/words/net/aspose.words.ai/anthropicaimodel/).

### Low Code

#### Low Code API Usabilità <sup>25.4</sup>

Sono stati introdotti miglioramenti significativi all'usabilità del **LowCode API**, semplificando l'elaborazione dei documenti e riducendo la necessità di codice ripetitivo.

### Formati supportati <sup>25.2</sup>

A partire dalla versione 25.2, è stata aggiunta la compatibilità con il nuovo formato di caricamento MsWorks per i documenti Works Microsoft.

### Conversione, caricamento e salvataggio di documenti

#### Migliorato il salvataggio nei formati HTML e SVG <sup>25.1</sup>

Il salvataggio nei formati HTML e SVG è stato migliorato aggiungendo le proprietà **IdPrefix** e **RemoveJavaScriptFromLinks** a entrambe le classi [HtmlFixedSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlfixedsaveoptions/) e [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/).

#### Impostare la risoluzione dell'immagine e la modalità di uscita OfficeMath Quando si salva su Markdown <sup>25.1</sup>

* Una nuova opzione [ImageResolution](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imageresolution/) è stata aggiunta alla classe [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) per impostare la risoluzione dell'immagine.
* Una nuova opzione [OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/officemathexportmode/) e l'enumerazione [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownofficemathexportmode/) sono state aggiunte alla classe [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) per impostare la modalità di output OfficeMath.
* La possibilità di impostare una filigrana di immagine da un flusso è stata introdotta aggiungendo un nuovo sovraccarico al metodo [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage_2). <sup>25.4</sup>

### Rendering

#### Controllo tipografico migliorato <sup>25.2</sup>

La proprietà [NumberSpacing](https://reference.aspose.com/words/net/aspose.words/font/numberspacing/) è stata aggiunta per migliorare il controllo tipografico.

#### Controllo della selezione dei caratteri per caratteri ambigui <sup>25.3</sup>

Una nuova proprietà pubblica [UpdateAmbiguousTextFont](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/updateambiguoustextfont/) è stata aggiunta alla classe [SaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/) per controllare la selezione del carattere in base al codice del carattere utilizzato.

#### Opzioni formato carta <sup>25.4</sup>

La possibilità di utilizzare i formati carta JIS B4 e JIS B5 è stata introdotta aggiungendo nuovi valori all'enumerazione [PaperSize](https://reference.aspose.com/words/net/aspose.words/papersize/).

#### HTML Controllo dell'uscita <sup>25.4</sup>

La possibilità di rimuovere JavaScript dal collegamento ipertestuale URLs durante l'esportazione HTML è stata introdotta aggiungendo la proprietà [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/removejavascriptfromlinks/).

### Altri

* La struttura logica di PDF è stata migliorata con il supporto per i campi TOA, BIBLIOGRAPHY e INDEX. <sup>25.2</sup>
* Il metodo [AddSingleLevelList](https://reference.aspose.com/words/net/aspose.words.lists/listcollection/addsinglelevellist/) è stato introdotto per una migliore gestione delle liste. <sup>25.2</sup>
* Una nuova proprietà [AttachmentsEmbeddingMode](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/attachmentsembeddingmode/) è stata aggiunta per sostituire **EmbedAttachments** per migliorare l'esportazione degli allegati PDF. Inoltre, sono stati aggiunti nuovi valori all'enumerazione [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) per supportare gli allegati alla versione PDF/A. Inoltre, gli allegati sono ora supportati con crittografia. <sup>25.3</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper .NET 25.1 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-1-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 25.2 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-2-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 25.3 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-3-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 25.4 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-4-release-notes/).

{{% /alert %}}

## Aspose.Wordsper .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduce l'inserimento group shape e l'inserimento StructuredDocumentTag tramite DocumentBuilder, migliora il rendering dei grafici radiali con graduazioni, migliora le firme digitali con il supporto XAdES-EPES, aggiunge il riconoscimento della sottolineatura Markdown e fornisce l'accesso ai separatori di note a piè di pagina/note di chiusura.

Aspose.Words 24.10 introduce il supporto migliorato del controllo ActiveX con la creazione di CommandButton, il nuovo controllo della visibilità delle forme, la possibilità di esportare group shapes, una migliore esportazione Markdown per le tabelle, la formattazione dei grafici per i grafici Pie e Doughnut, una migliore gestione della codifica Big5 e il supporto per i font taiwanesi obsoleti.

Aspose.Words 24.11 introduce il riepilogo del documento basato su AI, opzioni di rendering avanzate, accesso migliorato alle proprietà del documento e sottotitoli di controllo ActiveX.

Aspose.Words 24.12 introduce il posizionamento personalizzabile delle etichette dei dati, la traduzione del testo basata su Google AI, le opzioni di pulizia Mail Merge migliorate e le nuove classi di elaborazione LowCode.

### AI-Funzioni alimentate

#### Riepilogo dei documenti utilizzando OpenAI e Google <sup>24.11</sup>

Il supporto per il riepilogo dei documenti utilizzando i modelli di linguaggio generativo **OpenAI** e **Google** è stato integrato aggiungendo lo spazio dei nomi [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) con i suoi membri pubblici.

#### Traduzione del testo utilizzando i modelli linguistici generativi di Google <sup>24.12</sup>

La capacità di tradurre il testo utilizzando i modelli linguistici generativi di Google è stata implementata in Aspose.Words aggiungendo il metodo [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) e l'enumerazione [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) allo spazio dei nomi [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Nuove classi LowCode come [Comparer](https://reference.aspose.com/words/net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/net/aspose.words.lowcode/splitter/) ecc. è stato introdotto, offrendo una serie di metodi che colpiscono il perfetto equilibrio tra semplicità e flessibilità per l'elaborazione dei documenti.

### Rendering e stampa

#### Graduazioni su grafici radiali <sup>24.9</sup>

È stato implementato il rendering delle graduazioni su grafici radiali.

#### CommandButton ActiveX Controlli <sup>24.10</sup>

La possibilità di creare controlli CommandButton ActiveX è stata introdotta aggiungendo un nuovo metodo pubblico [InsertForms2OleControl](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertforms2olecontrol/) e una nuova classe pubblica [Forms2OleControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/).

#### Visibilità della forma di controllo <sup>24.10</sup>

È stata aggiunta una nuova proprietà pubblica [Hidden](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/hidden/) per controllare la visibilità delle forme.

#### Variazioni nei grafici Pie e Doughnut <sup>24.10</sup>

Diverse nuove proprietà pubbliche sono state aggiunte ai grafici format Pie e Doughnut.

#### Controllare il rendering dei bordi del campo del modulo di scelta PDF <sup>24.11</sup>

Una nuova opzione per controllare il rendering dei bordi del campo del modulo di scelta PDF è stata implementata aggiungendo una nuova opzione pubblica [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/renderchoiceformfieldborder/).

#### Ottenere e impostare i codici di formato per i dati del grafico <sup>24.11</sup>

La possibilità di ottenere e impostare i codici di formato per i dati del grafico è stata aggiunta implementando la proprietà [FormatCode](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/formatcode/) nelle classi [ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/) e [BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/).

#### Rendering di grafici istografici con contenitori ed etichette <sup>24.11</sup>

Il rendering del grafico istogramma è stato migliorato consentendo un numero specificato di contenitori ed etichette.

#### Personalizzare il posizionamento delle etichette dei dati <sup>24.12</sup>

La possibilità di personalizzare il posizionamento delle etichette dati è stata aggiunta introducendo nuove proprietà nelle classi [ChartDataLabel](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabel/) e [ChartDataLabelCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Conversione, caricamento e salvataggio di documenti

#### Formattazione sottolineata durante il caricamento dei file Markdown <sup>24.9</sup>

L'opzione per riconoscere la formattazione sottolineata durante il caricamento dei documenti Markdown è stata incorporata aggiungendo una nuova proprietà pubblica [ImportUnderlineFormatting](https://reference.aspose.com/words/net/aspose.words.loading/markdownloadoptions/importunderlineformatting/).

#### Esportazione di tabelle come HTMLquando si salva in Markdown <sup>24.10</sup>

Un'opzione per esportare tabelle come HTML quando si salvano documenti in formato Markdown è stata implementata aggiungendo una nuova proprietà pubblica [ExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/exportashtml/) e un'enumerazione [MarkdownExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownexportashtml/).

#### Esporta PDF con struttura logica aggiornata <sup>24.11</sup>

L'esportazione PDF è stata migliorata includendo le proprietà del titolo della tabella come titoli degli elementi della struttura logica PDF.

### Mail Merge e rapporti

#### Rimuovere le tabelle vuote durante Mail Merge <sup>24.12</sup>

Una nuova opzione **RemoveEmptyTables** è stata aggiunta all'enumerazione [MailMergeCleanupOptions](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmergecleanupoptions/) per perfezionare l'output Mail Merge.

### Firme digitali

#### Firma documenti con XAdES-EPES <sup>24.9</sup>

La possibilità di firmare documenti con firme di livello XAdES-EPES XML-DSig è stata introdotta aggiungendo una nuova proprietà pubblica [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/signoptions/xmldsiglevel/) e una nuova enumerazione pubblica [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/xmldsiglevel/).

### Altri

* Un nuovo metodo pubblico [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/) è stato aggiunto a group shapes. <sup>24.9</sup>
* Un nuovo metodo pubblico [InsertStructuredDocumentTag](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertstructureddocumenttag/) è stato aggiunto per inserire **StructuredDocumentTags** in un documento. <sup>24.9</sup>
* L'accesso pubblico ai separatori di note a piè di pagina/note di chiusura è stato fornito aggiungendo alcune classi e proprietà pubbliche. <sup>24.9</sup>
* La possibilità di raggruppare singole forme, group shapes insieme, e raggruppare direttamente entrambe le forme e group shapes è stata introdotta aggiungendo il metodo [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/#insertgroupshape_1). <sup>24.10</sup>
* La gestione della codifica Big5 per le tabelle cmap TrueType è stata migliorata. <sup>24.10</sup>
* Il supporto per i font taiwanesi obsoleti è stato migliorato. <sup>24.10</sup>
* Per accedere alle proprietà estese del documento, alla classe [BuiltInDocumentProperties](https://reference.aspose.com/words/net/aspose.words.properties/builtindocumentproperties/) sono state aggiunte proprietà di sola lettura. <sup>24.11</sup>
* L'impostazione delle didascalie per i controlli ActiveX è stata abilitata aggiungendo un nuovo setter pubblico alla proprietà [Forms2OleControl.Caption](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper .NET 24.9 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-9-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 24.10 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-10-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 24.11 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-11-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 24.12 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words per .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 espande le opzioni per gli assembly, migliora le capacità di rendering ed espande alcune altre opzioni.

Aspose.Words 24.6 migliora le opzioni di rendering, migliora la funzionalità di ricerca e confronto e amplia diverse altre funzionalità.

Aspose.Words 24.7 modifica il modo in cui si lavora con ActiveX, espande le capacità di rendering e esporta nei formati Markdown e XLSX.

Aspose.Words 24.8 migliora la personalizzazione dei grafici con un controllo preciso sulle etichette degli assi, espande la gestione dei font, migliora la gestione della struttura dei documenti e aggiunge nuove funzionalità per l'esportazioneHTML/XAML, la funzionalità PDF, la conversione dei documenti e le firme digitali.

### Formati supportati

A partire dalla versione 24.7, l'esportazione a PDF/UA-2 è supportata per garantire l'accessibilità per gli utenti con disabilità.

### Piattaforma <sup>24.5</sup>

.NET 7.0/8.0 gli assembly sono stati inclusi nel pacchetto Aspose.Words NuGet.

### Rendering e stampa

#### Cambiamenti in grafici, forme e DrawingML <sup>24.5</sup>

* È stato implementato il rendering degli effetti DrawingML per la grafica SVG, che estende le funzionalità precedenti limitate alle immagini.
* Il supporto per la creazione di grafici combinati e la regolazione di proprietà come larghezza spazio, sovrapposizione e scala a bolle all'interno dei gruppi di serie è stato introdotto aggiungendo le classi [ChartSeriesGroup](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroup/) e [ChartSeriesGroupCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroupcollection/) e la proprietà [SeriesGroups](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/seriesgroups/).
* La funzionalità per manipolare l'effetto SoftEdge delle forme è stata implementata aggiungendo la classe [SoftEdgeFormat](https://reference.aspose.com/words/net/aspose.words.drawing/softedgeformat/).
* La possibilità di modificare regolare i valori delle forme è stata implementata aggiungendo le classi pubbliche [AdjustmentCollection](https://reference.aspose.com/words/net/aspose.words.drawing/adjustmentcollection/) e [Adjustment](https://reference.aspose.com/words/net/aspose.words.drawing/adjustment/) e la proprietà [Adjustments](https://reference.aspose.com/words/net/aspose.words.drawing/shape/adjustments/).

#### Cambiamenti nei grafici, nelle forme e nel disegno <sup>24.6</sup>

* Le capacità di creazione di grafici sono state migliorate. È ora possibile creare una più ampia varietà di grafici, tra cui *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* grafici, *Box & Whisker* grafici, *Waterfalls* e *Funnels*. Ciò consente di visualizzare i dati in modo più diversificato e informativo.
* Il controllo del colore per la formattazione delle ombre è stato migliorato. Puoi ottenere un controllo più preciso sull'aspetto dei tuoi documenti accedendo ai colori delle ombre.
* L'aumento delle prestazioni per il rendering in background è stato migliorato. È possibile velocizzare notevolmente il rendering di sfondi contenenti piccoli elementi grazie alla tecnologia di piastrellatura nativa.
* Sono stati aggiunti gradienti realistici per le forme. Ora è possibile creare forme DML con gradienti non lineari, imitando lo stile visivo di Microsoft Word per un aspetto più lucido.

#### Personalizzazione dell'etichetta dei dati del grafico <sup>24.7</sup>

È stata aggiunta la possibilità di personalizzare le etichette dei dati del grafico come **Orientation** e **Rotation**.

#### Stile numero personalizzato per i livelli di elenco <sup>24.7</sup>

È stato aggiunto un setter per la proprietà pubblica [CustomNumberStyleFormat](https://reference.aspose.com/words/net/aspose.words.lists/listlevel/customnumberstyleformat/). È ora possibile definire uno stile numero personalizzato per i livelli di elenco.

#### Cambiamenti nel lavoro con ActiveX <sup>24.7</sup>

* Le proprietà degli oggetti ActiveX possono ora essere modificate, dandoti un maggiore controllo sul loro comportamento.
* È stata aggiunta la possibilità di modificare il valore del controllo del pulsante di opzione ActiveX per abilitare l'interazione dinamica.
* È stata aggiunta la possibilità di attivare un ActiveX checkbox su "selezionato" o "deselezionato".

#### Controllo sull'asse del grafico Etichette di spunta Orientamento e rotazione <sup>24.8</sup>

È stato aggiunto un controllo preciso sull'orientamento e la rotazione delle etichette di spunta dell'asse del grafico per una più comoda personalizzazione del grafico: la classe [AxisTickLabels](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/) è stata estesa con le nuove proprietà [Orientation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/orientation/) e [Rotation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/rotation/).

#### Sostituzione della barra rovesciata con il segno Yen <sup>24.8</sup>

L'esportazione retrocompatibile HTML e XAML per sostituire il carattere di barra rovesciata con il segno di Yen è stata migliorata. Per ottenere ciò, la proprietà **ReplaceBackslashWithYenSign** è stata aggiunta alle classi [HtmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/) e [XamlFlowSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xamlflowsaveoptions/).

#### Utilizzo dei tag SDT come nomi dei campi modulo durante l'esportazione in PDF <sup>24.8</sup>

L'esportazione PDF con supporto per l'utilizzo di tag SDT come nomi di campi del modulo è stata migliorata aggiungendo una nuova proprietà [UseSdtTagAsFormFieldName](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/usesdttagasformfieldname/) alla classe [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/).

### Conversione, caricamento e salvataggio di documenti

#### Esportazione di collegamenti in formato Markdown <sup>24.7</sup>

La possibilità di controllare l'esportazione dei collegamenti in formato Markdown è stata aggiunta attraverso l'implementazione della proprietà [LinkExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/linkexportmode/).

#### LowCode 24.8 <sup>24.8</sup>

È stata introdotta una nuova classe [LowCode.Converter](https://reference.aspose.com/words/net/aspose.words.lowcode/converter/), progettata per fornire un insieme di metodi per convertire vari tipi di documenti con una singola riga di codice.

### Cerca e confronta

#### Opzioni di confronto avanzate <sup>24.6</sup>
È stata aggiunta la possibilità di semplificare i flussi di lavoro di analisi dei dati con funzionalità di confronto migliorate. Ciò include una nuova opzione [IgnoreStoreItemId](https://reference.aspose.com/words/net/aspose.words.comparing/advancedcompareoptions/ignorestoreitemid/) e un'interfaccia ridisegnata per confronti avanzati.

### Altri

* La funzione per eliminare le pagine vuote da un documento è stata implementata aggiungendo il metodo [RemoveBlankPages](https://reference.aspose.com/words/net/aspose.words/document/removeblankpages/). <sup>24.5</sup>
* La possibilità di verificare la presenza di macro VBA senza caricare un documento è stata fornita aggiungendo la proprietà [HasMacros](https://reference.aspose.com/words/net/aspose.words/fileformatinfo/hasmacros/). <sup>24.5</sup>
* Mantenere la numerazione delle origini durante l'inserimento di un documento utilizzando il motore di reporting LINQ è ora supportato. <sup>24.5</sup>
* È stata aggiunta una nuova proprietà [DateTimeUtc](https://reference.aspose.com/words/net/aspose.words/comment/datetimeutc/), che fornisce un timestamp più preciso per i commenti, migliorando l'organizzazione e la tracciabilità. <sup>24.6</sup>
* Il motore di reporting LINQ è stato migliorato. La rimozione selettiva di paragrafi vuoti e la definizione di messaggi personalizzati per i membri di oggetti mancanti sono stati fatti, portando a rapporti più puliti e più informativi. <sup>24.6</sup>
* Il formato datetime viene ora rilevato automaticamente per l'esportazione senza interruzioni nel formato XLSX. <sup>24.7</sup>
* È stata aggiunta la proprietà pubblica [IsProtected](https://reference.aspose.com/words/net/aspose.words.vba/vbaproject/isprotected/), che consente di verificare se un progetto VBA è protetto. <sup>24.7</sup>
* Le informazioni sui font sono state espanse con la proprietà **EmbeddingLicensingRights** aggiunta alle classi [FontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/fontinfo/) e [PhysicalFontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* È stato aggiunto un modo per cancellare in modo efficiente intestazioni di sezione e piè di pagina preservando le filigrane per lavorare in modo più accurato con la struttura del documento. Per cancellare intestazioni di sezione e piè di pagina, utilizzare il nuovo metodo pubblico [ClearHeadersFooters](https://reference.aspose.com/words/net/aspose.words/section/clearheadersfooters/). <sup>24.8</sup>
* È stata abilitata la firma digitale dei documenti XPS che utilizzano [XpsSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/): a tale scopo è stata aggiunta una nuova proprietà [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/digitalsignaturedetails/). <sup>24.8</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper .NET 24.5 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-5-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 24.6 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-6-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 24.7 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-7-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 24.8 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-8-release-notes/).

{{% /alert %}}

## Aspose.Wordsper .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 migliora l'esperienza di gestione dei colori dei tratti, migliora gli oggetti OLE e i rapporti LINQ e introduce un nuovo pubblico `Bibliography Sources` API.

Aspose.Words 24.2 Grafici espansi API, gestione dello stile e opzioni LINQ. Questa versione di Aspose.Words ha anche introdotto la capacità di specificare SvgSaveOptions durante il rendering, il controllo più flessibile che carica i file Markdown e lavora con il testo di riferimento per le note a piè di pagina e le note di chiusura.

Aspose.Words 24.3 introduce un nuovo lettore / scrittore TIFF ed emulazione di operazioni raster binarie per metafile WMF. Aspose.Words 24.3 continua anche ad espandere i Grafici API.

Aspose.Words 24.4 migliora il salvataggio dei formati, alcune opzioni di rendering e migliora il lavoro con le firme digitali.

### Formati supportati <sup>24.4</sup>

Il moderno formato immagine **WebP** è ora supportato in Aspose.Words per .NET Framework 4.6.2 e più in alto. Ora è possibile leggere e inserire immagini WebP nei documenti, nonché salvare le immagini in formato WebP.

Si noti che WebP è attualmente disponibile solo in .NET Standard e .NET Framework v4.6.2 e versioni successive.

### Rendering e stampa

#### Controllo del colore del tratto <sup>24.1</sup>

La classe [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) è stata estesa con una serie di nuove proprietà pubbliche relative alla gestione dei colori dei tratti: [ForeThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/forethemecolor/) e [BackThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/foretintandshade/) e [BackTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backtintandshade/).

#### DrawingML Grafici API Estensione <sup>24.2 / 24.3 / 24.4</sup>

Il **DrawingML Charts API** continua ad essere espanso.

#### Incorpora i font dichiarati nelle regole @font-face <sup>24.4</sup>

Aggiunta la possibilità di incorporare i font dichiarati nelle regole @font-face nelle definizioni dei font del documento risultante è stata introdotta aggiungendo una nuova proprietà [SupportFontFaceRules](https://reference.aspose.com/words/net/aspose.words.loading/htmlloadoptions/supportfontfacerules/).

#### Lavorare con la formattazione bagliore e riflessione <sup>24.4</sup>

È stata implementata la possibilità di lavorare con la formattazione di bagliore e riflessione per un oggetto di disegno.

### Caricamento e salvataggio dei documenti

#### Specificare SvgSaveOptions durante il rendering <sup>24.2</sup>

La capacità di specificare [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/) durante il rendering è stata aggiunta usando [ShapeRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) e [OfficeMathRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) metodi.

#### Conserva le righe vuote durante il caricamento dei file Markdown <sup>24.2</sup>

È stata aggiunta la possibilità di conservare le righe vuote durante il caricamento dei file Markdown.

#### Un nuovo TIFF Lettore / scrittore <sup>24.3</sup>

È stato sviluppato un nuovo lettore/scrittore TIFF per Aspose.Words per .NET Standard, .NET 6 e versioni successive. Aspose.Wordsper .NET 24.3 aggiunto il supporto per la lettura di immagini TIFF con tipi di compressione JPEG e vecchi JPEG e anche migliorato significativamente la qualità delle operazioni di lettura e scrittura.

### Altri

* La possibilità di modificare il testo del controllo `TextBox` OLE è stata introdotta aggiungendo una nuova proprietà [Text](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/text/) alla nuova classe [TextBoxControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/). <sup>24.1</sup>
* La Bibliography Sources public API è stata implementata attraverso l'aggiunta di un nuovo namespace [Aspose.Words.Bibliography](https://reference.aspose.com/words/net/aspose.words.bibliography/) con le sue nuove classi ed enumerazioni, e attraverso l'aggiunta di una nuova proprietà [Bibliography](https://reference.aspose.com/words/net/aspose.words/document/bibliography/) alla classe [Document](https://reference.aspose.com/words/net/aspose.words/document/). <sup>24.1</sup>
* È stato fornito un API per limitare l'accesso ai membri di tipo utilizzando la sintassi del modello per `LINQ Reporting Engine`. <sup>24.1</sup>
* Nuove proprietà pubbliche [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) e [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) per la gestione avanzata dello stile sono state aggiunte alla classe [Style](https://reference.aspose.com/words/net/aspose.words/style/). <sup>24.2</sup>
* La funzionalità per recuperare il testo del marchio di riferimento effettivo per le note a piè di pagina e le note di chiusura è stata migliorata con la proprietà [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) e il metodo [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* La compatibilità con i grafici `Word 2016` per il `LINQ Reporting Engine` è stata abilitata. <sup>24.2</sup>
* È stata implementata l'emulazione di operazioni raster binarie per metafile WMF. <sup>24.3</sup>
* La possibilità di definire le opzioni di firma per i documenti all'interno di **SaveOptions** è stata abilitata aggiungendo una nuova classe [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/digitalsignaturedetails/) con nuovi membri pubblici, nonché aggiungendo nuove proprietà alle classi [OoxmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/docsaveoptions/) e [OdtSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper .NET 24.1 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-1-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 24.2 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-2-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 24.3 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-3-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 24.4 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-4-release-notes/).

{{% /alert %}}

## Aspose.Wordsper .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 espande le opzioni di rendering, l'emulazione di rendering metafile e le opzioni di salvataggio markdown.

Aspose.Words 23.10 migliora il rendering, espande le opzioni per il caricamento e il salvataggio dei documenti e consente agli utenti di unire i documenti in nuovi modi.

Aspose.Words 23.11 migliora il lavoro con le revisioni, il formato XLSX e i caratteri sulla legenda del grafico con opzioni aggiuntive.

Aspose.Words 23.12 introduce nuove proprietà ed enumerazioni per lavorare con i documenti PDF e OOXML, nonché il supporto per le immagini WebP.

### Rendering e stampa

#### Personalizzazione dei titoli degli assi nei grafici DrawingML <sup>23.9</sup>

La possibilità di personalizzare i titoli degli assi nei grafici DrawingML è stata introdotta dall'implementazione di una nuova proprietà public class [ChartAxisTitle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxistitle/) e [Title](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxis/title/).

#### Determinazione della posizione verticale dei caratteri all'interno di un paragrafo <sup>23.9</sup>

È ora possibile definire la posizione verticale dei font all'interno di un paragrafo utilizzando la nuova proprietà public [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/paragraphformat/baselinealignment/) e la nuova enumerazione [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/baselinealignment/).

#### Controllo del colore di primo piano <sup>23.10</sup>

La possibilità di recuperare il colore di primo piano senza modificatori è stata aggiunta alle classi [Fill](https://reference.aspose.com/words/net/aspose.words.drawing/fill/) e [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) tramite la proprietà **BaseForeColor**.

#### Espansione della funzionalità dei grafici <sup>23.10</sup>

La funzionalità delle classi [ChartDataPointCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseries/) e [ChartFormat](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartformat/) è stata ampliata con nuovi metodi e proprietà.

#### Regola e adatta automaticamente un'immagine in una forma <sup>23.10</sup>

Un modo semplice per regolare e adattare automaticamente un'immagine all'interno di una particolare forma è stato fornito attraverso il nuovo metodo [FitImageToShape](https://reference.aspose.com/words/net/aspose.words.drawing/imagedata/fitimagetoshape/).

#### Formattazione predefinita dei caratteri per le voci della legenda del grafico DrawingML <sup>23.11</sup>

La possibilità di specificare la formattazione predefinita dei caratteri per le voci di legenda dei grafici DrawingML è stata aggiunta tramite la proprietà [Font](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartlegend/font/). Questa funzione facilita un aspetto più snello e coerente per gli elementi del grafico, migliorando l'estetica complessiva del documento.

#### Specificare il layout di pagina quando si apre PDF in Reader <sup>23.12</sup>

La possibilità di specificare il layout di pagina da utilizzare quando si apre un documento in un lettore PDF è stata aggiunta attraverso l'introduzione di una nuova proprietà [PageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/pagelayout/) alla classe [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) e l'introduzione di una nuova enumerazione [PdfPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfpagelayout/).

### Caricamento e salvataggio dei documenti

#### Specificare il nome di una cartella per costruire l'immagine URIsin Markdown <sup>23.9</sup>

La classe [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) è stata espansa includendo la proprietà [ImagesFolderAlias](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imagesfolderalias/), che consente di specificare il nome della cartella utilizzata per costruire l'immagine URIs scritta nel documento Markdown.

#### Ridurre PDF Dimensione dell'output <sup>23.10</sup>

Sono state implementate varie ottimizzazioni di rendering PDF per ridurre le dimensioni dell'output quando si utilizzano le impostazioni [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/).

#### Riconoscere i collegamenti ipertestuali durante il caricamento di documenti TXT <sup>23.10</sup>

La funzione per riconoscere i collegamenti ipertestuali durante il caricamento di documenti TXT è stata implementata aggiungendo una nuova proprietà [DetectHyperlinks](https://reference.aspose.com/words/net/aspose.words.loading/txtloadoptions/detecthyperlinks/).

### Altri

* È stata implementata l'emulazione del rendering Metafile per determinare la dimensione della rasterizzazione, in particolare per WMF pen width e EMF cosmetic pen width. Per ottenere ciò, la proprietà **ScaleWmfFontsToMetafileSize** è stata sostituita con la proprietà [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpage/) e la proprietà [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpageresolution/) è stata aggiunta. <sup>23.9</sup>
* Un metodo semplificato per l'inserimento di un documento in un altro documento nella posizione corrente del cursore è stato introdotto utilizzando il metodo [InsertDocumentInline](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertdocumentinline/). <sup>23.10</sup>
* La possibilità di accedere e modificare le proprietà di stile è stata aggiunta attraverso l'introduzione della nuova proprietà [Locked](https://reference.aspose.com/words/net/aspose.words/style/locked/). <sup>23.10</sup>
* Un parametro di tipo generico è stato aggiunto ai metodi della classe [CompositeNode](https://reference.aspose.com/words/net/aspose.words/compositenode/). <sup>23.10</sup>
* Un modo per controllare quando una determinata revisione deve essere accettata / rifiutata o meno è stato implementato utilizzando i metodi [Accept](https://reference.aspose.com/words/net/aspose.words/revisioncollection/accept/) e [Reject](https://reference.aspose.com/words/net/aspose.words/revisioncollection/reject/). Questo miglioramento garantisce agli utenti un controllo più preciso sul processo di revisione. <sup>23.11</sup>
* La possibilità di scrivere tutte le sezioni di un documento sullo stesso foglio di lavoro XLSX è stata fornita tramite il nuovo tipo di enumerazione [XlsxSectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsectionmode/) e la nuova proprietà [SectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsaveoptions/sectionmode/). <sup>23.11</sup>
* Un modo per controllare come verranno utilizzate le estensioni di formato ZIP64 per i documenti OOXML è stato implementato tramite la nuova proprietà Zip64Mode della classe `OoxmlSaveOptions` e la nuova enumerazione Zip64Mode. <sup>23.12</sup>
* È stato introdotto il supporto per l'immagine WebP. Si prega di notare che questa funzione è disponibile solo per .versioni NetStandart e .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper .NET 23.9 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-9-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 23.10 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-10-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 23.11 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-11-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 23.12 Note di rilascio](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-12-release-notes/).

{{% /alert %}}

## Vedi anche

{{% alert color="primary" %}}

Questa pagina contiene le ultime notizie di rilascio degli ultimi 2 anni. Per i dettagli sulle versioni precedenti, vedere [Note di rilascio'](https://releases.aspose.com/words/net/release-notes/) pagine nelle relative sezioni.

{{% /alert %}}
