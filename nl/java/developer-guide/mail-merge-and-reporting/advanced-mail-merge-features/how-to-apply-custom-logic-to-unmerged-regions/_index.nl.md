---
title: Aangepaste logica toepassen op niet-samengevoegde regio ' s
second_title: Aspose.Words voor Java
articleTitle: Aangepaste logica toepassen op niet-samengevoegde regio ' s
linktitle: Aangepaste logica toepassen op niet-samengevoegde regio ' s
type: docs
description: "Aangepaste logica toepassen op niet-samengevoegde gebieden tijdens een bewerking met Mail Merge met behulp van Java."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nl/java/how-to-apply-custom-logic-to-unmerged-regions/
timestamp: 2024-01-27-14-07-04
---

Er zijn enkele situaties waarin het volledig verwijderen van niet-samengevoegde gebieden uit het document tijdens Mail Merge niet gewenst is of het document er onvolledig uitziet. Dit kan gebeuren wanneer de afwezigheid van invoergegevens aan de gebruiker in de vorm van een bericht moet worden weergegeven in plaats van dat het gebied volledig wordt verwijderd.

Er zijn ook momenten waarop het verwijderen van het ongebruikte gebied op zichzelf niet voldoende is, bijvoorbeeld als het gebied wordt voorafgegaan door een titel of als het gebied in een tabel is opgenomen. Als dit gebied niet wordt gebruikt, blijven de titel en de tabel nog steeds bestaan nadat het gebied is verwijderd, wat er niet op zijn plaats zal uitzien in het document.

Dit artikel biedt een oplossing om handmatig te definiëren hoe ongebruikte gebieden in het document worden behandeld. De basiscode voor deze functionaliteit wordt geleverd en kan eenvoudig worden hergebruikt in een ander project.

De logica die op elk gebied moet worden toegepast, wordt gedefinieerd in een klasse die de interface [IFieldMergingCallback](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/) implementeert. Op dezelfde manier kan een Mail Merge handler worden ingesteld om te bepalen hoe elk veld wordt samengevoegd, deze handler kan worden ingesteld om acties uit te voeren op elk veld in een ongebruikt gebied of op het gebied als geheel. Binnen deze handler kunt u de code instellen om de tekst van een gebied te wijzigen, knooppunten of lege rijen en cellen te verwijderen, enz.

In dit voorbeeld gebruiken we het onderstaande document. Het bevat geneste gebieden en een gebied in een tabel.

![apply-custom-logic-to-unmerged-regions-aspose-words-java](how-to-apply-custom-logic-to-unmerged-regions-1.png)

Als een snelle demonstratie kunnen we een voorbeelddatabase uitvoeren op het voorbeelddocument met de vlag [MailMergeCleanupOptions.REMOVE_UNUSED_REGIONS](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/) ingeschakeld. Deze eigenschap verwijdert automatisch niet-samengevoegde regio ' s uit het document tijdens een mail merge.

De gegevensbron bevat twee records voor het **StoreDetails** - gebied, maar bevat opzettelijk gegevens voor de onderliggende **ContactDetails** - regio ' s voor een van de records. Bovendien heeft het **Suppliers** - Gebied ook geen gegevensrijen. Hierdoor blijven ongebruikte regio ' s in het document staan. Het resultaat na het samenvoegen van het document met deze gegevensbron staat hieronder.

![merged-regions-aspose-words-java](how-to-apply-custom-logic-to-unmerged-regions-2.png)

Zoals aangegeven op de afbeelding kunt u zien dat het **ContactDetails** - gebied voor de tweede record en **Suppliers** - regio ' s automatisch zijn verwijderd door de Mail Merge - engine omdat ze geen gegevens hebben. Er zijn echter een paar problemen waardoor dit uitvoerdocument er onvolledig uitziet:

- Het **ContactDetails** - gebied laat nog steeds een alinea achter met de tekst "contactgegevens".
- In hetzelfde geval is er geen aanwijzing dat er geen telefoonnummers zijn, alleen een lege ruimte die tot verwarring kan leiden.
- De tabel en titel met betrekking tot het **Suppliers** - gebied blijven ook bestaan nadat het gebied in de tabel is verwijderd.

De techniek in dit artikel laat zien hoe u aangepaste logica kunt toepassen op elk niet-samengevoegd gebied om deze problemen te voorkomen.

**Oplossing**

Om logica handmatig toe te passen op elk ongebruikt gebied in het document, maken we gebruik van functies die al beschikbaar zijn in Aspose.Words.

De Mail Merge engine biedt een eigenschap om ongebruikte gebieden te verwijderen via de **MailMergeCleanupOptions.RemoveUnusedRegions** vlag. Dit kan worden uitgeschakeld zodat dergelijke gebieden onaangetast blijven tijdens een mail merge. Dit stelt ons in staat om de niet-samengevoegde regio ' s in het document te laten en ze handmatig zelf te verwerken.

We kunnen dan gebruik maken van de eigenschap **MailMerge.FieldMergingCallback** als een middel om onze eigen aangepaste logica toe te passen op deze niet-gemergde gebieden tijdens Mail Merge door het gebruik van een handlerklasse die de **IFieldMergingCallback** interface implementeert.

Deze code binnen de handler-klasse is de enige klasse die u moet wijzigen om de logica te beheren die wordt toegepast op niet-gemergde regio ' s. De andere code in dit voorbeeld kan zonder wijziging in elk project worden hergebruikt.

Dit voorbeeldproject demonstreert deze techniek. Het gaat om de volgende stappen::

1. Voer Mail Merge uit op het document met behulp van uw gegevensbron. De vlag **MailMergeCleanupOptions.RemoveUnusedRegions** is uitgeschakeld voor nu willen we dat de regio ' s blijven zodat we ze handmatig kunnen afhandelen. Alle regio ' s zonder gegevens worden niet samengevoegd in het document.
1. Roep de methode **ExecuteCustomLogicOnEmptyRegions** aan. Deze methode wordt in deze steekproef verstrekt. Het voert acties uit waarmee de gespecificeerde handler voor elk niet-gemengd gebied kan worden opgeroepen. Deze methode is herbruikbaar en kan ongewijzigd worden gekopieerd naar elk project dat het vereist (samen met alle afhankelijke methoden).Deze methode voert de volgende stappen uit::
   1. Stelt de door de gebruiker opgegeven handler in op de eigenschap **MailMerge.FieldMergingCallback**.
   1. Roept de **CreateDataSourceFromDocumentRegions** methode aan die de **Document** en **ArrayList** bevattende regio ' s van de gebruiker accepteert. Met deze methode wordt een dummy-gegevensbron gemaakt met tabellen voor elk niet-gemengd gebied in het document.
   1. Voert Mail Merge uit op het document met behulp van de dummy-gegevensbron. Wanneer Mail Merge met deze gegevensbron wordt uitgevoerd, kan de door de gebruiker gespecificeerde handler worden opgeroepen voor elk unmerge-gebied en de aangepaste logica worden toegepast

**Code**

De implementatie voor de **ExecuteCustomLogicOnEmptyRegions** methode vindt u hieronder. Deze methode accepteert verschillende parameters:

1. Het [Document](https://reference.aspose.com/words/java/com.aspose.words/document/) - object dat niet-samengevoegde gebieden bevat die door de doorgegeven handler moeten worden behandeld.
1. De handler-klasse die de logica definieert die moet worden toegepast op niet-samengevoegde regio ' s. Deze handler moet de [IFieldMergingCallback](https://www.aspose.com/api/java/words/com.aspose.words/interfaces/IFieldMergingCallback) interface.
1. Door het gebruik van de juiste overbelasting kan de methode ook een derde parameter accepteren – een lijst van regio namen als strings. Als dit is opgegeven, worden alleen de namen van de regio ' s die overblijven van het document dat in de lijst is opgegeven, handmatig verwerkt. Andere gebieden die worden aangetroffen, worden niet door de handler opgeroepen en automatisch verwijderd. Wanneer de overbelasting met slechts twee parameters is gespecificeerd, wordt elk overgebleven gebied in het document opgenomen door de methode die handmatig moet worden verwerkt.

**Bijvoorbeeld**

Toont hoe u aangepaste logica uitvoert op ongebruikte gebieden met behulp van de opgegeven handler.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ExecuteCustomLogicOnUnusedRegions.java" >}}

{{% alert color="primary" %}}

Als u overweegt de methode **ExecuteCustomLogicOnEmptyRegions** achtereenvolgens uit te voeren met verschillende handlers (bijvoorbeeld elke handler past logica toe op bepaalde velden), moet u het verwijderen van ongebruikte regio 's uitschakelen, zodat dergelijke regio' s niet tussen deze aanroepen worden verwijderd.

{{% /alert %}}

**Bijvoorbeeld**

Definieert de methode die wordt gebruikt om niet-samengevoegde regio ' s handmatig te verwerken.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ManuallyHandleUnmergedRegions.java" >}}

Deze methode houdt in dat alle niet-samengevoegde regio ' s in het document worden gevonden. Dit wordt bereikt met behulp van de **MailMerge.GetFieldNames** methode. Deze methode retourneert alle samenvoegvelden in het document, inclusief de markeringen voor het begin en het einde van het gebied (weergegeven door samenvoegvelden met het voorvoegsel *TableStart* of *TableEnd*).

Wanneer een `TableStart` samenvoegveld wordt aangetroffen, wordt dit Toegevoegd als een nieuwe **DataTable** aan de **DataSet**. Aangezien een regio meer dan één keer kan worden weergegeven (bijvoorbeeld omdat het een geneste regio is waar de bovenliggende regio is samengevoegd met meerdere records), wordt de tabel alleen gemaakt en Toegevoegd als deze nog niet bestaat in de **DataSet**.

Wanneer een geschikte regio start is gevonden en toegevoegd aan de database, wordt het volgende veld (dat overeenkomt met het eerste veld in de regio) toegevoegd aan de **DataTable**. Alleen het eerste veld moet worden toegevoegd voor elk veld in het gebied dat moet worden samengevoegd en doorgegeven aan de handler.

We hebben ook de veldwaarde van het eerste veld ingesteld op 'FirstField ' om het gemakkelijker te maken om logica toe te passen op de eerste of andere velden in de regio. Door dit op te nemen betekent dit dat het niet nodig is om de naam van het eerste veld hard te coderen of extra code te implementeren om te controleren of het huidige veld het eerste is in de handlercode.

Onderstaande code laat zien hoe dit systeem werkt. Het document dat aan het begin van dit artikel wordt weergegeven, wordt opnieuw samengevoegd met dezelfde gegevensbron, maar deze keer worden de ongebruikte regio ' s behandeld met aangepaste code.

**Bijvoorbeeld**

Toont hoe niet-samengevoegde gebieden na Mail Merge met door de gebruiker gedefinieerde code moeten worden behandeld.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-HandleUnmergedRegionsAfterMailMerge.java" >}}


De code voert verschillende bewerkingen uit op basis van de naam van de regio die wordt opgehaald met behulp van de eigenschap **FieldMergingArgs.TableName**. Houd er rekening mee dat u, afhankelijk van uw document en regio ' s, de handler kunt coderen om logica uit te voeren die afhankelijk is van elke regio of code die van toepassing is op elk niet-gemengd gebied in het document of een combinatie van beide.

De logica voor het **ContactDetails** - Gebied houdt in dat de tekst van elk veld in het **ContactDetails** - gebied wordt gewijzigd met een passend bericht waarin staat dat er geen gegevens zijn. De namen van elk veld worden binnen de handler gematcht met behulp van de eigenschap **FieldMergingArgs.FieldName**.

Een soortgelijk proces wordt toegepast op het **Suppliers** - gebied met de toevoeging van extra code om de tabel te verwerken die het gebied bevat. De code controleert of het gebied in een tabel is opgenomen (aangezien het mogelijk al is verwijderd). Als dat zo is, wordt de hele tabel uit het document verwijderd, evenals de alinea die eraan voorafgaat, zolang deze is opgemaakt met een kopstijl, bijvoorbeeld "Heading 1".

**Bijvoorbeeld**

Toont hoe u aangepaste logica definieert in een handler die IFieldMergingCallback implementeert en die wordt uitgevoerd voor niet-samengevoegde gebieden in het document.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-EmptyRegionsHandler.java" >}}

Het resultaat van bovenstaande code is hieronder weergegeven. De niet-Samengevoegde velden in het eerste gebied worden vervangen door informatieve tekst en door de tabel en kop te verwijderen, kan het document er compleet uitzien.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-2](how-to-apply-custom-logic-to-unmerged-regions-3.png)


De code die de bovenliggende tabel verwijdert, kan ook worden uitgevoerd op elk ongebruikt gebied in plaats van alleen een specifiek gebied door de controle voor de tabelnaam te verwijderen. Als in dit geval een regio in een tabel niet is samengevoegd met gegevens, worden zowel de regio als de containertabel automatisch verwijderd.

We kunnen verschillende code in de handler invoegen om te bepalen hoe niet-samengevoegde regio ' s worden behandeld. Door de onderstaande code in de handler te gebruiken, wordt de tekst in de eerste alinea van de regio gewijzigd in een nuttig bericht, terwijl alle volgende alinea ' s in de regio worden verwijderd. Deze andere paragrafen worden verwijderd omdat ze in de regio zouden blijven na het samenvoegen van ons bericht.

De vervangende tekst wordt samengevoegd in het eerste veld door de opgegeven tekst in te stellen in de eigenschap **FieldMergingArgs.Text**. De tekst van deze eigenschap wordt door de engine Mail Merge in het veld samengevoegd.

De code past dit alleen toe voor het eerste veld in de regio door de eigenschap **FieldMergingArgs.FieldValue** te controleren. De veldwaarde van het eerste veld in het gebied is gemarkeerd met "FirstField". Dit maakt dit type logica gemakkelijker te implementeren in veel regio ' s, omdat er geen extra code nodig is.

**Bijvoorbeeld**

Hiermee kunt u een ongebruikt gebied vervangen door een bericht en extra alinea ' s verwijderen.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ReplaceAnUnusedRegionWithAMessage.java" >}}

Het resulterende document nadat de bovenstaande code is uitgevoerd, wordt hieronder weergegeven. Het ongebruikte gebied wordt vervangen door een bericht waarin staat dat er geen records moeten worden weergegeven.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-3](how-to-apply-custom-logic-to-unmerged-regions-4.png)


Als een ander voorbeeld kunnen we de onderstaande code invoegen in plaats van de code die oorspronkelijk de **SuppliersRegion** behandelde. Hiermee wordt een bericht in de tabel weergegeven en worden de cellen samengevoegd in plaats van de tabel uit het document te verwijderen. Aangezien het gebied zich in een tabel met meerdere cellen bevindt, lijkt het leuker om de cellen van de tabel samen te voegen en het bericht gecentreerd te hebben.

**Bijvoorbeeld**

Toont hoe u alle bovenliggende cellen van een ongebruikt gebied samenvoegt en een bericht in de tabel weergeeft.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-MergeAllTheParentCellsOfAnUnusedRegion.java" >}}

Het resulterende document nadat de bovenstaande code is uitgevoerd, wordt hieronder weergegeven.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-4](how-to-apply-custom-logic-to-unmerged-regions-5.png)


Ten slotte kunnen we de methode **ExecuteCustomLogicOnEmptyRegions** aanroepen en de tabelnamen specificeren die binnen onze handlermethode moeten worden verwerkt, terwijl we andere specificeren die automatisch moeten worden verwijderd.

**Bijvoorbeeld**

Toont hoe u alleen het `ContactDetails` - gebied opgeeft dat moet worden verwerkt via de klasse handler.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-HandleTheContactDetailsRegion.java" >}}

Het aanroepen van deze overbelasting met de opgegeven ArrayList zal de gegevensbron creëren die alleen gegevensrijen bevat voor de opgegeven regio ' s. Andere regio ' s dan de `ContactDetails` regio worden niet verwerkt en worden in plaats daarvan automatisch verwijderd door de Mail Merge engine. Het resultaat van de bovenstaande oproep met behulp van de code in onze originele handler wordt hieronder weergegeven.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-5](how-to-apply-custom-logic-to-unmerged-regions-6.png)
