---
title: Typen Mail Merge - bewerking in Java
second_title: Aspose.Words voor Java
articleTitle: Typen Mail Merge - bewerking
linktitle: Typen Mail Merge - bewerking
type: docs
description: "Voer twee verschillende soorten Mail Merge bewerkingen uit: eenvoudig Mail Merge en Mail Merge Met regio ' s. Simple Mail Merge herhaalt het hele document per gegevensbronrecord, terwijl Mail Merge Met regio 's alleen aangewezen regio' s per record herhaalt met behulp van Java."
keywords: "how to execute Mail Merge java, Mail Merge Java, Simple Mail Merge"
weight: 20
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nl/java/types-of-mail-merge-operations/
timestamp: 2024-01-27-14-07-04
---

Het belangrijkste idee van Mail Merge is om automatisch een document of meerdere documenten te maken op basis van uw sjabloon en gegevens die uit uw gegevensbron zijn opgehaald. Met Aspose.Words kunt u twee verschillende soorten Mail Merge bewerkingen uitvoeren: eenvoudig Mail Merge en Mail Merge met regio ' s.

Het meest voorkomende voorbeeld van het gebruik van simple Mail Merge is wanneer u een document voor verschillende clients wilt verzenden door hun namen aan het begin van het document op te nemen. Hiervoor moet u samenvoegvelden zoals *First Name* en *Last Name* in uw sjabloon maken en deze vervolgens invullen met gegevens uit uw gegevensbron. Terwijl het meest voorkomende voorbeeld van het gebruik van Mail Merge Met regio ' s is wanneer u een document wilt verzenden dat specifieke bestellingen bevat met de lijst van alle items binnen elke bestelling. Om dit te doen, moet u merge – regio ' s maken binnen uw template-eigen regio voor elke bestelling, om deze te vullen met alle vereiste gegevens voor de items.

Het belangrijkste verschil tussen beide samenvoegbewerkingen is dat eenvoudig Mail Merge (zonder regio 's) het hele document per gegevensbronrecord herhaalt, terwijl Mail Merge met regio' s alleen aangewezen regio ' s per record herhaalt. U kunt een eenvoudige Mail Merge - bewerking zien als een specifiek geval van samenvoegen met regio ' s waarbij het enige gebied het hele document is.

{{% alert color="primary" %}}

De [MailMerge](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/) klasse vertegenwoordigt een Mail Merge functionaliteit. Met zijn eigenschappen kunt u het vereiste gedrag aanpassen voordat u een Mail Merge - bewerking uitvoert.

{{% /alert %}}

## Eenvoudige Mail Merge Bewerking {#simple-mail-merge-operation}

Een eenvoudige Mail Merge wordt gebruikt om de Mail Merge velden in uw sjabloon te vullen met de vereiste gegevens uit uw gegevensbron (weergave van één tabel). Dus het is vergelijkbaar met de klassieke Mail Merge in Microsoft Word.

U kunt een of meer samenvoegvelden toevoegen aan uw sjabloon en vervolgens de eenvoudige bewerking Mail Merge uitvoeren. Het wordt aanbevolen om het te gebruiken als uw sjabloon geen samenvoeggebieden bevat.

De belangrijkste beperking van het gebruik van dit type is dat de volledige documentinhoud voor elke record in de gegevensbron wordt herhaald.

### Een eenvoudige Mail Merge - bewerking {#how-to-execute-a-simple-mail-merge-operation}uitvoeren

Zodra uw sjabloon klaar is, kunt u beginnen met het uitvoeren van de eenvoudige Mail Merge - bewerking. Met Aspose.Words kunt u een eenvoudige Mail Merge - bewerking uitvoeren met verschillende [Execute methods](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#execute-com.aspose.words.IMailMergeDataSource) die verschillende gegevensobjecten als gegevensbron accepteren.

Het volgende codevoorbeeld laat zien hoe u een eenvoudige Mail Merge - bewerking uitvoert met behulp van een van de [Execute](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#execute-java.lang.String---java.lang.Object) - methode:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e"  "Examples-src-main-java-com-aspose-words-examples-mail_merge-TypesofMailMergeOperations-ExecuteSimpleMailMerge.java" >}}

U kunt het verschil tussen het document opmerken voordat u simple mail mergeuitvoert:

<img src="execute-simple-mail-merge-1.png" alt="simple_mail_merge_template_aspose_words_java" style="width:300px"/>

En na het uitvoeren van simple mail merge:

<img src="execute-simple-mail-merge-2.png" alt="execute_simple_mail_merge_aspose_words_java" style="width:300px"/>

### Hoe meerdere samengevoegde documenten te maken

In Aspose.Words vult de standaard Mail Merge - bewerking slechts één document met inhoud uit uw gegevensbron. U moet de bewerking Mail Merge dus meerdere keren uitvoeren om meerdere samengevoegde documenten als uitvoer te maken.

Het volgende codevoorbeeld laat zien hoe u meerdere samengevoegde documenten kunt genereren tijdens een bewerking van Mail Merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e"  "Examples-src-main-java-com-aspose-words-examples-mail_merge-ProduceMultipleDocumentsDuringMailMerge-ProduceMultipleDocumentsDuringMailMerge.java" >}}

{{% alert color="primary" %}}

U kunt het voorbeeldbestand van dit voorbeeld downloaden van [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/tree/master/Examples/src/main/resources/MailMerge).

{{% /alert %}}

## Mail Merge Met regio ' s

U kunt verschillende regio ' s in uw sjabloon maken om speciale gebieden te hebben die u eenvoudig met uw gegevens kunt vullen. Gebruik Mail Merge Met regio 's als u tabellen, rijen met herhalende gegevens wilt invoegen om uw documenten dynamisch te laten groeien door deze regio' s in uw sjabloon op te geven.

U kunt geneste (kind) regio 's maken en regio' s samenvoegen. Het belangrijkste voordeel van het gebruik van dit type is om delen in een document dynamisch te vergroten. Zie meer details in het volgende artikel "geneste Mail Merge Met regio 's".

{{% alert color="primary" %}}

Informatie over een Mail Merge Regio kan worden verkregen met behulp van de [MailMergeRegionInfo](https://reference.aspose.com/words/java/com.aspose.words/mailmergeregioninfo/) Klasse.

{{% /alert %}}

### Mail Merge uitvoeren met regio ' s

Een Mail Merge regio is een specifiek deel in een document dat een begin-en eindpunt heeft. Beide punten worden weergegeven als Mail Merge velden met specifieke namen *"TableStart:XXX"* en *"TableEnd:XXX"*. Alle inhoud die is opgenomen in een Mail Merge - regio wordt automatisch herhaald voor elke record in de gegevensbron.

Met Aspose.Words kunt u Mail Merge uitvoeren met regio ' s met verschillende [Execute methods](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/executewithregions/#executewithregions/) die verschillende gegevensobjecten als gegevensbron accepteren.

Als eerste stap moeten we de `DataSet` maken om deze later als invoerparameter door te geven aan de `ExecuteWithRegions` methode:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e"  "Examples-src-main-java-com-aspose-words-examples-mail_merge-TypesofMailMergeOperations-CreateDataSet.java" >}}

Het volgende codevoorbeeld laat zien hoe Mail Merge met regio ' s uitgevoerd moet worden met behulp van de [ExecuteWithRegions(DataSet)](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#executeWithRegions-com.aspose.words.net.System.Data.DataSet) methode:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e"  "Examples-src-main-java-com-aspose-words-examples-mail_merge-TypesofMailMergeOperations-MailMergeWithRegions.java" >}}

U kunt het verschil tussen het document opmerken voordat u Mail Merge uitvoert met regio ' s:

<img src="execute-mail-merge-with-regions-1.png" alt="mail_merge_with_regions_template_aspose_words_java" style="width:850px"/>

En na het uitvoeren van Mail Merge Met regio ' s:

<img src="execute-mail-merge-with-regions-2.png" alt="mail_merge_with_regions_execute_aspose_words_java" style="width:850px"/>

### Beperkingen van Mail Merge Met regio ' s

Er zijn enkele belangrijke punten waar u rekening mee moet houden bij het uitvoeren van een Mail Merge Met regio ' s:

* Het beginpunt *TableStart:Orders* en het eindpunt *TableEnd:Orders* moeten beide in dezelfde rij of cel staan. Als u bijvoorbeeld een samenvoeggebied start in een cel van een tabel, moet u het samenvoeggebied beëindigen in dezelfde rij als de eerste cel.
* De naam van het veld samenvoegen moet overeenkomen met de naam van de kolom in uw DataTable. Tenzij u toegewezen velden hebt opgegeven, zal de Mail Merge Met regio ' s niet succesvol zijn voor een samenvoegveld met een andere naam dan de naam van de kolom.

Als een van deze regels wordt overtreden, krijg je onverwachte resultaten of kan er een uitzondering worden gegooid.

{{% alert color="primary" %}}

Als u geen Mail Merge - regio ' s gebruikt, is deze vergelijkbaar met Microsoft Word mail merge en wordt de hele documentinhoud herhaald voor elke record in de gegevensbron.

{{% /alert %}}

