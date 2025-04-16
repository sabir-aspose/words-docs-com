---
title: Cosa c'è di nuovo
second_title: Aspose.Words per Python via .NET
articleTitle: Cosa c'è di nuovo in Aspose.Words per Python via .NET
linktitle: Cosa c'è di nuovo in Aspose.Words per Python via .NET
type: docs
description: "Aspose.Words per Python via .NET si espande e migliora ogni giorno. In questa pagina, puoi conoscere le caratteristiche enormi e più interessanti del prodotto."
weight: 10
url: /it/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-02-17-18-02-05
---

Questa pagina descrive le nuove funzionalità Aspose.Words più interessanti introdotte nelle ultime versioni.

## Aspose.Wordsper Python via .NET 25.1, 25.2

Aspose.Words 25.1 introduce il controllo grammaticale basato su AI e migliora il salvataggio dei documenti con opzioni avanzate per i formati HTML, SVG e Markdown.

Aspose.Words 25.2 introduce la sintesi del testo con i modelli Anthropic AI, aggiunge il supporto al formato MsWorks, migliora il controllo tipografico e migliora la struttura PDF e la gestione degli elenchi.

### AI-Funzioni alimentate

#### Controllo grammaticale del documento AI <sup>25.1</sup>

La possibilità di controllare la grammatica del documento fornito utilizzando i modelli generativi OpenAI è stata introdotta aggiungendo un nuovo metodo [check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/).

#### Riassunto utilizzando modelli linguistici antropici generativi <sup>25.2</sup>

La sintesi del testo utilizzando modelli di linguaggio antropico generativo è stata abilitata introducendo una nuova classe pubblica [AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/).

### Formati supportati <sup>25.2</sup>

A partire dalla versione 25.2, è stata aggiunta la compatibilità con il nuovo formato di caricamento MsWorks per i documenti Works Microsoft.

### Conversione, caricamento e salvataggio di documenti

#### Migliorato il salvataggio nei formati HTML e SVG <sup>25.1</sup>

Il salvataggio nei formati HTML e SVG è stato migliorato aggiungendo le proprietà **id_prefix** e **remove_java_script_from_links** a entrambe le classi [HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/) e [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/).

#### Impostare la risoluzione dell'immagine e la modalità di uscita OfficeMath Quando si salva su Markdown <sup>25.1</sup>

* Una nuova opzione [image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/) è stata aggiunta alla classe [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) per impostare la risoluzione dell'immagine.
* Una nuova opzione [office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/) e l'enumerazione [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/) sono state aggiunte alla classe [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) per impostare la modalità di output OfficeMath.

### Rendering

#### Controllo tipografico migliorato <sup>25.2</sup>

La proprietà [number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/) è stata aggiunta per migliorare il controllo tipografico.

### Altri

* La struttura logica di PDF è stata migliorata con il supporto per i campi TOA, BIBLIOGRAPHY e INDEX. <sup>25.2</sup>
* Il metodo [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate) è stato introdotto per una migliore gestione delle liste. <sup>25.2</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Python via .NET 25.1 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 25.2 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

{{% /alert %}}

## Aspose.Words per Python tramite .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduce l'inserimento group shape e l'inserimento StructuredDocumentTag tramite DocumentBuilder, migliora il rendering dei grafici radiali con graduazioni, migliora le firme digitali con il supporto XAdES-EPES, aggiunge il riconoscimento della sottolineatura Markdown e fornisce l'accesso ai separatori di note a piè di pagina/note di chiusura.

Aspose.Words 24.10 introduce il supporto avanzato del controllo ActiveX con la creazione di CommandButton, il nuovo controllo della visibilità delle forme, la possibilità di esportare group shapes, una migliore esportazione Markdown per le tabelle, la formattazione dei grafici per i grafici Pie e Doughnut, una migliore gestione della codifica Big5 e il supporto per i font taiwanesi obsoleti.

Aspose.Words 24.11 introduce il riepilogo del documento basato su AI, opzioni di rendering avanzate, accesso migliorato alle proprietà del documento e sottotitoli del controllo ActiveX.

Aspose.Words 24.12 introduce il posizionamento personalizzabile delle etichette dei dati, la traduzione del testo basata su Google AI e nuove classi di elaborazione LowCode migliorate.

### AI-Funzioni alimentate

#### Riepilogo dei documenti utilizzando OpenAI e Google <sup>24.11</sup>

Il supporto per il riepilogo dei documenti utilizzando i modelli di linguaggio generativo **OpenAI** e **Google** è stato integrato aggiungendo lo spazio dei nomi [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) con i suoi membri pubblici.

#### Traduzione del testo utilizzando i modelli linguistici generativi di Google <sup>24.12</sup>

La capacità di tradurre il testo utilizzando i modelli linguistici generativi di Google è stata implementata in Aspose.Words aggiungendo il metodo [translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/) e l'enumerazione [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) allo spazio dei nomi [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Nuove classi LowCode come [Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) ecc. è stato introdotto, offrendo una serie di metodi che colpiscono il perfetto equilibrio tra semplicità e flessibilità per l'elaborazione dei documenti.

### Rendering e stampa

#### Graduazioni su grafici radiali <sup>24.9</sup>

È stato implementato il rendering delle graduazioni su grafici radiali.

#### CommandButton Controlli ActiveX <sup>24.10</sup>

La possibilità di creare controlli ActiveX CommandButton è stata introdotta aggiungendo un nuovo metodo pubblico [insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/) e una nuova classe pubblica [Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/).

#### Visibilità della forma di controllo <sup>24.10</sup>

È stata aggiunta una nuova proprietà pubblica [hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/) per controllare la visibilità delle forme.

#### Variazioni nei grafici Pie e Doughnut <sup>24.10</sup>

Diverse nuove proprietà pubbliche sono state aggiunte ai grafici format Pie e Doughnut.

#### Controllare il rendering dei bordi del campo del modulo di scelta PDF <sup>24.11</sup>

Una nuova opzione per controllare il rendering dei bordi del campo del modulo di scelta PDF è stata implementata aggiungendo una nuova opzione pubblica [render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/).

#### Ottenere e impostare i codici di formato per i dati del grafico <sup>24.11</sup>

La possibilità di ottenere e impostare i codici di formato per i dati del grafico è stata aggiunta implementando la proprietà [format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/) nelle classi [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/) e [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/).

#### Rendering di grafici istografici con contenitori ed etichette <sup>24.11</sup>

Il rendering del grafico istogramma è stato migliorato consentendo un numero specificato di contenitori ed etichette.

#### Personalizzare il posizionamento delle etichette dei dati <sup>24.12</sup>

La possibilità di personalizzare il posizionamento delle etichette dati è stata aggiunta introducendo nuove proprietà nelle classi th [ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/) e [ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Conversione, caricamento e salvataggio di documenti

#### Formattazione sottolineata durante il caricamento dei file Markdown <sup>24.9</sup>

L'opzione per riconoscere la formattazione sottolineata durante il caricamento dei documenti Markdown è stata incorporata aggiungendo una nuova proprietà pubblica [import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/).

#### Esportazione di tabelle come HTMLquando si salva in Markdown <sup>24.10</sup>

Un'opzione per esportare tabelle come HTML quando si salvano documenti in formato Markdown è stata implementata aggiungendo una nuova proprietà pubblica [export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/) e un'enumerazione [MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/).

#### Esporta PDF con struttura logica aggiornata <sup>24.11</sup>

L'esportazione PDF è stata migliorata includendo le proprietà del titolo della tabella come titoli degli elementi della struttura logica PDF.

### Firme digitali

#### Firma documenti con XAdES-EPES <sup>24.9</sup>

La possibilità di firmare documenti con firme di livello XAdES-EPES XML-DSig è stata introdotta aggiungendo una nuova proprietà pubblica [xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/) e una nuova enumerazione pubblica [XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/).

### Altri

* Un nuovo metodo pubblico [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/) è stato aggiunto a group shapes. <sup>24.9</sup>
* Un nuovo metodo pubblico [insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/) è stato aggiunto per inserire **StructuredDocumentTags** in un documento. <sup>24.9</sup>
* L'accesso pubblico ai separatori di note a piè di pagina/note di chiusura è stato fornito aggiungendo alcune classi e proprietà pubbliche. <sup>24.9</sup>
* La possibilità di raggruppare singole forme, group shapes insieme, e raggruppare direttamente entrambe le forme e group shapes è stata introdotta aggiungendo il metodo [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist). <sup>24.10</sup>
* La gestione della codifica Big5 per le tabelle cmap TrueType è stata migliorata. <sup>24.10</sup>
* Il supporto per i font taiwanesi obsoleti è stato migliorato. <sup>24.10</sup>
* Per accedere alle proprietà estese del documento, alla classe [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/) sono state aggiunte proprietà di sola lettura. <sup>24.11</sup>
* L'impostazione dei sottotitoli per i controlli ActiveX è stata abilitata aggiungendo un nuovo setter pubblico alla proprietà [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Python via .NET 24.9 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 24.10 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 24.11 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 24.12 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words per Python tramite .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 espande le opzioni per gli assembly, migliora le capacità di rendering ed espande alcune altre opzioni.

Aspose.Words 24.6 migliora le opzioni di rendering, migliora la funzionalità di ricerca e confronto e amplia diverse altre funzionalità.

Aspose.Words 24.7 modifica il modo in cui si lavora con ActiveX, espande le capacità di rendering e esporta nei formati Markdown e XLSX.

Aspose.Words 24.8 migliora la personalizzazione dei grafici con un controllo preciso sulle etichette degli assi, espande la gestione dei font, migliora la gestione della struttura dei documenti e aggiunge nuove funzionalità per l'esportazioneHTML/XAML, la funzionalità PDF, la conversione dei documenti e le firme digitali.

### Formati supportati

A partire dalla versione 24.7, l'esportazione a PDF/UA-2 è supportata per garantire l'accessibilità per gli utenti con disabilità.

### Rendering e stampa

#### Cambiamenti in grafici, forme e DrawingML <sup>24.5</sup>

* È stato implementato il rendering degli effetti DrawingML per la grafica SVG, che estende le funzionalità precedenti limitate alle immagini.
* Il supporto per la creazione di grafici combinati e la regolazione di proprietà come larghezza spazio, sovrapposizione e scala a bolle all'interno dei gruppi di serie è stato introdotto aggiungendo le classi [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/) e [ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/) e la proprietà [series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/).
* La funzionalità per manipolare l'effetto SoftEdge delle forme è stata implementata aggiungendo la classe [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/).
* La possibilità di modificare regolare i valori delle forme è stata implementata aggiungendo le classi pubbliche **AdjustmentCollection** e **Adjustment** e la proprietà [adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/).

#### Cambiamenti nei grafici, nelle forme e nel disegno <sup>24.6</sup>

- Le capacità di creazione di grafici sono state migliorate. È ora possibile creare una più ampia varietà di grafici, tra cui *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* grafici, *Box & Whisker* grafici, *Waterfalls* e *Funnels*. Ciò consente di visualizzare i dati in modo più diversificato e informativo.
- Il controllo del colore per la formattazione delle ombre è stato migliorato. Puoi ottenere un controllo più preciso sull'aspetto dei tuoi documenti accedendo ai colori delle ombre.
- L'aumento delle prestazioni per il rendering in background è stato migliorato. È possibile velocizzare notevolmente il rendering di sfondi contenenti piccoli elementi grazie alla tecnologia di piastrellatura nativa.
- Sono stati aggiunti gradienti realistici per le forme. Ora è possibile creare forme DML con gradienti non lineari, imitando lo stile visivo di Microsoft Word per un aspetto più lucido.

#### Personalizzazione dell'etichetta dei dati del grafico <sup>24.7</sup>

È stata aggiunta la possibilità di personalizzare le etichette dei dati del grafico come **Orientation** e **Rotation**.

#### Stile numero personalizzato per i livelli di elenco <sup>24.7</sup>

È stato aggiunto un setter per la proprietà pubblica [custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/). È ora possibile definire uno stile numero personalizzato per i livelli di elenco.

#### Cambiamenti nel lavoro con ActiveX <sup>24.7</sup>

- Le proprietà degli oggetti ActiveX possono ora essere modificate, offrendo un maggiore controllo sul loro comportamento.
- È stata aggiunta la possibilità di modificare il valore del controllo ActiveX del pulsante di opzione per abilitare l'interazione dinamica.
- È stata aggiunta la possibilità di attivare un ActiveX checkbox su "controllato" o "deselezionato".

#### Controllo sull'asse del grafico Etichette di spunta Orientamento e rotazione <sup>24.8</sup>

È stato aggiunto un controllo preciso sull'orientamento e la rotazione delle etichette di spunta dell'asse del grafico per una più comoda personalizzazione del grafico: la classe [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) è stata estesa con le nuove proprietà [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) e [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/).

#### Sostituzione della barra rovesciata con il segno Yen <sup>24.8</sup>

L'esportazione retrocompatibile HTML e XAML per sostituire il carattere di barra rovesciata con il segno di Yen è stata migliorata. Per ottenere ciò, la proprietà **replace_backslash_with_yen_sign** è stata aggiunta alle classi [HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/) e [XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/).

#### Utilizzo dei tag SDT come nomi dei campi modulo durante l'esportazione in PDF <sup>24.8</sup>

L'esportazione PDF con supporto per l'utilizzo di tag SDT come nomi di campi del modulo è stata migliorata aggiungendo una nuova proprietà [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) alla classe [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/).

### Conversione, caricamento e salvataggio di documenti

#### Esportazione di collegamenti in formato Markdown <sup>24.7</sup>

La possibilità di controllare l'esportazione dei collegamenti in formato Markdown è stata aggiunta attraverso l'implementazione della proprietà [link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/).

#### LowCode 24.8 <sup>24.8</sup>

È stata introdotta una nuova classe [LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/), progettata per fornire un insieme di metodi per convertire vari tipi di documenti con una singola riga di codice.

### Cerca e confronta

#### Opzioni di confronto avanzate <sup>24.6</sup>

È stata aggiunta la possibilità di semplificare i flussi di lavoro di analisi dei dati con funzionalità di confronto migliorate. Ciò include una nuova opzione [ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/) e un'interfaccia ridisegnata per confronti avanzati.

### Altri

* La funzione per eliminare le pagine vuote da un documento è stata implementata aggiungendo il metodo [remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/). <sup>24.5</sup>
* La possibilità di verificare la presenza di macro VBA senza caricare un documento è stata fornita aggiungendo la proprietà [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/). <sup>24.5</sup>
* Mantenere la numerazione delle origini durante l'inserimento di un documento utilizzando il motore di reporting LINQ è ora supportato. <sup>24.5</sup>
* È stata aggiunta una nuova proprietà [date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/), che fornisce un timestamp più preciso per i commenti, migliorando l'organizzazione e la tracciabilità. <sup>24.6</sup>
* Il formato datetime viene ora rilevato automaticamente per l'esportazione senza interruzioni nel formato XLSX. <sup>24.7</sup>
* È stata aggiunta la proprietà pubblica [is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/), che consente di verificare se un progetto VBA è protetto. <sup>24.7</sup>
* Le informazioni sui font sono state espanse con la proprietà **embedding_licensing_rights** aggiunta alle classi [FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/) e [PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* È stato aggiunto un modo per cancellare in modo efficiente intestazioni di sezione e piè di pagina preservando le filigrane per lavorare in modo più accurato con la struttura del documento. Per cancellare intestazioni di sezione e piè di pagina, utilizzare il nuovo metodo pubblico [clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default). <sup>24.8</sup>
* È stata abilitata la firma digitale dei documenti XPS che utilizzano [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/): a tale scopo è stata aggiunta una nuova proprietà [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/). <sup>24.8</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Python via .NET 24.5 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 24.6 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 24.7 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 24.8 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words per Python tramite .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 migliora l'esperienza di gestione dei colori dei tratti, migliora gli oggetti OLE e introduce un nuovo pubblico `Bibliography Sources` API.

Aspose.Words 24.2 Grafici espansi API e gestione dello stile. Questa versione di Aspose.Words ha anche introdotto la capacità di specificare SvgSaveOptions durante il rendering, il controllo più flessibile che carica i file Markdown e lavora con il testo di riferimento per le note a piè di pagina e le note di chiusura.

Aspose.Words 24.3 introduce un nuovo lettore / scrittore TIFF ed emulazione di operazioni raster binarie per metafile WMF. Aspose.Words 24.3 continua anche ad espandere i Grafici API.

Aspose.Words 24.4 migliora il salvataggio dei formati, alcune opzioni di rendering e migliora il lavoro con le firme digitali.

### Formati supportati <sup>24.4</sup>

Il moderno formato immagine **WebP** è ora supportato in Aspose.Words per .NET Framework 4.6.2 e più in alto. Ora è possibile leggere e inserire immagini WebP nei documenti, nonché salvare le immagini in formato WebP.

Si noti che WebP è attualmente disponibile solo in .NET Standard e .NET Framework v4.6.2 e versioni successive.

### Rendering e stampa

#### Controllo del colore del tratto <sup>24.1</sup>

La classe [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) è stata estesa con una serie di nuove proprietà pubbliche relative alla gestione dei colori dei tratti: [fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/) e [back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/), [fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/) e [back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### DrawingML Grafici API Estensione <sup>24.2 / 24.3 / 24.4</sup>

Il **DrawingML Charts API** continua ad essere espanso.

#### Incorpora i font dichiarati nelle regole @font-face <sup>24.4</sup>

Aggiunta la possibilità di incorporare i font dichiarati nelle regole @font-face nelle definizioni dei font del documento risultante è stata introdotta aggiungendo una nuova proprietà [support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/).

#### Lavorare con la formattazione bagliore e riflessione <sup>24.4</sup>

È stata implementata la possibilità di lavorare con la formattazione di bagliore e riflessione per un oggetto di disegno.

### Caricamento e salvataggio dei documenti

#### Specificare SvgSaveOptions durante il rendering <sup>24.2</sup>

La capacità di specificare [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) durante il rendering è stata aggiunta usando [ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) e [OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) metodi.

#### Conserva le righe vuote durante il caricamento dei file Markdown <sup>24.2</sup>

È stata aggiunta la possibilità di conservare le righe vuote durante il caricamento dei file Markdown.

#### Un nuovo TIFF Lettore / scrittore <sup>24.3</sup>

È stato sviluppato un nuovo lettore/scrittore TIFF per Aspose.Words. Aspose.Wordsper .NET 24.3 aggiunto il supporto per la lettura di immagini TIFF con tipi di compressione JPEG e vecchi JPEG e anche migliorato significativamente la qualità delle operazioni di lettura e scrittura.

### Altri

* La possibilità di modificare il testo del controllo `TextBox` OLE è stata introdotta aggiungendo una nuova proprietà **Text** alla nuova classe **TextBoxControl**. <sup>24.1</sup>
* La Bibliography Sources public API è stata implementata attraverso l'aggiunta di un nuovo namespace [Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/) con le sue nuove classi ed enumerazioni, e attraverso l'aggiunta di una nuova proprietà [bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/) alla classe [Document](https://reference.aspose.com/words/python-net/aspose.words/document/). <sup>24.1</sup>
* Nuove proprietà pubbliche [priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/), [unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/) e [semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/) per la gestione avanzata dello stile sono state aggiunte alla classe [Style](https://reference.aspose.com/words/python-net/aspose.words/style/). <sup>24.2</sup>
* La funzionalità per recuperare il testo del marchio di riferimento effettivo per le note a piè di pagina e le note di chiusura è stata migliorata con la proprietà [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/) e il metodo [update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default). <sup>24.2</sup>
* È stata implementata l'emulazione di operazioni raster binarie per metafile WMF. <sup>24.3</sup>
* La possibilità di definire le opzioni di firma per i documenti all'interno di **SaveOptions** è stata abilitata aggiungendo una nuova classe [DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/) con nuovi membri pubblici, nonché aggiungendo nuove proprietà alle classi [OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/) e [OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Python via .NET 24.1 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 24.2 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 24.3 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 24.4 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words per Python tramite .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 espande le opzioni di rendering, l'emulazione di rendering metafile e le opzioni di salvataggio markdown.

Aspose.Words 23.10 migliora il rendering, espande le opzioni per il caricamento e il salvataggio dei documenti e consente agli utenti di unire i documenti in nuovi modi.

Aspose.Words 23.11 migliora il lavoro con le revisioni, il formato XLSX e i caratteri sulla legenda del grafico con opzioni aggiuntive.

Aspose.Words 23.12 introduce nuove proprietà ed enumerazioni per lavorare con i documenti PDF e OOXML, nonché il supporto per le immagini WebP.

### Rendering e stampa

#### Personalizzazione dei titoli degli assi nei grafici DrawingML <sup>23.9</sup>

La possibilità di personalizzare i titoli degli assi nei grafici DrawingML è stata introdotta dall'implementazione di una nuova proprietà public class [ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/) e [title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/).

####  Determinazione della posizione verticale dei caratteri all'interno di un paragrafo <sup>23.9</sup>

È ora possibile definire la posizione verticale dei font all'interno di un paragrafo utilizzando la nuova proprietà public [baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/) e la nuova enumerazione [BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/).

#### Controllo del colore di primo piano <sup>23.10</sup>

La possibilità di recuperare il colore di primo piano senza modificatori è stata aggiunta alle classi [Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/) e [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) tramite la proprietà **BaseForeColor**.

#### Espansione della funzionalità dei grafici <sup>23.10</sup>

La funzionalità delle classi [ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/) e [ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/) è stata ampliata con nuovi metodi e proprietà.

#### Regola e adatta automaticamente un'immagine in una forma <sup>23.10</sup>

Un modo semplice per regolare e adattare automaticamente un'immagine all'interno di una particolare forma è stato fornito attraverso il nuovo metodo [fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default).

#### Formattazione predefinita dei caratteri per le voci della legenda del grafico DrawingML <sup>23.11</sup>

La possibilità di specificare la formattazione predefinita dei caratteri per le voci di legenda dei grafici DrawingML è stata aggiunta tramite la proprietà [font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/). Questa funzione facilita un aspetto più snello e coerente per gli elementi del grafico, migliorando l'estetica complessiva del documento.

#### Specificare il layout di pagina quando si apre PDF in Reader <sup>23.12</sup>

La possibilità di specificare il layout di pagina da utilizzare quando si apre un documento in un lettore PDF è stata aggiunta attraverso l'introduzione di una nuova proprietà [page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/) alla classe [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) e l'introduzione di una nuova enumerazione [PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/).

### Caricamento e salvataggio dei documenti

#### Specificare il nome di una cartella per costruire l'immagine URIsin Markdown <sup>23.9</sup>

La classe [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) è stata espansa includendo la proprietà [images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/), che consente di specificare il nome della cartella utilizzata per costruire l'immagine URIs scritta nel documento Markdown.

#### Ridurre PDF Dimensione dell'output <sup>23.10</sup>

Sono state implementate varie ottimizzazioni di rendering PDF per ridurre le dimensioni dell'output quando si utilizzano le impostazioni [optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/).

#### Riconoscere i collegamenti ipertestuali durante il caricamento di documenti TXT <sup>23.10</sup>

La funzione per riconoscere i collegamenti ipertestuali durante il caricamento di documenti TXT è stata implementata aggiungendo una nuova proprietà [detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/).

### Altri

- È stata implementata l'emulazione del rendering Metafile per determinare la dimensione della rasterizzazione, in particolare per WMF pen width e EMF cosmetic pen width. Per ottenere ciò, la proprietà **ScaleWmfFontsToMetafileSize** è stata sostituita con la proprietà [emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/) e la proprietà [emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/) è stata aggiunta. <sup>23.9</sup>
- Un metodo semplificato per l'inserimento di un documento in un altro documento nella posizione corrente del cursore è stato introdotto utilizzando il metodo [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions). <sup>23.10</sup>
- La possibilità di accedere e modificare le proprietà di stile è stata aggiunta attraverso l'introduzione della nuova proprietà [locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/). <sup>23.10</sup>
- Un parametro di tipo generico è stato aggiunto ai metodi della classe [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/). <sup>23.10</sup>
- La possibilità di scrivere tutte le sezioni di un documento sullo stesso foglio di lavoro XLSX è stata fornita tramite il nuovo tipo di enumerazione [XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/) e la nuova proprietà [section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/). <sup>23.11</sup>
* Un modo per controllare come verranno utilizzate le estensioni di formato ZIP64 per i documenti OOXML è stato implementato tramite la nuova proprietà Zip64Mode della classe `OoxmlSaveOptions` e la nuova enumerazione Zip64Mode. <sup>23.12</sup>
* È stato introdotto il supporto per l'immagine WebP. Si prega di notare che questa funzione è disponibile solo per .versioni NetStandart e .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Python via .NET 23.9 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 23.10 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 23.11 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

Scopri di più su [Aspose.Wordsper .NET 23.12 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words per Python tramite .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 migliora la capacità di lavorare con i dati delle serie di grafici e la capacità di lavorare con i documenti ODT, oltre a migliorare le intestazioni/piè di pagina e il loro spostamento del testo.

Aspose.Words 23.6 espande le opzioni di rendering, aggiunge un nuovo formato di esportazione, migliora gli strumenti LINQ reporting e LowCode.

Aspose.Words 23.7 migliora le funzionalità di reporting, aggiunge un nuovo formato di esportazione e introduce modifiche all'utilizzo di tabelle e firme digitali.

Aspose.Words 23.8 espande le funzionalità di diversi formati, migliora il rendering e aggiunge nuove opzioni per lavorare con i campi.

### Formati supportati

* A partire dalla versione 23.6, è possibile salvare un documento in formato XLSX. Ora puoi convertire i tuoi documenti in formato Excel. <sup>23.6</sup>

* A partire dalla versione 23.7, è possibile salvare una pagina o una forma del documento in formato EPS. <sup>23.7</sup>

### Nuove funzionalità di formato

- È stata introdotta la funzionalità per generare automaticamente il Sommario (TOC) per i documenti MOBI. <sup>23.8</sup>
- Il costruttore [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) è stato espanso con [PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions). <sup>23.8</sup>
- È stata implementata la modellatura del testo verticale per metafile EMF. <sup>23.8</sup>

### Rendering

#### Ottenere e modificare i dati delle serie di grafici <sup>23.5</sup>

La funzione per ottenere e modificare i dati delle serie di grafici è stata fornita aggiungendo:

- nuove classi: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- nuovi tipi di enum: [ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### Supporto per tipografia avanzata <sup>23.6</sup>

È stato aggiunto il supporto per la tipografia avanzata nel rendering WMF, EMF e EMF+.

#### Contenuto colorato sulla pagina <sup>23.6</sup>

La proprietà pubblica [PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/), che indica se la pagina è colorata o meno, è stata aggiunta.

#### Formattazione per le etichette dei dati del grafico <sup>23.6</sup>

È stata implementata la possibilità di impostare la formattazione di riempimento, traccia e callout per le etichette dei dati del grafico.

### Mail Merge e rapporti

#### Inserimento dinamico HTML per il motore di reportistica LINQ <sup>23.6</sup>

È stato aggiunto un nuovo modo di inserimento dinamico HTML per il motore di reportistica LINQ.

#### Mustache Tag Supporto <sup>23.7</sup>

I tag Mustache sono ora supportati nei metodi [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/) e [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/).

#### Specificare la dimensione delle immagini renderizzate <sup>23.8</sup>

È stata introdotta una nuova proprietà pubblica [image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/) per specificare la dimensione delle immagini renderizzate in pixel.

#### Conserva spazi bianchi per JSON Valori stringa - LINQ <sup>23.8</sup>

È stata aggiunta un'opzione al motore di reporting LINQ per preservare gli spazi bianchi per i valori di stringa JSON.

### LowCode <sup>23.6</sup>

Sono stati aggiunti nuovi metodi LowCode destinati a unire diversi tipi di documenti in un singolo documento di output.

### Altri

- È stato implementato il supporto per il wrapping del testo nelle intestazioni/piè di pagina. <sup>23.5</sup>
- La possibilità di rimuovere le firme digitali dai documenti ODT è stata aggiunta tramite il metodo [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str). <sup>23.5</sup>
- È stata aggiunta la proprietà pubblica [phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/) per ottenere il testo base e ruby della guida fonetica [Run](https://reference.aspose.com/words/python-net/aspose.words/run/). <sup>23.5</sup>
- La possibilità di recuperare un valore di firma digitale da un documento con firma digitale come matrice di byte è stata aggiunta introducendo una nuova proprietà [signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/). <sup>23.7</sup>
- Le classi [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/) e [Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/) sono state ampliate con nuovi membri pubblici– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), e [Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/). <sup>23.7</sup>

{{% alert color="primary" %}}

Scopri di più su [Aspose.Wordsper Python via .NET 23.5 Note di rilascio](/words/python-net/aspose-words-for-python-via-dotnet-23-5-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 23.6 Note di rilascio](/words/python-net/aspose-words-for-python-via-dotnet-23-6-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 23.7 Note di rilascio](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

Scopri di più su [Aspose.Wordsper Python via .NET 23.8 Note di rilascio](/words/python-net/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## Vedi anche

{{% alert color="primary" %}}

Questa pagina contiene le ultime notizie di rilascio degli ultimi 2 anni. Per i dettagli sulle versioni precedenti, vedere [Note di rilascio'](https://releases.aspose.com/words/python/release-notes/) pagine nelle relative sezioni.

{{% /alert %}}
