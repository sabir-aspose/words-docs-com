---
title: Cosa c'è di nuovo
second_title: Aspose.Wordsper Java
articleTitle: Cosa c'è di nuovo in Aspose.Wordsper Java
linktitle: Cosa c'è di nuovo in Aspose.Wordsper Java
type: docs
description: "Aspose.Wordsper Java si espande e migliora ogni giorno. In questa pagina, puoi conoscere le caratteristiche enormi e più interessanti del prodotto."
weight: 2
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /it/java/what-s-new-in-aspose-words-for-java/
timestamp: 2025-04-22-08-02-05
---

Questa pagina descrive le nuove funzionalità Aspose.Words più interessanti introdotte nelle ultime versioni.

## Aspose.Wordsper Java 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 introduce il controllo grammaticale basato su AI e migliora il salvataggio dei documenti con opzioni avanzate per i formati HTML, SVG e Markdown.

Aspose.Words 25.2 introduce il riepilogo del testo con i modelli Anthropic AI, aggiunge il supporto al formato MsWorks, migliora il controllo tipografico e migliora la struttura e la gestione degli elenchi PDF.

Aspose.Words 25.3 migliora un correttore grammaticale alimentato da AI e la selezione dei caratteri con la proprietà UpdateAmbiguousTextFont, oltre a migliorare l'esportazione degli allegati PDF.

Aspose.Words 25.4 introduce il supporto per nuovi formati di carta, abilita il controllo avanzato delle esportazioni HTML, migliora la gestione della filigrana e migliora l'usabilità del LowCode API.

### AI-Funzioni alimentate

#### Controllo grammaticale del documento AI

* La possibilità di controllare la grammatica del documento fornito utilizzando i modelli generativi OpenAI è stata introdotta aggiungendo un nuovo metodo [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions). <sup>25.1</sup>
* La funzione di controllo grammaticale alimentata da AI è stata aggiornata per supportare tutti i modelli disponibili nell'enumerazione [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). <sup>25.3</sup>

#### Riassunto utilizzando Anthropic Modelli di linguaggio generativo <sup>25.2</sup>

Il riepilogo del testo utilizzando i modelli di linguaggio generativo Anthropic è stato abilitato introducendo una nuova classe pubblica [AnthropicAiModel](https://reference.aspose.com/words/java/com.aspose.words/anthropicaimodel/).

### Low Code

#### Low Code API Usabilità <sup>25.4</sup>

Sono stati introdotti miglioramenti significativi all'usabilità del **LowCode API**, semplificando l'elaborazione dei documenti e riducendo la necessità di codice ripetitivo.

### Formati supportati <sup>25.2</sup>

A partire dalla versione 25.2, è stata aggiunta la compatibilità con il nuovo formato di caricamento MsWorks per i documenti Works Microsoft.

### Conversione, caricamento e salvataggio di documenti

#### Migliorato il salvataggio nei formati HTML e SVG <sup>25.1</sup>

Il salvataggio nei formati HTML e SVG è stato migliorato aggiungendo le proprietà **IdPrefix** e **RemoveJavaScriptFromLinks** a entrambe le classi [HtmlFixedSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlfixedsaveoptions/) e [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/).

#### Impostare la risoluzione dell'immagine e la modalità di uscita OfficeMath Quando si salva su Markdown <sup>25.1</sup>

* Una nuova opzione [ImageResolution](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImageResolution) è stata aggiunta alla classe [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) per impostare la risoluzione dell'immagine.
* Una nuova opzione [OfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getOfficeMathExportMode) e l'enumerazione [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownofficemathexportmode/) sono state aggiunte alla classe [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) per impostare la modalità di output OfficeMath.
* La possibilità di impostare una filigrana di immagine da un flusso è stata introdotta aggiungendo un nuovo sovraccarico al metodo [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.io.InputStream-com.aspose.words.ImageWatermarkOptions). <sup>25.4</sup>

### Rendering

#### Controllo tipografico migliorato <sup>25.2</sup>

La proprietà [NumberSpacing](https://reference.aspose.com/words/java/com.aspose.words/font/#getNumberSpacing) è stata aggiunta per migliorare il controllo tipografico.

#### Controllo della selezione dei caratteri per caratteri ambigui <sup>25.3</sup>

Una nuova proprietà pubblica [UpdateAmbiguousTextFont](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/#getUpdateAmbiguousTextFont) è stata aggiunta alla classe [SaveOptions](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/) per controllare la selezione del carattere in base al codice del carattere utilizzato.

#### Opzioni formato carta <sup>25.4</sup>

La possibilità di utilizzare i formati carta JIS B4 e JIS B5 è stata introdotta aggiungendo nuovi valori all'enumerazione [PaperSize](https://reference.aspose.com/words/java/com.aspose.words/papersize/).

#### HTML Controllo dell'uscita <sup>25.4</sup>

La possibilità di rimuovere JavaScript dal collegamento ipertestuale URLs durante l'esportazione HTML è stata introdotta aggiungendo la proprietà [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/#getRemoveJavaScriptFromLinks).

### Altri

* La struttura logica di PDF è stata migliorata con il supporto per i campi TOA, BIBLIOGRAPHY e INDEX. <sup>25.2</sup>
* Il metodo [AddSingleLevelList](https://reference.aspose.com/words/java/com.aspose.words/listcollection/#addSingleLevelList-int) è stato introdotto per una migliore gestione delle liste. <sup>25.2</sup>
* Una nuova proprietà [AttachmentsEmbeddingMode](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getAttachmentsEmbeddingMode) è stata aggiunta per sostituire **EmbedAttachments** per migliorare l'esportazione degli allegati PDF. Inoltre, sono stati aggiunti nuovi valori all'enumerazione [PdfCompliance](https://reference.aspose.com/words/java/com.aspose.words/pdfcompliance/) per supportare gli allegati alla versione PDF/A. Inoltre, gli allegati sono ora supportati con crittografia. <sup>25.3</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Java 25.1 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-1-release-notes/).

Scopri di più su [Aspose.Wordsper Java 25.2 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-2-release-notes/).

Scopri di più su [Aspose.Wordsper Java 25.3 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-3-release-notes/).

Scopri di più su [Aspose.Wordsper Java 25.4 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-4-release-notes/).

{{% /alert %}}

## Aspose.Wordsper Java 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduce l'inserimento group shape e l'inserimento StructuredDocumentTag tramite DocumentBuilder, migliora il rendering dei grafici radiali con graduazioni, migliora le firme digitali con il supporto XAdES-EPES, aggiunge il riconoscimento della sottolineatura Markdown e fornisce l'accesso ai separatori di note a piè di pagina/note di chiusura.

Aspose.Words 24.10 introduce il supporto migliorato del controllo ActiveX con la creazione di CommandButton, il nuovo controllo della visibilità delle forme, la possibilità di esportare group shapes, una migliore esportazione Markdown per le tabelle, la formattazione dei grafici per i grafici Pie e Doughnut, una migliore gestione della codifica Big5 e il supporto per i font taiwanesi obsoleti.

Aspose.Words 24.11 introduce il riepilogo del documento basato su AI, opzioni di rendering avanzate, accesso migliorato alle proprietà del documento e sottotitoli di controllo ActiveX.

Aspose.Words 24.12 introduce il posizionamento personalizzabile delle etichette dei dati, la traduzione del testo basata su Google AI, le opzioni di pulizia Mail Merge migliorate e le nuove classi di elaborazione LowCode.

### AI-Funzioni alimentate

#### Riepilogo dei documenti utilizzando OpenAI e Google <sup>24.11</sup>

È stato integrato il supporto per la sintesi dei documenti utilizzando modelli linguistici generativi **OpenAI** e **Google**.

#### Traduzione del testo utilizzando i modelli linguistici generativi di Google <sup>24.12</sup>

La capacità di tradurre il testo utilizzando i modelli linguistici generativi di Google è stata implementata in Aspose.Words aggiungendo il metodo [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) e l'enumerazione [Language](https://reference.aspose.com/words/java/com.aspose.words/language/).

### Low Code <sup>24.12</sup>

Nuove classi LowCode come [Comparer](https://reference.aspose.com/words/java/com.aspose.words/comparer/), [MailMerger](https://reference.aspose.com/words/java/com.aspose.words/mailmerger/), [Replacer](https://reference.aspose.com/words/java/com.aspose.words/replacer/), [Splitter](https://reference.aspose.com/words/java/com.aspose.words/splitter/) ecc. è stato introdotto, offrendo una serie di metodi che colpiscono il perfetto equilibrio tra semplicità e flessibilità per l'elaborazione dei documenti.

### Rendering e stampa

#### Graduazioni su grafici radiali <sup>24.9</sup>

È stato implementato il rendering delle graduazioni su grafici radiali.

#### CommandButton ActiveX Controlli <sup>24.10</sup>

La possibilità di creare controlli CommandButton ActiveX è stata introdotta aggiungendo un nuovo metodo pubblico [InsertForms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertForms2OleControl-com.aspose.words.Forms2OleControl) e una nuova classe pubblica [Forms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/).

#### Visibilità della forma di controllo <sup>24.10</sup>

È stata aggiunta una nuova proprietà pubblica [Hidden](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#getHidden) per controllare la visibilità delle forme.

#### Variazioni nei grafici Pie e Doughnut <sup>24.10</sup>

Diverse nuove proprietà pubbliche sono state aggiunte ai grafici format Pie e Doughnut.

#### Controllare il rendering dei bordi del campo del modulo di scelta PDF <sup>24.11</sup>

Una nuova opzione per controllare il rendering dei bordi del campo del modulo di scelta PDF è stata implementata aggiungendo una nuova opzione pubblica [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getRenderChoiceFormFieldBorder).

#### Ottenere e impostare i codici di formato per i dati del grafico <sup>24.11</sup>

La possibilità di ottenere e impostare i codici di formato per i dati del grafico è stata aggiunta implementando la proprietà [FormatCode](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/#getFormatCode) nelle classi [ChartXValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartyvaluecollection/) e [BubbleSizeCollection](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/).

#### Rendering di grafici istografici con contenitori ed etichette <sup>24.11</sup>

Il rendering del grafico istogramma è stato migliorato consentendo un numero specificato di contenitori ed etichette.

### Conversione, caricamento e salvataggio di documenti

#### Formattazione sottolineata durante il caricamento dei file Markdown <sup>24.9</sup>

L'opzione per riconoscere la formattazione sottolineata durante il caricamento dei documenti Markdown è stata incorporata aggiungendo una nuova proprietà pubblica [ImportUnderlineFormatting](https://reference.aspose.com/words/java/com.aspose.words/markdownloadoptions/#getImportUnderlineFormatting).

#### Esportazione di tabelle come HTMLquando si salva in Markdown <sup>24.10</sup>

Un'opzione per esportare tabelle come HTML quando si salvano documenti in formato Markdown è stata implementata aggiungendo una nuova proprietà pubblica [ExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getExportAsHtml) e un'enumerazione [MarkdownExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownexportashtml/).

#### Esporta PDF con struttura logica aggiornata <sup>24.11</sup>

L'esportazione PDF è stata migliorata includendo le proprietà del titolo della tabella come titoli degli elementi della struttura logica PDF.

### Mail Merge e rapporti

#### Rimuovere le tabelle vuote durante Mail Merge <sup>24.12</sup>

Una nuova opzione **RemoveEmptyTables** è stata aggiunta all'enumerazione [MailMergeCleanupOptions](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/) per perfezionare l'output Mail Merge.

### Firme digitali

#### Firma documenti con XAdES-EPES <sup>24.9</sup>

La possibilità di firmare documenti con firme di livello XAdES-EPES XML-DSig è stata introdotta aggiungendo una nuova proprietà pubblica [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/signoptions/#getXmlDsigLevel) e una nuova enumerazione pubblica [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/xmldsiglevel/)

### Altri

* Un nuovo metodo pubblico [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-com.aspose.words.Shape...) è stato aggiunto a group shapes. <sup>24.9</sup>
* Un nuovo metodo pubblico [InsertStructuredDocumentTag](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertStructuredDocumentTag-int) è stato aggiunto per inserire **StructuredDocumentTags** in un documento. <sup>24.9</sup>
* L'accesso pubblico ai separatori di note a piè di pagina/note di chiusura è stato fornito aggiungendo alcune classi e proprietà pubbliche. <sup>24.9</sup>
* La possibilità di raggruppare singole forme, group shapes insieme, e raggruppare direttamente entrambe le forme e group shapes è stata introdotta aggiungendo il metodo [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-double-double-double-double-com.aspose.words.ShapeBase...). <sup>24.10</sup>
* La gestione della codifica Big5 per le tabelle cmap TrueType è stata migliorata. <sup>24.10</sup>
* Il supporto per i font taiwanesi obsoleti è stato migliorato. <sup>24.10</sup>
* Per accedere alle proprietà estese del documento, alla classe [BuiltInDocumentProperties](https://reference.aspose.com/words/java/com.aspose.words/builtindocumentproperties/) sono state aggiunte proprietà di sola lettura. <sup>24.11</sup>
* L'impostazione delle didascalie per i controlli ActiveX è stata abilitata aggiungendo un nuovo setter pubblico alla proprietà [Forms2OleControl.Caption](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/#getCaption). <sup>24.11</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Java 24.9 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-9-release-notes/).

Scopri di più su [Aspose.Wordsper Java 24.10 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-10-release-notes/).

Scopri di più su [Aspose.Wordsper Java 24.11 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-11-release-notes/).

Scopri di più su [Aspose.Wordsper Java 24.12 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-12-release-notes/).

{{% /alert %}}

## Aspose.Wordsper Java 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 espande le opzioni per gli assembly, migliora le capacità di rendering ed espande alcune altre opzioni.

Aspose.Words 24.6 migliora le opzioni di rendering, migliora la funzionalità di ricerca e confronto e amplia diverse altre funzionalità.

Aspose.Words 24.7 modifica il modo in cui si lavora con ActiveX, espande le capacità di rendering e esporta nei formati Markdown e XLSX.

Aspose.Words 24.8 migliora la personalizzazione dei grafici con un controllo preciso sulle etichette degli assi, espande la gestione dei font, migliora la gestione della struttura dei documenti e aggiunge nuove funzionalità per l'esportazioneHTML/XAML, la funzionalità PDF, la conversione dei documenti e le firme digitali.

### Formati supportati

A partire dalla versione 24.7, l'esportazione a PDF/UA-2 è supportata per garantire l'accessibilità per gli utenti con disabilità.

### Rendering e stampa

#### Cambiamenti in grafici, forme e DrawingML <sup>24.5</sup>

- È stato implementato il rendering degli effetti DrawingML per la grafica SVG, che estende le funzionalità precedenti limitate alle immagini.
- Il supporto per la creazione di grafici combinati e la regolazione di proprietà come larghezza spazio, sovrapposizione e scala a bolle all'interno dei gruppi di serie è stato introdotto aggiungendo le classi [ChartSeriesGroup](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroup/) e [ChartSeriesGroupCollection](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroupcollection/) e la proprietà [SeriesGroups](https://reference.aspose.com/words/java/com.aspose.words/chart/#getSeriesGroups).
- La funzionalità per manipolare l'effetto SoftEdge delle forme è stata implementata aggiungendo la classe [SoftEdgeFormat](https://reference.aspose.com/words/java/com.aspose.words/softedgeformat/).
- La possibilità di modificare regolare i valori delle forme è stata implementata aggiungendo le classi pubbliche [AdjustmentCollection](https://reference.aspose.com/words/java/com.aspose.words/adjustmentcollection/) e [Adjustment](https://reference.aspose.com/words/java/com.aspose.words/adjustment/) e la proprietà [Adjustments](https://reference.aspose.com/words/java/com.aspose.words/shape/#getAdjustments).

#### Cambiamenti nei grafici, nelle forme e nel disegno <sup>24.6</sup>

- Le capacità di creazione di grafici sono state migliorate. È ora possibile creare una più ampia varietà di grafici, tra cui *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* grafici, *Box & Whisker* grafici, *Waterfalls* e *Funnels*. Ciò consente di visualizzare i dati in modo più diversificato e informativo.
- Il controllo del colore per la formattazione delle ombre è stato migliorato. Puoi ottenere un controllo più preciso sull'aspetto dei tuoi documenti accedendo ai colori delle ombre.
- L'aumento delle prestazioni per il rendering in background è stato migliorato. È possibile velocizzare notevolmente il rendering di sfondi contenenti piccoli elementi grazie alla tecnologia di piastrellatura nativa.
- Sono stati aggiunti gradienti realistici per le forme. Ora è possibile creare forme DML con gradienti non lineari, imitando lo stile visivo di Microsoft Word per un aspetto più lucido.

#### Personalizzazione dell'etichetta dei dati del grafico <sup>24.7</sup>

È stata aggiunta la possibilità di personalizzare le etichette dei dati del grafico come **Orientation** e **Rotation**.

#### Stile numero personalizzato per i livelli di elenco <sup>24.7</sup>

È stato aggiunto un setter per la proprietà pubblica [CustomNumberStyleFormat](https://reference.aspose.com/words/java/com.aspose.words/listlevel/#getCustomNumberStyleFormat). È ora possibile definire uno stile numero personalizzato per i livelli di elenco.

#### Cambiamenti nel lavoro con ActiveX <sup>24.7</sup>

* Le proprietà degli oggetti ActiveX possono ora essere modificate, dandoti un maggiore controllo sul loro comportamento.
* È stata aggiunta la possibilità di modificare il valore del controllo del pulsante di opzione ActiveX per abilitare l'interazione dinamica.
* È stata aggiunta la possibilità di attivare un ActiveX checkbox su "selezionato" o "deselezionato".

#### Controllo sull'asse del grafico Etichette di spunta Orientamento e rotazione <sup>24.8</sup>

È stato aggiunto un controllo preciso sull'orientamento e la rotazione delle etichette di spunta dell'asse del grafico per una più comoda personalizzazione del grafico: la classe [AxisTickLabels](https://reference.aspose.com/words/java/com.aspose.words/axisticklabels/) è stata estesa con le nuove proprietà **Orientation** e **Rotation**.

#### Sostituzione della barra rovesciata con il segno Yen <sup>24.8</sup>

L'esportazione retrocompatibile HTML e XAML per sostituire il carattere di barra rovesciata con il segno di Yen è stata migliorata. Per ottenere ciò, la proprietà **ReplaceBackslashWithYenSign** è stata aggiunta alle classi [HtmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/) e [XamlFlowSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/).

#### Utilizzo dei tag SDT come nomi dei campi modulo durante l'esportazione in PDF <sup>24.8</sup>

L'esportazione PDF con supporto per l'utilizzo di tag SDT come nomi di campi del modulo è stata migliorata aggiungendo una nuova proprietà **UseSdtTagAsFormFieldName** alla classe [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/).

### Conversione, caricamento e salvataggio di documenti

#### Esportazione di collegamenti in formato Markdown <sup>24.7</sup>

La possibilità di controllare l'esportazione dei collegamenti in formato Markdown è stata aggiunta attraverso l'implementazione della proprietà [LinkExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getLinkExportMode).

#### LowCode 24.8 <sup>24.8</sup>

È stata introdotta una nuova classe **LowCode.Converter**, progettata per fornire un insieme di metodi per convertire vari tipi di documenti con una singola riga di codice.

### Cerca e confronta

#### Opzioni di confronto avanzate <sup>24.6</sup>

È stata aggiunta la possibilità di semplificare i flussi di lavoro di analisi dei dati con funzionalità di confronto migliorate. Ciò include una nuova opzione [IgnoreStoreItemId](https://reference.aspose.com/words/java/com.aspose.words/advancedcompareoptions/#getIgnoreStoreItemId) e un'interfaccia ridisegnata per confronti avanzati.

### Altri

* La funzione per eliminare le pagine vuote da un documento è stata implementata aggiungendo il metodo [RemoveBlankPages](https://reference.aspose.com/words/java/com.aspose.words/document/#removeBlankPages). <sup>24.5</sup>
* La possibilità di verificare la presenza di macro VBA senza caricare un documento è stata fornita aggiungendo la proprietà [HasMacros](https://reference.aspose.com/words/java/com.aspose.words/fileformatinfo/#hasMacros). <sup>24.5</sup>
* Mantenere la numerazione delle origini durante l'inserimento di un documento utilizzando il motore di reporting LINQ è ora supportato. <sup>24.5</sup>
* È stata aggiunta una nuova proprietà [DateTimeUtc](https://reference.aspose.com/words/java/com.aspose.words/comment/#getDateTimeUtc), che fornisce un timestamp più preciso per i commenti, migliorando l'organizzazione e la tracciabilità. <sup>24.6</sup>
* Il motore di reporting LINQ è stato migliorato. La rimozione selettiva di paragrafi vuoti e la definizione di messaggi personalizzati per i membri di oggetti mancanti sono stati fatti, portando a rapporti più puliti e più informativi. <sup>24.6</sup>
* Il formato datetime viene ora rilevato automaticamente per l'esportazione senza interruzioni nel formato XLSX. <sup>24.7</sup>
* È stata aggiunta la proprietà pubblica [IsProtected](https://reference.aspose.com/words/java/com.aspose.words/vbaproject/#isProtected), che consente di verificare se un progetto VBA è protetto. <sup>24.7</sup>
* Le informazioni sui font sono state espanse con la proprietà **EmbeddingLicensingRights** aggiunta alle classi [FontInfo](https://reference.aspose.com/words/java/com.aspose.words/fontinfo/) e [PhysicalFontInfo](https://reference.aspose.com/words/java/com.aspose.words/physicalfontinfo/). <sup>24.8</sup>
* È stato aggiunto un modo per cancellare in modo efficiente intestazioni di sezione e piè di pagina preservando le filigrane per lavorare in modo più accurato con la struttura del documento. Per cancellare intestazioni di sezione e piè di pagina, utilizzare il nuovo metodo pubblico **ClearHeadersFooters**. <sup>24.8</sup>
* È stata abilitata la firma digitale dei documenti XPS che utilizzano [XpsSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xpssaveoptions/): a tale scopo è stata aggiunta una nuova proprietà **DigitalSignatureDetails**. <sup>24.8</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Java 24.5 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-5-release-notes/).

Scopri di più su [Aspose.Wordsper Java 24.6 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-6-release-notes/).

Scopri di più su [Aspose.Wordsper Java 24.7 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-7-release-notes/).

Scopri di più su [Aspose.Wordsper Java 24.8 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-8-release-notes/).

{{% /alert %}}

## Aspose.Wordsper Java 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 migliora l'esperienza di gestione dei colori dei tratti, migliora gli oggetti OLE e il reporting LINQ, oltre a introdurre una nuova bibliografia Fonti pubbliche API.

Aspose.Words 24.2 Grafici espansi API, gestione dello stile e opzioni LINQ. Questa versione di Aspose.Words ha anche introdotto la capacità di specificare SvgSaveOptions durante il rendering, il controllo più flessibile che carica i file Markdown e lavora con il testo di riferimento per le note a piè di pagina e le note di chiusura.

Aspose.Words 24.3 introduce un nuovo lettore / scrittore TIFF ed emulazione di operazioni raster binarie per metafile WMF. Aspose.Words 24.3 continua anche ad espandere i Grafici API.

Aspose.Words 24.4 migliora il salvataggio dei formati, alcune opzioni di rendering e migliora il lavoro con le firme digitali.

### Formati supportati <sup>24.4</sup>

Il moderno formato immagine **WebP** è ora supportato in Aspose.Words. Ora è possibile leggere e inserire immagini WebP nei documenti, nonché salvare le immagini in formato WebP.

### Rendering e stampa

#### Controllo del colore del tratto <sup>24.1</sup>

La classe [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) è stata estesa con una serie di nuove proprietà pubbliche relative alla gestione dei colori dei tratti: [ForeThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeThemeColor) e [BackThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackThemeColor), [ForeTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeTintAndShade) e [BackTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackTintAndShade).

#### DrawingML Grafici API Estensione <sup>24.2 / 24.3 / 24.4</sup>

Il **DrawingML Charts API** continua ad essere espanso.

#### Incorpora i font dichiarati nelle regole @font-face <sup>24.4</sup>

Aggiunta la possibilità di incorporare i font dichiarati nelle regole @font-face nelle definizioni dei font del documento risultante è stata introdotta aggiungendo una nuova proprietà [SupportFontFaceRules](https://reference.aspose.com/words/java/com.aspose.words/htmlloadoptions/#getSupportFontFaceRules).

#### Lavorare con la formattazione bagliore e riflessione <sup>24.4</sup>

È stata implementata la possibilità di lavorare con la formattazione di bagliore e riflessione per un oggetto di disegno.

### Caricamento e salvataggio dei documenti

#### Specificare SvgSaveOptions durante il rendering <sup>24.2</sup>

La capacità di specificare [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/) durante il rendering è stata aggiunta usando [ShapeRenderer](https://reference.aspose.com/words/java/com.aspose.words/shaperenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) e [OfficeMathRenderer](https://reference.aspose.com/words/java/com.aspose.words/officemathrenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) metodi.

#### Conserva le righe vuote durante il caricamento dei file Markdown <sup>24.2</sup>

È stata aggiunta la possibilità di conservare le righe vuote durante il caricamento dei file Markdown.

#### Un nuovo TIFF Lettore / scrittore <sup>24.3</sup>

È stato sviluppato un nuovo lettore/scrittore TIFF per Aspose.Words per .NET Standard, .NET 6 e versioni successive. Aspose.Wordsper .NET 24.3 aggiunto il supporto per la lettura di immagini TIFF con tipi di compressione JPEG e vecchi JPEG e anche migliorato significativamente la qualità delle operazioni di lettura e scrittura.

### Altri

* La possibilità di modificare il testo del controllo `TextBox` OLE è stata introdotta aggiungendo una nuova proprietà [Text](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/#getText) alla nuova classe [TextBoxControl](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/). 24.1 <sup>24.1</sup>
* La Bibliografia Fonti pubbliche API è stato implementato con l'aggiunta di alcuni nuovi [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/bibliography/), [Source](https://reference.aspose.com/words/java/com.aspose.words/source/), [ContributorCollection](https://reference.aspose.com/words/java/com.aspose.words/contributorcollection/), [Contributor](https://reference.aspose.com/words/java/com.aspose.words/contributor/), [Corporate](https://reference.aspose.com/words/java/com.aspose.words/corporate/), [PersonCollection](https://reference.aspose.com/words/java/com.aspose.words/personcollection/) e classi [Person](https://reference.aspose.com/words/java/com.aspose.words/person/) e un'enumerazione [SourceType](https://reference.aspose.com/words/java/com.aspose.words/sourcetype/), nonché aggiungendo una nuova proprietà [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/document/#getBibliography) alla classe [Document](https://reference.aspose.com/words/java/com.aspose.words/document/). <sup>24.1</sup>
* È stato fornito un API per limitare l'accesso ai membri di tipo utilizzando la sintassi del modello per il motore di reporting LINQ. <sup>24.1</sup>
* Nuove proprietà pubbliche [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) e [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) per la gestione avanzata dello stile sono state aggiunte alla classe [Style](https://reference.aspose.com/words/net/aspose.words/style/). <sup>24.2</sup>
* La funzionalità per recuperare il testo del marchio di riferimento effettivo per le note a piè di pagina e le note di chiusura è stata migliorata con la proprietà [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) e il metodo [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* La compatibilità con i grafici `Word 2016` per il `LINQ Reporting Engine` è stata abilitata. <sup>24.2</sup>
* È stata implementata l'emulazione di operazioni raster binarie per metafile WMF. <sup>24.3</sup>
* La possibilità di definire le opzioni di firma per i documenti all'interno di **SaveOptions** è stata abilitata aggiungendo una nuova classe [DigitalSignatureDetails](https://reference.aspose.com/words/java/com.aspose.words/digitalsignaturedetails/) con nuovi membri pubblici, nonché aggiungendo nuove proprietà alle classi [OoxmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/docsaveoptions/) e [OdtSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Java 24.1 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-1-release-notes/).

Scopri di più su [Aspose.Wordsper Java 24.2 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-2-release-notes/).

Scopri di più su [Aspose.Wordsper Java 24.3 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-3-release-notes/).

Scopri di più su [Aspose.Wordsper Java 24.4 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-4-release-notes/).

{{% /alert %}}

## Aspose.Wordsper Java 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 espande le opzioni di rendering, l'emulazione di rendering metafile e le opzioni di salvataggio markdown.

Aspose.Words 23.10 migliora il rendering, espande le opzioni per il caricamento e il salvataggio dei documenti e consente agli utenti di unire i documenti in nuovi modi.

Aspose.Words 23.11 migliora il lavoro con le revisioni, il formato XLSX e i caratteri sulla legenda del grafico con opzioni aggiuntive.

Aspose.Words 23.12 introduce nuove proprietà ed enumerazioni per lavorare con i documenti PDF, il supporto per le immagini WebP e la libreria Bouncy Castle aggiornata.

### Rendering e stampa

#### Personalizzazione dei titoli degli assi nei grafici DrawingML <sup>23.9</sup>

La possibilità di personalizzare i titoli degli assi nei grafici DrawingML è stata introdotta dall'implementazione di una nuova proprietà public class [ChartAxisTitle](https://reference.aspose.com/words/java/com.aspose.words/chartaxistitle/) e [Title](https://reference.aspose.com/words/java/com.aspose.words/chartaxis/#getTitle).

#### Determinazione della posizione verticale dei caratteri all'interno di un paragrafo <sup>23.9</sup>

È ora possibile definire la posizione verticale dei font all'interno di un paragrafo utilizzando la nuova proprietà public [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getBaselineAlignment) e la nuova enumerazione [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/baselinealignment/).

#### Controllo del colore di primo piano <sup>23.10</sup>

La possibilità di recuperare il colore di primo piano senza modificatori è stata aggiunta alle classi [Fill](https://reference.aspose.com/words/java/com.aspose.words/fill/) e [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) tramite la proprietà **BaseForeColor**.

#### Espansione della funzionalità dei grafici <sup>23.10</sup>

La funzionalità delle classi [ChartDataPointCollection](https://reference.aspose.com/words/java/com.aspose.words/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/java/com.aspose.words/chartseries/) e [ChartFormat](https://reference.aspose.com/words/java/com.aspose.words/chartformat/) è stata ampliata con nuovi metodi e proprietà.

#### Regola e adatta automaticamente un'immagine in una forma <sup>23.10</sup>

Un modo semplice per regolare e adattare automaticamente un'immagine all'interno di una particolare forma è stato fornito attraverso il nuovo metodo [FitImageToShape](https://reference.aspose.com/words/java/com.aspose.words/imagedata/#fitImageToShape).

#### Formattazione predefinita dei caratteri per le voci della legenda del grafico DrawingML <sup>23.11</sup>

La possibilità di specificare la formattazione predefinita dei caratteri per le voci di legenda dei grafici DrawingML è stata aggiunta tramite la proprietà **Font**. Questa funzione facilita un aspetto più snello e coerente per gli elementi del grafico, migliorando l'estetica complessiva del documento.

#### Specificare il layout di pagina quando si apre PDF in Reader <sup>23.12</sup>

La possibilità di specificare il layout di pagina da utilizzare quando si apre un documento in un lettore PDF è stata aggiunta attraverso l'introduzione di una nuova proprietà [PageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getPageLayout) alla classe [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/) e l'introduzione di una nuova enumerazione [PdfPageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfpagelayout/).

### Caricamento e salvataggio dei documenti

#### Specificare il nome di una cartella per costruire l'immagine URIsin Markdown <sup>23.9</sup>

La classe [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) è stata espansa includendo la proprietà [ImagesFolderAlias](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImagesFolderAlias), che consente di specificare il nome della cartella utilizzata per costruire l'immagine URIs scritta nel documento Markdown.

#### Ridurre PDF Dimensione dell'output <sup>23.10</sup>

Sono state implementate varie ottimizzazioni di rendering PDF per ridurre le dimensioni dell'output quando si utilizzano le impostazioni [OptimizeOutput](https://reference.aspose.com/words/java/com.aspose.words/fixedpagesaveoptions/#getOptimizeOutput).

#### Riconoscere i collegamenti ipertestuali durante il caricamento di documenti TXT <sup>23.10</sup>

La funzione per riconoscere i collegamenti ipertestuali durante il caricamento di documenti TXT è stata implementata aggiungendo una nuova proprietà [DetectHyperlinks](https://reference.aspose.com/words/java/com.aspose.words/txtloadoptions/#getDetectHyperlinks).

### Altri

- È stata implementata l'emulazione del rendering Metafile per determinare la dimensione della rasterizzazione, in particolare per WMF pen width e EMF cosmetic pen width. Per ottenere ciò, la proprietà **ScaleWmfFontsToMetafileSize** è stata sostituita con la proprietà [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPage) e la proprietà [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPageResolution) è stata aggiunta. <sup>23.9</sup>
- Un metodo semplificato per l'inserimento di un documento in un altro documento nella posizione corrente del cursore è stato introdotto utilizzando il metodo [InsertDocumentInline](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertDocumentInline-com.aspose.words.Document-int-com.aspose.words.ImportFormatOptions). <sup>23.10</sup>
- La possibilità di accedere e modificare le proprietà di stile è stata aggiunta attraverso l'introduzione della nuova proprietà [Locked](https://reference.aspose.com/words/java/com.aspose.words/style/#getLocked). <sup>23.10</sup>
- Un parametro di tipo generico è stato aggiunto ai metodi della classe [CompositeNode](https://reference.aspose.com/words/java/com.aspose.words/compositenode/). <sup>23.10</sup>
- Un modo per controllare quando una determinata revisione deve essere accettata / rifiutata o meno è stato implementato utilizzando i metodi [Accept](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#accept-com.aspose.words.IRevisionCriteria) e [Reject](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#reject-com.aspose.words.IRevisionCriteria). Questo miglioramento garantisce agli utenti un controllo più preciso sul processo di revisione. <sup>23.11</sup>
- La possibilità di scrivere tutte le sezioni di un documento sullo stesso foglio di lavoro XLSX è stata fornita tramite il nuovo tipo di enumerazione [XlsxSectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsectionmode/) e la nuova proprietà [SectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/#getSectionMode). <sup>23.11</sup>
- È stato introdotto il supporto per l'immagine WebP. Si prega di notare che questa funzione è disponibile solo per .versioni NetStandart e .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Java 23.9 Note di rilascio](/words/java/aspose-words-for-java-23-9-release-notes/).

Scopri di più su [Aspose.Wordsper Java 23.10 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-10-release-notes/).

Scopri di più su [Aspose.Wordsper Java 23.11 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-11-release-notes/).

Scopri di più su [Aspose.Wordsper Java 23.12 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-12-release-notes/).

{{% /alert %}}

## Aspose.Wordsper Java 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 migliora la capacità di lavorare con i dati delle serie di grafici e la capacità di lavorare con i documenti ODT, oltre a migliorare le intestazioni/piè di pagina e il loro spostamento del testo.

Aspose.Words 23.6 espande le opzioni di rendering, aggiunge un nuovo formato di esportazione, migliora gli strumenti LINQ reporting e LowCode.

Aspose.Words 23.7 migliora le funzionalità di reporting, aggiunge un nuovo formato di esportazione e introduce modifiche all'utilizzo di tabelle e firme digitali.

Aspose.Words 23.8 espande le funzionalità di diversi formati, migliora il rendering e aggiunge nuove opzioni per lavorare con i campi.

### Formati supportati

* A partire dalla versione 23.6, è possibile salvare un documento in formato XLSX. Ora puoi convertire i tuoi documenti in formato Excel. <sup>23.6</sup>

* A partire dalla versione 23.7, è possibile salvare una pagina o una forma del documento in formato EPS. <sup>23.7</sup>

* ### Nuove caratteristiche di formato

  - È stata introdotta la funzionalità per generare automaticamente il Sommario (TOC) per i documenti MOBI. <sup>23.8</sup>
  - Il costruttore [PdfEncryptionDetails](https://reference.aspose.com/words/java/com.aspose.words/pdfencryptiondetails/#PdfEncryptionDetails-java.lang.String-java.lang.String) è stato espanso con [PdfPermissions](https://reference.aspose.com/words/java/com.aspose.words/pdfpermissions/). <sup>23.8</sup>
  - È stata implementata la modellatura del testo verticale per metafile EMF. <sup>23.8</sup>

### Rendering

#### Ottenere e modificare i dati delle serie di grafici <sup>23.5</sup>

La funzione per ottenere e modificare i dati delle serie di grafici è stata fornita aggiungendo:

- nuove classi: [ChartXValue](https://reference.aspose.com/words/java/com.aspose.words/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/java/com.aspose.words/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/java/com.aspose.words/chartmultilevelvalue/)
- nuovi tipi di enum: [ChartXValueType](https://reference.aspose.com/words/java/com.aspose.words/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/java/com.aspose.words/chartyvaluetype/)

#### Supporto per tipografia avanzata <sup>23.6</sup>

È stato aggiunto il supporto per la tipografia avanzata nel rendering WMF, EMF e EMF+.

#### Contenuto colorato sulla pagina <sup>23.6</sup>

La proprietà pubblica [PageInfo.Colored](https://reference.aspose.com/words/java/com.aspose.words/pageinfo/#getColored), che indica se la pagina è colorata o meno, è stata aggiunta.

#### Formattazione per le etichette dei dati del grafico <sup>23.6</sup>

È stata implementata la possibilità di impostare la formattazione di riempimento, traccia e callout per le etichette dei dati del grafico.

### Mail Merge e rapporti

#### Inserimento dinamico HTML per il motore di reportistica LINQ <sup>23.6</sup>

È stato aggiunto un nuovo modo di inserimento dinamico HTML per il motore di reportistica LINQ.

#### Mustache Tag Supporto <sup>23.7</sup>

I tag Mustache sono ora supportati nei metodi [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#getRegionsHierarchy) e [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#getFieldNamesForRegion-java.lang.String).

#### LINQ Aggiornamenti della sintassi del modello del motore di reporting <sup>23.7</sup>

La sintassi del modello del motore di reporting LINQ ora supporta i metodi di estensione `ElementAt` e ElementAtOrDefault.

#### Specificare la dimensione delle immagini renderizzate <sup>23.8</sup>

È stata introdotta una nuova proprietà pubblica **ImageSize** per specificare la dimensione delle immagini renderizzate in pixel.

#### Conserva spazi bianchi per JSON Valori stringa - LINQ <sup>23.8</sup>

È stata aggiunta un'opzione al motore di reporting LINQ per preservare gli spazi bianchi per i valori di stringa JSON.

### LowCode <sup>23.6</sup>

Sono stati aggiunti nuovi metodi LowCode destinati a unire diversi tipi di documenti in un singolo documento di output.

### Altri

- È stato implementato il supporto per il wrapping del testo nelle intestazioni/piè di pagina. <sup>23.5</sup>
- La possibilità di rimuovere le firme digitali dai documenti ODT è stata aggiunta tramite il metodo [RemoveAllSignatures](https://reference.aspose.com/words/java/com.aspose.words/digitalsignatureutil/#removeAllSignatures-java.io.InputStream-java.io.OutputStream). <sup>23.5</sup>
- È stata aggiunta la proprietà pubblica [PhoneticGuide](https://reference.aspose.com/words/java/com.aspose.words/run/#getPhoneticGuide) per ottenere il testo base e ruby della guida fonetica [Run](https://reference.aspose.com/words/java/com.aspose.words/run/). <sup>23.5</sup>
- La possibilità di recuperare un valore di firma digitale da un documento con firma digitale come matrice di byte è stata aggiunta introducendo una nuova proprietà [SignatureValue](https://reference.aspose.com/words/java/com.aspose.words/digitalsignature/#getSignatureValue). <sup>23.7</sup>
- Le classi [Row](https://reference.aspose.com/words/java/com.aspose.words/row/) e [Cell](https://reference.aspose.com/words/java/com.aspose.words/cell/) sono state ampliate con nuovi membri pubblici– [Row.NextRow](https://reference.aspose.com/words/java/com.aspose.words/row/#getNextRow), [Row.PreviousRow](https://reference.aspose.com/words/java/com.aspose.words/row/#getPreviousRow), [Cell.NextCell](https://reference.aspose.com/words/java/com.aspose.words/cell/#getNextCell), e [Cell.PreviousCell](https://reference.aspose.com/words/java/com.aspose.words/cell/#getPreviousCell). <sup>23.7</sup>
- È stato aggiunto il supporto per i campi CITATION e BIBLIOGRAPHY. <sup>23.8</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Java 23.5 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-5-release-notes/).

Scopri di più su [Aspose.Wordsper Java 23.6 Note di rilascio](/words/java/aspose-words-for-java-23-6-release-notes/).

Scopri di più su [Aspose.Wordsper Java 23.7 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-7-release-notes/).

Scopri di più su [Aspose.Wordsper Java 23.8 Note di rilascio](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-8-release-notes/).

{{% /alert %}}

## Vedi anche

{{% alert color="primary" %}}

Questa pagina contiene le ultime notizie di rilascio degli ultimi 2 anni. Per i dettagli sulle versioni precedenti, vedere [Note di rilascio'](https://releases.aspose.com/words/java/release-notes/) pagine nelle relative sezioni.

{{% /alert %}}
