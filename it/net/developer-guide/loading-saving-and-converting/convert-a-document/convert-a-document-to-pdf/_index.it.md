---
title: Convertire Word in PDF in C#
second_title: Aspose.Words per .NET
articleTitle: Trasformare documento in PDF
linktitle: Trasformare documento in PDF
description: "Convertire Word in PDF in C#. Semplici esempi di codice per conversione DOCX in PDF. Supporta tutti i formati Word e immagini."
type: docs
weight: 10
url: /it/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

La capacità di convertire facilmente e affidabilmente i documenti da un formato all'altro è una caratteristica chiave di Aspose.Words. PDF è uno dei formati più popolari per la conversione – è un formato a layout fisso che preserva l'aspetto originale di un documento durante il rendering su diverse piattaforme. Il termine "rendering" è utilizzato in Aspose.Words per descrivere il processo di conversione di un documento in un formato di file paginato o che ha il concetto di pagine.

## Convertire documento Word in PDF

La conversione da Word a PDF è un processo abbastanza complesso che richiede diverse fasi di calcolo. Il motore di layout di Aspose.Words imita il modo in cui funziona il motore di layout delle pagine di Microsoft Word, rendendo i documenti PDF di output il più vicini possibile a quello che puoi vedere in Microsoft Word.

Con Aspose.Words puoi convertire programmaticamente un documento dai formati Word, come DOC o DOCX, in PDF senza utilizzare Microsoft Office. Questo articolo spiega come eseguire questa trasformazione.

{{% alert color="primary" %}}

Nota che il numero di pagine in un documento influisce sul tempo di conversione.

{{% /alert %}}

### Convertire DOCX o DOC in PDF

La trasformazione dal formato documento DOC o DOCX al formato PDF in Aspose.Words è molto semplice e può essere realizzata con solo due righe di codice che:

1. Carica il tuo documento in un oggetto [Document](https://reference.aspose.com/words/net/aspose.words/document/) utilizzando uno dei suoi costruttori specificando il nome del documento con la sua estensione di formato.
1. Invoca uno dei metodi [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) sull'oggetto **Document** e specifica il formato di output desiderato come PDF inserendo un nome file con estensione ".PDF".

L'esempio di codice seguente mostra come convertire un documento da DOCX a PDF utilizzando il metodo [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Puoi scaricare il file template di questo esempio da [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

A volte è necessario specificare opzioni aggiuntive che possono influenzare il risultato del salvataggio di un documento come PDF. Queste opzioni possono essere specificate utilizzando la classe [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), contenente proprietà che determinano come verrà mostrato l'output PDF.

Nota che con la stessa tecnica puoi trasformare qualsiasi documento in formato flow-layout nel formato PDF.

{{% /alert %}}

### Convertire in diversi standard PDF

Aspose.Words fornisce l'enumerazione [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) per supportare la conversione di DOC o DOCX in vari standard di formato PDF (come PDF 1.7, PDF 1.5, ecc.).

L'esempio di codice seguente dimostra come cambiare un documento in PDF 1.7 utilizzando [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) con conformità a PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Convertire immagini in PDF

La conversione in PDF non è limitata ai formati di documento Microsoft Word. Qualsiasi formato supportato da Aspose.Words, inclusi quelli creati programmaticamente, può anche essere trasformato in PDF. Ad esempio, possiamo convertire immagini a pagina singola, come JPEG, PNG, BMP, EMF, o WMF, così come immagini multi-pagina, come TIFF e GIF, in PDF.

L'esempio di codice seguente mostra come cambiare immagini JPEG e TIFF in PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Per far funzionare questo codice, devi aggiungere riferimenti ad Aspose.Words e `System.Drawing` nel tuo progetto.

## Ridurre la dimensione dell'output PDF

Quando salvi in PDF, puoi specificare se vuoi ottimizzare l'output. Per fare questo, devi impostare il flag [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) su true, e quindi verranno rimossi canvas annidati ridondanti e vuoti, i glifi adiacenti con la stessa formattazione verranno concatenati.

L'esempio di codice seguente mostra come ottimizzare l'output:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

L'utilizzo della proprietà **OptimizeOutput** può influenzare l'accuratezza della visualizzazione del contenuto.

{{% /alert %}}

## Vedi anche

- L'articolo [Rendering](/words/it/net/rendering/) per ulteriori informazioni sui formati a pagina fissa e flow-layout
- L'articolo [Conversione in formato a pagina fissa](/words/it/net/converting-to-fixed-page-format/#what-is-a-page-layout) per ulteriori informazioni sul layout di pagina
- L'articolo [Specificare opzioni di rendering durante la trasformazione in PDF](/words/it/net/specify-rendering-options-when-converting-to-pdf/) per ulteriori informazioni sull'utilizzo della classe `PdfSaveOptions`
- L'articolo [Impara le caratteristiche della conversione in PDF/A e PDF/UA](/words/it/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) che descrive quale standard PDF e gli ISO rilevanti per gli standard PDF sono supportati da Aspose.Words
- L'articolo [Quale standard PDF è meglio scegliere](/words/it/net/which-pdf-standard-is-better-to-choose/) per determinare quali standard PDF hanno senso per quali casi

- L'articolo [Lavorare con PDF/A o PDF/UA](/words/it/net/working-with-pdfa-or-pdfua/) descrive i requisiti per il contenuto del documento nei formati PDF/A e PDF/UA – principalmente i requisiti per la struttura e i font

- L'articolo [Avvisi di problemi di accessibilità quando si salva in PDF/A e PDF/UA](/words/it/net/warnings-when-saving-to-pdfa-and-pdfua/) descrive quali requisiti di accessibilità del contenuto impongono PDF/A e PDF/UA
