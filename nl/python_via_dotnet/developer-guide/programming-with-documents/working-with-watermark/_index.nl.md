---
title: Werken met watermerk in Python
second_title: Aspose.Words voor Python via .NET
articleTitle: Werken met Watermark
linktitle: Werken met Watermark
description: "Watermerken maken en beheren in een document met Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nl/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

In dit onderwerp wordt besproken hoe u programmatisch met watermerk kunt werken met Aspose.Words. Een watermerk is een achtergrondafbeelding die achter de tekst in een document wordt weergegeven. Een watermerk kan een tekst of een afbeelding bevatten die wordt weergegeven door de klasse [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Online proberen**

U kunt deze functionaliteit proberen met onze [Gratis online document watermerk](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Een watermerk toevoegen aan een Document

In Microsoft Word kan een watermerk eenvoudig in een document worden ingevoegd met de opdracht watermerk invoegen. Aspose.Words biedt de [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) klasse voor het toevoegen of verwijderen van watermerken in documenten. Aspose.Words geeft de[WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) opsomming die drie mogelijke soorten watermerken definieert ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) en [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) om mee te werken.

### Tekst Watermerk Toevoegen

Het volgende codevoorbeeld laat zien hoe u een tekstwatermerk invoegt in een document door [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) te definiëren met de methode [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### Afbeelding Toevoegen Watermerk

Het volgende codevoorbeeld laat zien hoe u een watermerk voor een afbeelding invoegt in een document door [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) te definiëren met de methode [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

Beeldwatermerk kan worden ingevoegd als afbeelding, tekenreeks of stream.

Het watermerk kan ook worden ingevoegd met behulp van de vormklasse. Het is heel eenvoudig om elke vorm of afbeelding in een kop-of voettekst in te voegen en zo een watermerk van elk denkbaar type te maken.

Het volgende codevoorbeeld voegt een watermerk in een Word document:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

U kunt het sjabloonbestand van dit voorbeeld downloaden van [hier](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Watermerk uit een Document verwijderen

De klasse [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) biedt de methode verwijderen om het watermerk uit een document te verwijderen.

Het volgende codevoorbeeld laat zien hoe u een watermerk uit documenten verwijdert:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

Als de watermerken worden toegevoegd met het [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/) class-object, moet u om het watermerk uit een document te verwijderen alleen de naam van de watermerkshape instellen tijdens het invoegen en vervolgens de watermerkshape verwijderen met een toegewezen naam.

In het volgende codevoorbeeld ziet u hoe u de naam van de watermerkshape instelt en deze uit het document verwijdert:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## Een watermerk toevoegen in tabelcel

Soms moet u een watermerk/afbeelding in de cel van een tabel invoegen en deze buiten de tabel weergeven, U kunt de eigenschap [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/) gebruiken. Deze eigenschap krijgt of stelt een vlag die aangeeft of de vorm wordt weergegeven binnen of buiten een tabel. Merk op dat deze eigenschap alleen werkt wanneer u het document optimaliseert voor Microsoft Word 2010 met de methode [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

Het volgende codevoorbeeld laat zien hoe deze eigenschap te gebruiken:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
