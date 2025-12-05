---
title: Werken met watermerk in C#
second_title: Aspose.Words voor .NET
articleTitle: Werken met Watermark
linktitle: Werken met Watermark
description: "Document watermerk manipulatie met behulp van C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nl/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

In dit onderwerp wordt besproken hoe u programmatisch met watermerk kunt werken met Aspose.Words. Een watermerk is een achtergrondafbeelding die achter de tekst in een document wordt weergegeven. Een watermerk kan een tekst of een afbeelding bevatten die wordt weergegeven door de klasse [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Online proberen**

U kunt deze functionaliteit proberen met onze [Gratis online document watermerk](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Een watermerk aan een Document toevoegen

In Microsoft Word kan een watermerk eenvoudig in een document worden ingevoegd met de opdracht watermerk invoegen. Aspose.Words biedt de [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) klasse voor het toevoegen of verwijderen van watermerken in documenten. Aspose.Words geeft de [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)opsomming die drie mogelijke typen watermerken definieert (tekst, afbeelding en geen) om mee te werken.

### Tekst Watermerk Toevoegen

Het volgende codevoorbeeld laat zien hoe u een tekstwatermerk invoegt in een document door [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) te definiëren met de methode [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Afbeelding Toevoegen Watermerk

Het volgende codevoorbeeld laat zien hoe u een watermerk voor een afbeelding invoegt in een document door [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) te definiëren met de methode [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Beeldwatermerk kan worden ingevoegd als afbeelding, tekenreeks of stream.

Het watermerk kan ook worden ingevoegd met behulp van de vormklasse. Het is heel eenvoudig om elke vorm of afbeelding in een kop-of voettekst in te voegen en zo een watermerk van elk denkbaar type te maken.

Het volgende codevoorbeeld voegt een watermerk in een Word document:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

U kunt het voorbeeldbestand van dit voorbeeld downloaden van [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Watermerk uit een Document verwijderen

De klasse [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) biedt de methode verwijderen om het watermerk uit een document te verwijderen.

Het volgende codevoorbeeld laat zien hoe u een watermerk uit documenten verwijdert:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Als de watermerken worden toegevoegd met het [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/) class-object, moet u om het watermerk uit een document te verwijderen alleen de naam van de watermerkshape instellen tijdens het invoegen en vervolgens de watermerkshape verwijderen met een toegewezen naam.

In het volgende codevoorbeeld ziet u hoe u de naam van de watermerkshape instelt en deze uit het document verwijdert:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Een watermerk toevoegen aan een tabelcel

Soms moet u een watermerk/afbeelding in de cel van een tabel invoegen en deze buiten de tabel weergeven, U kunt de eigenschap [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/) gebruiken. Deze eigenschap krijgt of stelt een vlag die aangeeft of de vorm wordt weergegeven binnen of buiten een tabel. Merk op dat deze eigenschap alleen werkt wanneer u het document optimaliseert voor Microsoft Word 2010 met de methode [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

Het volgende codevoorbeeld laat zien hoe deze eigenschap te gebruiken:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
