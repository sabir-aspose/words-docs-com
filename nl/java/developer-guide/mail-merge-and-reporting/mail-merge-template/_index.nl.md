---
title: Mail Merge sjabloon in Java
second_title: Aspose.Words voor Java
articleTitle: Mail Merge sjabloon
linktitle: Mail Merge sjabloon
type: docs
description: "Maak een Mail Merge - sjabloon om vaste inhoud in uitvoerdocumenten te definiëren en genereer vervolgens samenvoegdocumenten met behulp van de samenvoegvelden in Java."
keywords: "create Mail Merge template Java, Mail Merge Java"
weight: 10
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nl/java/mail-merge-template/
timestamp: 2024-01-31-14-23-37
---

Het is gebruikelijk om een samenvoegsjabloon te gebruiken als basisdocument voor een Mail Merge - bewerking, hetzij als het een eenvoudige Mail Merge of Mail Merge Met regio ' s is. Mail merge met regio ' s is krachtiger en populairder dan de eenvoudige mail merge. Een eenvoudige Mail Merge wordt beschouwd als een specifiek geval van Mail Merge Met regio ' s waar de regio het hele document is. Alles wordt uitgelegd in het volgende artikel "typen van Mail Merge - bewerking" in meer detail.

De sjabloon zorgt ervoor dat de tekst in het samengevoegde document correct is opgemaakt en de bewerking Mail Merge garandeert dat de tekst uit de gegevensbron correct is ingevoerd in de samenvoegsjabloon.

Aspose.Words biedt de mogelijkheid om een Mail Merge - sjabloon te maken om vaste inhoud te definiëren en vervolgens samenvoegdocumenten te genereren met behulp van de samenvoegvelden. De samenvoegsjabloon heeft dus de nodige tekst, die hetzelfde is in alle uitvoerdocumenten, en de samenvoegvelden om de veranderende inhoud in te vullen. Als gevolg hiervan wordt informatie uit de opgegeven gegevensbron via deze velden toegevoegd aan de samenvoegsjabloon tijdens het genereren van het samengevoegde document.

## Wat is een Mail Merge Template

Een Mail Merge - sjabloon is een gepersonaliseerd document dat de vaste gegevens en de samengevoegde velden bevat waar u de variabele tekst wilt hebben. Een samenvoegsjabloon kan in elke indeling zijn die velden ondersteunt, bijvoorbeeld, DOC, DOCX, DOT, DOTX, RTF. Daarnaast kunt u ook de mustache sjabloon gebruiken die in het artikel "Mustache Sjabloonsyntaxis" in meer detail wordt uitgelegd.

U kunt een samenvoegsjabloon maken als model voor nieuwe documenten en deze moet de hoofdtekst bevatten die voor elke versie van het samengevoegde document hetzelfde moet zijn. Het toevoegen van samenvoegvelden in de sjabloon vertegenwoordigt de personalisatiegegevens, zoals namen of adressen die worden opgehaald uit een gegevensbron. Met een bewerking Mail Merge worden de personalisatiegegevens uit uw gegevensbron automatisch ingevoegd in uw samenvoegsjabloondocument.

Bovendien kunt u een Mail Merge - regio toevoegen aan uw sjabloon door twee Mail Merge - velden in te voegen om het begin en het einde van het e-mailgebied te markeren. Het volgende artikel "typen van Mail Merge - bewerking" legt dat in meer detail uit.

## Een Mail Merge sjabloon maken

U kunt een sjabloon maken en er specifieke samenvoegvelden aan toevoegen, die worden vervangen door de waarden uit de gegevensbron, handmatig, bijvoorbeeld met behulp van Microsoft Word, of programmatisch met behulp van Aspose.Words. In dit artikel zullen we kijken naar de programmatische manier van het maken van een sjabloon.

Gebruik de klasse [DocumentBuilder](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/) om de vereiste samenvoegsjabloon te maken met behulp van Aspose.Words. U kunt een tekst, een samenvoegveld en een regeleinde in zo ' n sjabloon opnemen met behulp van de [InsertTextInput](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertTextInput(java.lang.String,int,java.lang.String,java.lang.String,int)), [InsertField](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertField(int,boolean)), en [InsertParagraph](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertParagraph()) methoden.

Het volgende codevoorbeeld laat zien hoe u een Mail Merge sjabloon maakt:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeTemplate-CreateMailMergeTemplate.java" >}}

De afbeelding hieronder toont de gemaakte sjabloon:

<img src="mail-merge-template-1.png" alt="mail_merge_template_aspose_words_java" style="width:650px"/>

## Eigenschappen van een Mail Merge - sjabloon aanpassen

Met Aspose.Words kunt u uw sjabloon aanpassen via vele eigenschappen. Template aanpassing zal hieronder worden beschreven door middel van een voorbeeld van het aanpassen van sommige eigenschappen van afbeeldingen en tekst.

### Afbeeldingseigenschappen Aanpassen

U kunt de eigenschappen van de afbeelding opgeven met de klasse [ImageFieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/). Merk op dat u een afbeelding uit een database kunt invoegen zoals beschreven in [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/c693ec7a8957051c206edc69612094a4169f6def/Examples/DocsExamples/Java/src/main/java/DocsExamples/Mail_Merge_And_Reporting/WorkingWithFields.java#L226).

Het volgende codevoorbeeld laat zien hoe u de naam en de grootte van het afbeeldingsbestand kunt opgeven:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-ImageFieldMerging.java" >}}

### Teksteigenschappen Aanpassen

U kunt de klassen [Text]https://reference.aspose.com/words/java/com.aspose.words/Fieldmergingargs#Text) property to insert text into the document for the current merge field. Also, you can change the formatting of texts and paragraphs inside your template using [Font](https://reference.aspose.com/words/java/com.aspose.words/font/) en [ParagraphFormat](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/) gebruiken. U kunt de tekst die voor of na het samenvoegveld moet worden ingevoegd, verwerken met behulp van de eigenschappen [TextBefore](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/#TextBefore) en [TextAfter](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/#TextAfter) die zijn opgenomen in de klasse [FieldMergeField](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/).

Het volgende codevoorbeeld laat zien hoe u selectievakjes of HTML invoegt tijdens Mail Merge - bewerking:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-MailMergeFormFields.java" >}}

{{% alert color="primary" %}}

U kunt het voorbeeldbestand van dit voorbeeld downloaden van [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20destinations%20-%20Fax.docx).

U kunt ook de implementatie van de `HandleMergeField` klasse controleren van [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/DocsExamples/Java/src/main/java/DocsExamples/Mail_Merge_And_Reporting/WorkingWithFields.java).

{{% /alert %}}

## Zie Ook

* Voor meer informatie over het handmatig maken van sjablonen in Microsoft Word, raadpleegt u de [Een sjabloon maken](https://support.microsoft.com/en-us/office/save-a-word-document-as-a-template-cb17846d-ecec-49d4-82ea-a6f5e3e8b9ae) artikel in de Microsoft documentatie
