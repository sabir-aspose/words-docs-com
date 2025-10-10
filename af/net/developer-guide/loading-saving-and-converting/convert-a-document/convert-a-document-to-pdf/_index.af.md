---
title: Omskep Word na PDF in C#
second_title: Aspose.Words vir .NET
articleTitle: Verander dokument na PDF
linktitle: Verander dokument na PDF
description: "Omskep Word na PDF in C#. Eenvoudige kode voorbeelde vir DOCX na PDF omskepping. Ondersteun alle Word formate en beelde."
type: docs
weight: 10
url: /af/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Die vermoë om dokumente maklik en betroubaar van een formaat na 'n ander te omskep is 'n kernfunksie van Aspose.Words. PDF is een van die gewildste formate vir omskepping – dit is 'n formaat met vaste uitleg wat die oorspronklike voorkoms van 'n dokument behou tydens weergawe op verskillende platforms. Die term "weergawe" word in Aspose.Words gebruik om die proses te beskryf van die verander van 'n dokument na 'n lêerformaat wat gepagineer is of die konsep van bladsye het.

## Omskep Word dokument na PDF

Omskepping van Word na PDF is 'n redelik komplekse proses wat verskeie stadiums van berekening vereis. Die uitleg-enjin van Aspose.Words boots die werking van Microsoft Word se bladsy-uitleg enjin na, wat maak dat PDF uitset dokumente so na as moontlik lyk aan wat jy in Microsoft Word kan sien.

Met Aspose.Words kan jy programmaties 'n dokument van Word formate, soos DOC of DOCX, na PDF omskakel sonder om Microsoft Office te gebruik. Hierdie artikel verduidelik hoe om hierdie omskepping uit te voer.

{{% alert color="primary" %}}

Let daarop dat die aantal bladsye in 'n dokument die omskeppingstyd beïnvloed.

{{% /alert %}}

### Omskep DOCX of DOC na PDF

Verander van DOC of DOCX dokument formaat na PDF formaat in Aspose.Words is baie eenvoudig en kan bereik word met slegs twee lyne kode wat:

1. Laai jou dokument in 'n [Document](https://reference.aspose.com/words/net/aspose.words/document/) objek deur een van sy konstruktors te gebruik deur die dokument naam met sy formaat uitbreiding te spesifiseer.
1. Roep een van die [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) metodes op die **Document** objek aan en spesifiseer die gewenste uitset formaat as PDF deur 'n lêer naam met die ".PDF" uitbreiding in te voer.

Die volgende kode voorbeeld toon hoe om 'n dokument van DOCX na PDF te omskep deur die [Save](https://reference.aspose.com/words/net/aspose.words/document/save/) metode te gebruik:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Jy kan die sjabloon lêer van hierdie voorbeeld aflaai van [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Soms is dit nodig om addisionele opsies te spesifiseer wat die resultaat van die stoor van 'n dokument as PDF kan beïnvloed. Hierdie opsies kan gespesifiseer word deur die [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) klas te gebruik, wat eienskappe bevat wat bepaal hoe die PDF uitset vertoon sal word.

Let daarop dat met dieselfde tegniek jy enige vloei-uitleg formaat dokument na PDF formaat kan omskakel.

{{% /alert %}}

### Verander na verskillende PDF standaarde

Aspose.Words bied die [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) opsomming om die omskepping van DOC of DOCX na verskeie PDF formaat standaarde (soos PDF 1.7, PDF 1.5, ens.) te ondersteun.

Die volgende kode voorbeeld demonstreer hoe om 'n dokument na PDF 1.7 te omskep deur [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) te gebruik met nakoming van PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Omskep beelde na PDF

Omskepping na PDF is nie beperk tot Microsoft Word dokument formate nie. Enige formaat wat deur Aspose.Words ondersteun word, insluitend dié wat programmaties geskep is, kan ook na PDF verander word. Byvoorbeeld, ons kan enkelbladsy beelde, soos JPEG, PNG, BMP, EMF, of WMF, sowel as meerbladsy beelde, soos TIFF en GIF, na PDF omskep.

Die volgende kode voorbeeld toon hoe om JPEG en TIFF beelde na PDF te omskakel:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Om hierdie kode te laat werk, moet jy verwysings na Aspose.Words en `System.Drawing` by jou projek voeg.

## Verminder PDF uitset grootte

Wanneer jy na PDF stoor, kan jy spesifiseer of jy die uitset wil optimeer. Om dit te doen, moet jy die [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) vlag op waar stel, en dan sal oortollige geneste en leë kanvasse verwyder word, aangrensende glywe met dieselfde formatering sal saamgevoeg word.

Die volgende kode voorbeeld toon hoe om die uitset te optimeer:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Die gebruik van die **OptimizeOutput** eienskap kan die akkuraatheid van inhoud vertoning beïnvloed.

{{% /alert %}}

## Sien ook

- Die artikel [Weergawe](/words/af/net/rendering/) vir meer inligting oor vaste bladsy en vloei-uitleg formate
- Die artikel [Omskepping na vaste bladsy formaat](/words/af/net/converting-to-fixed-page-format/#what-is-a-page-layout) vir meer inligting oor bladsy uitleg
- Die artikel [Spesifiseer weergawe opsies wanneer jy na PDF verander](/words/af/net/specify-rendering-options-when-converting-to-pdf/) vir meer inligting oor die gebruik van die `PdfSaveOptions` klas
- Die artikel [Leer die kenmerke van omskepping na PDF/A en PDF/UA](/words/af/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) wat beskryf watter PDF standaard en relevante ISO's vir PDF standaarde deur Aspose.Words ondersteun word
- Die artikel [Watter PDF standaard is beter om te kies](/words/af/net/which-pdf-standard-is-better-to-choose/) om te bepaal watter PDF standaarde sin maak vir watter gevalle

- Die artikel [Werk met PDF/A of PDF/UA](/words/af/net/working-with-pdfa-or-pdfua/) beskryf die vereistes vir dokument inhoud in PDF/A en PDF/UA formate – hoofsaaklik die vereistes vir struktuur en lettertipes

- Die artikel [Waarskuwings vir toeganklikheid probleme wanneer jy na PDF/A en PDF/UA stoor](/words/af/net/warnings-when-saving-to-pdfa-and-pdfua/) beskryf watter inhoud toeganklikheid vereistes PDF/A en PDF/UA oplê
