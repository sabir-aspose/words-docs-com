---
title: Utilizzo della filigrana in Python
second_title: Aspose.Words per Python via .NET
articleTitle: Lavorare con Watermark
linktitle: Lavorare con Watermark
description: "Creare e gestire filigrane in un documento utilizzando Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /it/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

In questo argomento viene illustrato come lavorare a livello di programmazione con la filigrana utilizzando Aspose.Words. Una filigrana è un'immagine di sfondo che viene visualizzata dietro il testo di un documento. Una filigrana può contenere un testo o un'immagine rappresentata dalla classe [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Prova online**

Puoi provare questa funzionalità con il nostro [Filigrana di documenti online gratuita](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Come aggiungere una filigrana a un documento

In Microsoft Word, una filigrana può essere facilmente inserita in un documento utilizzando il comando Inserisci filigrana. Aspose.Words fornisce la classe [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) per aggiungere o rimuovere la filigrana nei documenti. Aspose.Words fornisce l'enumerazione [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) che definisce tre possibili tipi di filigrane ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) e [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) con cui lavorare.

### Aggiungi filigrana di testo

Nell'esempio di codice seguente viene illustrato come inserire una filigrana di testo in un documento definendo [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) utilizzando il metodo [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### Aggiungi Filigrana immagine

Nell'esempio di codice seguente viene illustrato come inserire una filigrana di immagine in un documento definendo [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) utilizzando il metodo [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

La filigrana dell'immagine può essere inserita come immagine, stringa o flusso.

La filigrana può anche essere inserita usando la classe shape. È molto facile inserire qualsiasi forma o immagine in un'intestazione o piè di pagina e quindi creare una filigrana di qualsiasi tipo immaginabile.

L'esempio di codice seguente inserisce una filigrana in un documento Word:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

È possibile scaricare il file modello di questo esempio da [qui](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Rimuovere la filigrana da un documento

La classe [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) fornisce il metodo remove per rimuovere la filigrana da un documento.

Il seguente esempio di codice mostra come rimuovere una filigrana dai documenti:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

Se le filigrane vengono aggiunte utilizzando l'oggetto classe [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/), per rimuovere la filigrana da un documento è necessario impostare solo il nome della forma filigrana durante l'inserimento e quindi rimuovere la forma filigrana con un nome assegnato.

L'esempio di codice seguente mostra come impostare il nome della forma della filigrana e rimuoverla dal documento:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## Aggiungere una filigrana nella cella della tabella

A volte è necessario inserire una filigrana/immagine nella cella di una tabella e visualizzarla all'esterno della tabella, è possibile utilizzare la proprietà [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/). Questa proprietà ottiene o imposta un flag che indica se la forma viene visualizzata all'interno di una tabella o all'esterno di essa. Si noti che questa proprietà funziona solo quando si ottimizza il documento per Microsoft Word 2010 utilizzando il metodo [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

Il seguente esempio di codice mostra come utilizzare questa proprietà:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
