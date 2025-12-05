---
title: Checkboxes, tekstinvoer of afbeeldingen invoegen tijdens Mail Merge
second_title: Aspose.Words voor Java
articleTitle: Checkboxes, tekstinvoer of afbeeldingen invoegen
linktitle: Checkboxes, tekstinvoer of afbeeldingen invoegen
description: "Voeg checkboxes of tekstinvoervelden in tijdens Mail Merge met behulp van Java. Voeg ook afbeeldingen uit een Database toe tijdens Mail Merge in Java."
type: docs
weight: 20
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nl/java/insert-checkboxes-text-input-or-images-mail-merge/
timestamp: 2024-01-27-14-07-04
---

De merge engine neemt een document als invoer, zoekt naar `MERGEFIELD` velden erin en vervangt deze door de gegevens die uit de gegevensbron zijn verkregen. Normaal gesproken worden platte tekst en HTML ingevoegd, maar Aspose.Words gebruikers kunnen ook een document genereren dat meer ongebruikelijke scenario ' s voor Mail Merge velden behandelt.

Met de krachtige Aspose.Words - functionaliteit kunt u het Mail Merge - proces uitbreiden:

- invoegen checkbox es en tekst invoer formuliervelden in het document tijdens een mail merge
- afbeeldingen invoegen vanuit een aangepaste opslag (bestanden, BLOB velden, enz.)

## Checkboxes en tekstinvoer invoegen tijdens Mail Merge

Soms is het nodig om een Mail Merge - bewerking uit te voeren, zodat er geen tekst wordt vervangen in het samenvoegveld, maar een checkbox - of tekstinvoerveld. Hoewel dit niet het meest voorkomende scenario is, is het erg handig voor sommige taken.

De volgende schermafbeelding van een Word document toont een sjabloon met samenvoegvelden:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-1](insert-checkboxes-html-or-images-during-mail-merge_1.jpeg)

Deze screenshot van het Word document hieronder toont het reeds gegenereerde document:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-2](insert-checkboxes-html-or-images-during-mail-merge-2.png)

{{% alert color="primary" %}}

Merk op dat sommige velden zijn vervangen door platte tekst, sommige velden zijn vervangen door checkbox formuliervelden en het veld `Subject` is vervangen door een tekstinvoerveld.

{{% /alert %}}

Het volgende codevoorbeeld laat zien hoe u checkboxes invoegt en tekstvelden invoert in een document tijdens een mail merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-MailMergeFormFields.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-HandleMergeField.java" >}}

## Afbeeldingen invoegen tijdens Mail Merge

Wanneer u een bewerking Mail Merge uitvoert, kunt u afbeeldingen uit de database in het document invoegen met behulp van speciale velden voor Afbeelding Mail Merge. Het veld Afbeelding Mail Merge is een samenvoegveld met de naam afbeelding:MyFieldName.

### Afbeeldingen uit een Database Invoegen

Tijdens een mail merge, wanneer een afbeelding Mail Merge veld wordt aangetroffen in een document, wordt de [FieldMergingCallback](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#getFieldMergingCallback) gebeurtenis gestart. U kunt op deze gebeurtenis reageren om een bestandsnaam, stream of afbeeldingsobject terug te sturen naar de engine Mail Merge, zodat deze in het document kan worden ingevoegd.

Het volgende codevoorbeeld laat zien hoe u afbeeldingen die zijn opgeslagen in een databaseveld BLOB invoegt in een rapport:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageFromBlob.java" >}}

### Afbeeldingseigenschappen instellen tijdens Mail Merge

Tijdens het samenvoegen van een veld voor het samenvoegen van afbeeldingen moet u soms verschillende afbeeldingseigenschappen beheren, zoals [WrapType](https://reference.aspose.com/words/java/com.aspose.words/wraptype/).

Op dit moment kunt u met [ImageFieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/) alleen de eigenschappen breedte of hoogte van de afbeelding instellen. Om dit probleem op te lossen, biedt Aspose.Words De Eigenschap [Shape](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/#getShape), waarmee u volledige controle krijgt over de ingevoegde afbeelding of een andere vorm.

Het volgende codevoorbeeld laat zien hoe u verschillende afbeeldingseigenschappen instelt:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-MailMergeImageField.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-FieldMergingHandler.java" >}}

