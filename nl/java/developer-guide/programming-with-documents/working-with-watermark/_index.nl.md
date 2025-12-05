---
title: Werken met watermerk in Java
second_title: Aspose.Words voor Java
articleTitle: Werken met Watermark
linktitle: Werken met Watermark
type: docs
description: "Document watermerk manipulatie met behulp van Java."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nl/java/working-with-watermark/
timestamp: 2025-04-22-08-07-04
---

In dit onderwerp wordt besproken hoe je programmatisch kunt werken met een watermerk met behulp van Aspose.Words. Een watermerk is een achtergrondafbeelding die achter de tekst in een document wordt weergegeven. Een watermerk kan een tekst of een afbeelding bevatten die wordt weergegeven door de klasse [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/).

{{% alert color="primary" %}}

**Online proberen**

U kunt deze functionaliteit proberen met onze [Gratis online document watermerk](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Een watermerk aan een Document toevoegen

In Microsoft Word kan een watermerk eenvoudig in een document worden ingevoegd met de opdracht watermerk invoegen. Aspose.Words biedt de [watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) klasse voor het toevoegen of verwijderen van watermerken in documenten. Aspose.Words geeft de [WatermarkType ](https://reference.aspose.com/words/java/com.aspose.words/watermarktype/)opsomming die drie mogelijke typen watermerken definieert (tekst, afbeelding en geen) om mee te werken.

### Tekst Watermerk Toevoegen

Het volgende codevoorbeeld laat zien hoe u een tekstwatermerk invoegt in een document door [TextWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/textwatermarkoptions/) te definiëren met de methode [SetText](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setText-java.lang.String):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddTextWatermarkWithSpecificOptions.java" >}}

### Afbeelding Toevoegen Watermerk

Het volgende codevoorbeeld laat zien hoe u een watermerk voor een afbeelding invoegt in een document door [ImageWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/imagewatermarkoptions/) te definiëren met de methode [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.awt.image.BufferedImage):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddImageWatermarkWithSpecificOptions.java" >}}

Beeldwatermerk kan worden ingevoegd als afbeelding, tekenreeks of stream.

Het watermerk kan ook worden ingevoegd met behulp van de vormklasse. Het is heel eenvoudig om elke vorm of afbeelding in een kop-of voettekst in te voegen en zo een watermerk van elk denkbaar type te maken.

Het volgende codevoorbeeld voegt een watermerk in een Word document:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-AddWatermarkToADocument-AddWatermarkToADocument.java" >}}

{{% alert color="primary" %}}

U kunt het voorbeeldbestand van dit voorbeeld downloaden van [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Document.doc).

{{% /alert %}}


## Watermerk uit een Document verwijderen

De klasse [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) biedt de methode `Remove` om het watermerk uit een document te verwijderen.

De volgende codevoorbeelden laten zien hoe u een watermerk uit documenten verwijdert:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-RemoveWatermarkFromDocument.java" >}}

Als u het watermerk uit een document wilt verwijderen, moet u tijdens het invoegen alleen de naam van de vorm van het watermerk instellen en vervolgens de vorm van het watermerk verwijderen met een toegewezen naam.

In het volgende codevoorbeeld ziet u hoe u de naam van de watermerkshape instelt en deze uit het document verwijdert:

{{< highlight csharp >}}

// Set name to be able to remove it afterwards
watermark.Name("WaterMark");
{{< /highlight >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-RemoveWatermark-RemoveWatermark.java" >}}

## Een watermerk toevoegen aan een tabelcel

Soms moet u een watermerk/afbeelding in de cel van een tabel invoegen en deze buiten de tabel weergeven, U kunt de eigenschap [IsLayoutInCell](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#isLayoutInCell-boolean) gebruiken. Deze eigenschap krijgt of stelt een vlag die aangeeft of de vorm wordt weergegeven binnen of buiten een tabel. Merk op dat deze eigenschap alleen werkt wanneer u het document optimaliseert voor Microsoft Word 2010 met de methode [OptimizeFor](https://reference.aspose.com/words/java/com.aspose.words/compatibilityoptions/#optimizeFor-int).

Het volgende codevoorbeeld laat zien hoe deze eigenschap te gebruiken:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-Shapes-WorkingWithShapes-SetShapeLayoutInCell.java" >}}
