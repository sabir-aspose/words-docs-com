---
title: Lucrul cu filigran în C#
second_title: Aspose.Words pentru .NET
articleTitle: Lucrul cu filigran
linktitle: Lucrul cu filigran
description: "Manipularea filigranului documentului folosind C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ro/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Acest subiect discută cum să lucrați programatic cu filigran folosind Aspose.Words. Un filigran este o imagine de fundal care se afișează în spatele textului dintr-un document. Un filigran poate conține un text sau o imagine reprezentată de clasa [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Încercați online**

Puteți încerca această funcționalitate cu [Filigran online gratuit pentru documente](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Adăugarea unui filigran la un Document

În Microsoft Word, un filigran poate fi inserat cu ușurință într-un document folosind comanda Insert Watermark. Aspose.Words oferă clasa [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) pentru a adăuga sau elimina filigranul în documente. Aspose.Words oferă enumerarea [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)definind trei tipuri posibile de filigrane (Text, imagine și niciuna) cu care să lucrați.

### Adăugați Filigran Text

Următorul exemplu de cod demonstrează cum să inserați un filigran text într-un document definind [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) folosind metoda [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Adăugați Filigran De Imagine

Următorul exemplu de cod demonstrează cum să inserați un filigran de imagine într-un document definind [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) folosind metoda [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Filigranul imaginii poate fi inserat ca imagine, șir sau flux.

Filigranul poate fi, de asemenea, inserat folosind clasa de formă. Este foarte ușor să inserați orice formă sau imagine într-un antet sau subsol și astfel să creați un filigran de orice tip imaginabil.

Următorul exemplu de cod introduce un filigran într-un document Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Puteți descărca fișierul eșantion al acestui exemplu din [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Eliminați filigranul dintr-un Document

Clasa [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) oferă metoda remove pentru a elimina filigranul dintr-un document.

Următorul exemplu de cod arată cum să eliminați un filigran din documente:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Dacă Filigranele sunt adăugate folosind obiectul clasei [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/), atunci pentru a elimina filigranul dintr-un document, trebuie să setați doar numele formei filigranului în timpul inserării și apoi să eliminați forma filigranului printr-un nume atribuit.

Următorul exemplu de cod vă arată cum să setați numele formei filigranului și să îl eliminați din document:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Adăugați un filigran într-o celulă de tabel

Uneori trebuie să introduceți un filigran/imagine în celula unui tabel și să o afișați în afara tabelului, puteți utiliza proprietatea [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). Această proprietate primește sau setează un steag care indică dacă forma este afișată în interiorul unui tabel sau în afara acestuia. Rețineți că această proprietate funcționează numai atunci când optimizați documentul pentru Microsoft Word 2010 folosind metoda [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

Următorul exemplu de cod arată cum să utilizați această proprietate:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
