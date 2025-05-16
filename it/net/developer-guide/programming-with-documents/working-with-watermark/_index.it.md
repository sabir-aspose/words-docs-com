---
title: Utilizzo della filigrana in C#
second_title: Aspose.Wordsper .NET
articleTitle: Lavorare con Watermark
linktitle: Lavorare con Watermark
description: "Manipolazione filigrana documento utilizzando C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /it/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

In questo argomento viene illustrato come lavorare a livello di programmazione con la filigrana utilizzando Aspose.Words. Una filigrana è un'immagine di sfondo che viene visualizzata dietro il testo di un documento. Una filigrana può contenere un testo o un'immagine rappresentata dalla classe [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Prova online**

Puoi provare questa funzionalità con il nostro [Filigrana di documenti online gratuita](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Aggiungere una filigrana a un documento

In Microsoft Word, una filigrana può essere facilmente inserita in un documento utilizzando il comando Inserisci filigrana. Aspose.Words fornisce la classe [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) per aggiungere o rimuovere la filigrana nei documenti. Aspose.Words fornisce l'enumerazione [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/) che definisce tre possibili tipi di filigrane (Testo, Immagine e Nessuna) con cui lavorare.

### Aggiungi filigrana di testo

Nell'esempio di codice seguente viene illustrato come inserire una filigrana di testo in un documento definendo [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) utilizzando il metodo [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Aggiungi Filigrana immagine

Nell'esempio di codice seguente viene illustrato come inserire una filigrana di immagine in un documento definendo [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) utilizzando il metodo [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

La filigrana dell'immagine può essere inserita come immagine, stringa o flusso.

La filigrana può anche essere inserita usando la classe shape. È molto facile inserire qualsiasi forma o immagine in un'intestazione o piè di pagina e quindi creare una filigrana di qualsiasi tipo immaginabile.

L'esempio di codice seguente inserisce una filigrana in un documento Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

È possibile scaricare il file di esempio di questo esempio da [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Rimuovere la filigrana da un documento

La classe [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) fornisce il metodo remove per rimuovere la filigrana da un documento.

Il seguente esempio di codice mostra come rimuovere una filigrana dai documenti:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Se le filigrane vengono aggiunte utilizzando l'oggetto classe [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/), per rimuovere la filigrana da un documento è necessario impostare solo il nome della forma filigrana durante l'inserimento e quindi rimuovere la forma filigrana con un nome assegnato.

L'esempio di codice seguente mostra come impostare il nome della forma della filigrana e rimuoverla dal documento:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Aggiungere una filigrana in una cella di tabella

A volte è necessario inserire una filigrana/immagine nella cella di una tabella e visualizzarla all'esterno della tabella, è possibile utilizzare la proprietà [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). Questa proprietà ottiene o imposta un flag che indica se la forma viene visualizzata all'interno di una tabella o all'esterno di essa. Si noti che questa proprietà funziona solo quando si ottimizza il documento per Microsoft Word 2010 utilizzando il metodo [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

Il seguente esempio di codice mostra come utilizzare questa proprietà:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
