---
title: Converti Word în PDF în C#
second_title: Aspose.Words pentru .NET
articleTitle: Transforma document în PDF
linktitle: Transforma document în PDF
description: "Converti Word în PDF în C#. Exemple de cod simple pentru conversie DOCX în PDF. Suportă toate formatele Word și imaginile."
type: docs
weight: 10
url: /ro/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Capacitatea de a converti documente ușor și fiabil dintr-un format în altul este o caracteristică cheie a Aspose.Words. PDF este unul dintre formatele cele mai populare pentru conversie – este un format cu aspect fix care păstrează aspectul original al unui document în timpul redării pe diverse platforme. Termenul "redare" este utilizat în Aspose.Words pentru a descrie procesul de conversie a unui document într-un format de fișier paginat sau care are conceptul de pagini.

## Converti document Word în PDF

Conversia din Word în PDF este un proces destul de complex care necesită mai multe etape de calcul. Motorul de layout al Aspose.Words imită modul în care funcționează motorul de layout al paginilor Microsoft Word, făcând ca documentele PDF de ieșire să arate cât mai aproape posibil de ceea ce puteți vedea în Microsoft Word.

Cu Aspose.Words puteți transforma programatic un document din formatele Word, cum ar fi DOC sau DOCX, în PDF fără a utiliza Microsoft Office. Acest articol explică cum să realizați această conversie.

{{% alert color="primary" %}}

Rețineți că numărul de pagini dintr-un document afectează timpul de conversie.

{{% /alert %}}

### Converti DOCX sau DOC în PDF

Transformarea din formatul de document DOC sau DOCX în formatul PDF în Aspose.Words este foarte simplă și poate fi realizată cu doar două linii de cod care:

1. Încărcați documentul vostru într-un obiect [Document](https://reference.aspose.com/words/net/aspose.words/document/) utilizând unul dintre constructorii săi prin specificarea numelui documentului cu extensia sa de format.
1. Invocați una dintre metodele [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) pe obiectul **Document** și specificați formatul de ieșire dorit ca PDF prin introducerea unui nume de fișier cu extensia ".PDF".

Următorul exemplu de cod arată cum să convertiți un document din DOCX în PDF utilizând metoda [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Puteți descărca fișierul șablon al acestui exemplu din [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Uneori este necesar să specificați opțiuni suplimentare care pot afecta rezultatul salvării unui document ca PDF. Aceste opțiuni pot fi specificate utilizând clasa [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), care conține proprietăți ce determină modul în care va fi afișată ieșirea PDF.

Rețineți că cu aceeași tehnică puteți schimba orice document cu format de flux în format PDF.

{{% /alert %}}

### Transforma în diferite standarde PDF

Aspose.Words oferă enumerația [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) pentru a sprijini conversia DOC sau DOCX în diverse standarde de format PDF (cum ar fi PDF 1.7, PDF 1.5, etc.).

Următorul exemplu de cod demonstrează cum să convertiți un document în PDF 1.7 utilizând [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) cu conformitate la PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Converti imagini în PDF

Conversia în PDF nu este restricționată la formatele de documente Microsoft Word. Orice format suportat de Aspose.Words, inclusiv cele create programatic, poate fi de asemenea transformat în PDF. De exemplu, putem converti imagini cu o singură pagină, cum ar fi JPEG, PNG, BMP, EMF, sau WMF, precum și imagini cu mai multe pagini, cum ar fi TIFF și GIF, în PDF.

Următorul exemplu de cod arată cum să schimbați imagini JPEG și TIFF în PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Pentru ca acest cod să funcționeze, trebuie să adăugați referințe la Aspose.Words și `System.Drawing` în proiectul vostru.

## Reducerea dimensiunii de ieșire PDF

Când salvați în PDF, puteți specifica dacă doriți să optimizați ieșirea. Pentru a face acest lucru, trebuie să setați steagul [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) la true, iar apoi canvasurile imbricate redundante și goale vor fi eliminate, glifele adiacente cu aceeași formatare vor fi concatenate.

Următorul exemplu de cod arată cum să optimizați ieșirea:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Utilizarea proprietății **OptimizeOutput** poate afecta acuratețea afișării conținutului.

{{% /alert %}}

## Vezi și

- Articolul [Redare](/words/ro/net/rendering/) pentru mai multe informații despre formatele cu pagină fixă și flux de layout
- Articolul [Conversie în format cu pagină fixă](/words/net/converting-to-fixed-page-format/#what-is-a-page-layout) pentru mai multe informații despre layout-ul paginii
- Articolul [Specificarea opțiunilor de redare la transformarea în PDF](/words/ro/net/specify-rendering-options-when-converting-to-pdf/) pentru mai multe informații despre utilizarea clasei `PdfSaveOptions`
- Articolul [Învățați caracteristicile conversiei în PDF/A și PDF/UA](/words/ro/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) care descrie ce standard PDF și ISO-urile relevante pentru standardele PDF sunt suportate de Aspose.Words
- Articolul [Ce standard PDF este mai bine să alegeți](/words/ro/net/which-pdf-standard-is-better-to-choose/) pentru a determina care standarde PDF au sens pentru care cazuri

- Articolul [Lucrul cu PDF/A sau PDF/UA](/words/ro/net/working-with-pdfa-or-pdfua/) descrie cerințele pentru conținutul documentului în formatele PDF/A și PDF/UA – în principal cerințele pentru structură și fonturi

- Articolul [Avertismente privind problemele de accesibilitate la salvarea în PDF/A și PDF/UA](/words/ro/net/warnings-when-saving-to-pdfa-and-pdfua/) descrie ce cerințe de accesibilitate a conținutului impun PDF/A și PDF/UA
