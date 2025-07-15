---
title: Word naar PDF converteren in C#
second_title: Aspose.Words voor .NET
articleTitle: Document naar PDF omzetten
linktitle: Document naar PDF omzetten
description: "Word naar PDF converteren in C#. Eenvoudige codevoorbeelden voor DOCX naar PDF conversie. Ondersteunt alle Word-formaten en afbeeldingen."
type: docs
weight: 10
url: /nl/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Het vermogen om documenten eenvoudig en betrouwbaar van het ene formaat naar het andere te converteren is een belangrijke functie van Aspose.Words. PDF is een van de meest populaire formaten voor conversie – het is een formaat met vaste lay-out dat de oorspronkelijke weergave van een document behoudt bij rendering op verschillende platformen. De term "rendering" wordt in Aspose.Words gebruikt om het proces van het omzetten van een document naar een bestandsformaat dat gepagineerd is of het concept van pagina's heeft te beschrijven.

## Word-document naar PDF converteren

Conversie van Word naar PDF is een vrij complex proces dat verschillende rekenfasen vereist. De lay-out engine van Aspose.Words imiteert de manier waarop de pagina lay-out engine van Microsoft Word werkt, waardoor PDF-uitvoerdocumenten er zo dicht mogelijk bij uitzien als wat u kunt zien in Microsoft Word.

Met Aspose.Words kunt u programmatisch een document van Word-formaten, zoals DOC of DOCX, naar PDF omzetten zonder Microsoft Office te gebruiken. Dit artikel legt uit hoe u deze conversie uitvoert.

{{% alert color="primary" %}}

Merk op dat het aantal pagina's in een document de conversietijd beïnvloedt.

{{% /alert %}}

### DOCX of DOC naar PDF converteren

Het transformeren van DOC of DOCX documentformaat naar PDF-formaat in Aspose.Words is zeer eenvoudig en kan worden bereikt met slechts twee regels code die:

1. Laad uw document in een [Document](https://reference.aspose.com/words/net/aspose.words/document/)-object met behulp van een van zijn constructors door de documentnaam met zijn formaatextensie te specificeren.
1. Roep een van de [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/)-methoden aan op het **Document**-object en specificeer het gewenste uitvoerformaat als PDF door een bestandsnaam met de extensie ".PDF" in te voeren.

Het volgende codevoorbeeld toont hoe u een document van DOCX naar PDF converteert met behulp van de [Save](https://reference.aspose.com/words/net/aspose.words/document/save/)-methode:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

U kunt het sjabloonbestand van dit voorbeeld downloaden van [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Soms is het nodig om aanvullende opties te specificeren die het resultaat van het opslaan van een document als PDF kunnen beïnvloeden. Deze opties kunnen worden gespecificeerd door gebruik te maken van de [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)-klasse, die eigenschappen bevat die bepalen hoe de PDF-uitvoer wordt weergegeven.

Merk op dat u met dezelfde techniek elk document met flow-layout formaat naar PDF-formaat kunt transformeren.

{{% /alert %}}

### Converteren naar verschillende PDF-standaarden

Aspose.Words biedt de [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/)-enumeratie om de conversie van DOC of DOCX naar verschillende PDF-formaatstandaarden (zoals PDF 1.7, PDF 1.5, enz.) te ondersteunen.

Het volgende codevoorbeeld toont hoe u een document naar PDF 1.7 converteert met behulp van [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) met naleving van PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Afbeeldingen naar PDF converteren

Converteren naar PDF is niet beperkt tot Microsoft Word-documentformaten. Elk formaat dat door Aspose.Words wordt ondersteund, inclusief programmatisch gecreëerde, kan ook worden omgezet naar PDF. We kunnen bijvoorbeeld enkelvoudige afbeeldingen, zoals JPEG, PNG, BMP, EMF, of WMF, evenals meervoudige afbeeldingen, zoals TIFF en GIF, naar PDF transformeren.

Het volgende codevoorbeeld toont hoe u JPEG- en TIFF-afbeeldingen naar PDF converteert:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Om deze code te laten werken, moet u referenties naar Aspose.Words en `System.Drawing` toevoegen aan uw project.

## PDF-uitvoergrootte verkleinen

Bij het opslaan naar PDF kunt u specificeren of u de uitvoer wilt optimaliseren. Om dit te doen, moet u de [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/)-vlag op true instellen, en dan worden overtollige geneste en lege canvassen weggenomen, aangrenzende glyphs met dezelfde opmaak worden samengevoegd.

Het volgende codevoorbeeld toont hoe u de uitvoer kunt optimaliseren:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Het gebruik van de **OptimizeOutput**-eigenschap kan de nauwkeurigheid van contentweergave beïnvloeden.

{{% /alert %}}

## Zie ook

- Het artikel [Rendering](/words/nl/net/rendering/) voor meer informatie over vaste pagina en flow-layout formaten
- Het artikel [Conversie naar vast paginaformaat](/words/nl/net/converting-to-fixed-page-format/#what-is-a-page-layout) voor meer informatie over pagina-indeling
- Het artikel [Renderingopties specificeren bij converteren naar PDF](/words/nl/net/specify-rendering-options-when-converting-to-pdf/) voor meer informatie over het gebruik van de `PdfSaveOptions`-klasse
- Het artikel [Leer de functies van conversie naar PDF/A en PDF/UA](/words/nl/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) dat beschrijft welke PDF-standaard en de relevante ISO's voor PDF-standaarden worden ondersteund door Aspose.Words
- Het artikel [Welke PDF-standaard is beter om te kiezen](/words/nl/net/which-pdf-standard-is-better-to-choose/) om te bepalen welke PDF-standaarden zinvol zijn voor welke gevallen

- Het artikel [Werken met PDF/A of PDF/UA](/words/nl/net/working-with-pdfa-or-pdfua/) beschrijft de vereisten voor documentinhoud in PDF/A en PDF/UA formaten – hoofdzakelijk de vereisten voor structuur en lettertypen

- Het artikel [Waarschuwingen voor toegankelijkheidsproblemen bij opslaan naar PDF/A en PDF/UA](/words/nl/net/warnings-when-saving-to-pdfa-and-pdfua/) beschrijft welke contenttoegankelikheidseisen PDF/A en PDF/UA opleggen
