---
title: Mail Merge šablona v Java
second_title: Aspose.Words pro Java
articleTitle: Mail Merge šablona
linktitle: Mail Merge šablona
type: docs
description: "Vytvořte šablonu Mail Merge pro definování pevného obsahu ve výstupních dokumentech a poté Vygenerujte slučovací dokumenty pomocí slučovacích polí v Java."
keywords: "create Mail Merge template Java, Mail Merge Java"
weight: 10
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/java/mail-merge-template/
timestamp: 2024-01-31-14-23-37
---

Je běžné používat šablonu sloučení jako základní dokument pro operaci Mail Merge, pokud se jedná o jednoduchou Mail Merge nebo Mail Merge s oblastmi. Mail merge s regiony je silnější a populárnější než jednoduchý mail merge. Jednoduchý Mail Merge je považován za konkrétní případ Mail Merge s regiony, kde region je celý dokument. Vše je vysvětleno v dalším článku "Typy operací Mail Merge" podrobněji.

Šablona zajišťuje správné formátování textu ve výstupním sloučeném dokumentu a operace Mail Merge zaručuje správné zadání textu ze zdroje dat do šablony sloučení.

Aspose.Words poskytuje možnost Vytvořit šablonu Mail Merge pro definování pevného obsahu a poté generovat slučovací dokumenty pomocí slučovacích polí. Šablona sloučení tedy bude mít potřebný text, který je stejný ve všech výstupních dokumentech, a pole sloučení pro vyplnění měnícího se obsahu. V důsledku toho budou informace ze zadaného zdroje dat přidány do šablony sloučení prostřednictvím těchto polí během generování sloučeného dokumentu.

## Co je Mail Merge šablona

Šablona Mail Merge je personalizovaný dokument, který obsahuje pevná data a sloučená pole, kde má být text proměnné. Šablona sloučení může být v libovolném formátu, který podporuje pole, například, DOC, DOCX, DOT, DOTX, RTF. Kromě toho můžete také použít šablonu mustache, která je podrobněji vysvětlena v článku "syntaxe šablonyMustache".

Šablonu sloučení můžete vytvořit jako model pro nové dokumenty a měla by obsahovat hlavní text, který musí být stejný pro každou verzi sloučeného dokumentu. Přidání slučovacích polí do šablony bude představovat personalizační data, jako jsou jména nebo adresy, které jsou načteny ze zdroje dat. Operace Mail Merge automaticky vloží personalizační data ze zdroje dat do dokumentu šablony sloučení.

Kromě toho můžete do šablony přidat oblast Mail Merge vložením dvou polí Mail Merge pro označení začátku a konce oblasti pošty. Další článek "Typy operací Mail Merge" to vysvětluje podrobněji.

## Vytvořte šablonu Mail Merge

Můžete vytvořit šablonu a přidat do ní konkrétní slučovací pole, která budou nahrazena hodnotami ze zdroje dat buď ručně, například pomocí Microsoft Word, nebo programově pomocí Aspose.Words. V tomto článku se podíváme na programový způsob vytváření šablony.

Pomocí třídy [DocumentBuilder](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/) vytvořte požadovanou šablonu sloučení pomocí Aspose.Words. Do takové šablony můžete zahrnout text, slučovací pole a zalomení řádku pomocí [InsertTextInput](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertTextInput(java.lang.String,int,java.lang.String,java.lang.String,int)), [InsertField](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertField(int,boolean)), a [InsertParagraph](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertParagraph()) metody.

Následující příklad kódu ukazuje, jak vytvořit šablonu Mail Merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeTemplate-CreateMailMergeTemplate.java" >}}

Obrázek níže ukazuje vytvořenou šablonu:

<img src="mail-merge-template-1.png" alt="mail_merge_template_aspose_words_java" style="width:650px"/>

## Přizpůsobení vlastností šablony Mail Merge

Aspose.Words umožňuje přizpůsobit šablonu pomocí mnoha vlastností. Přizpůsobení šablony bude popsáno níže na příkladu přizpůsobení některých vlastností obrázků a textu.

### Přizpůsobte Vlastnosti Obrázku

Vlastnosti obrázku můžete určit pomocí třídy [ImageFieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/). Všimněte si, že můžete vložit obrázek z databáze, jak je popsáno v [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/c693ec7a8957051c206edc69612094a4169f6def/Examples/DocsExamples/Java/src/main/java/DocsExamples/Mail_Merge_And_Reporting/WorkingWithFields.java#L226).

Následující příklad kódu ukazuje, jak zadat název souboru obrázku a velikost obrázku:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-ImageFieldMerging.java" >}}

### Přizpůsobení Vlastností Textu

Můžete použít třídy [Text]https://reference.aspose.com/words/java/com.aspose.words/Fieldmergingargs#Text) property to insert text into the document for the current merge field. Also, you can change the formatting of texts and paragraphs inside your template using [Font](https://reference.aspose.com/words/java/com.aspose.words/font/) a [ParagraphFormat](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/). Text, který se má vložit před nebo za pole sloučení, můžete zpracovat pomocí vlastností [TextBefore](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/#TextBefore) a [TextAfter](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/#TextAfter), které jsou součástí třídy [FieldMergeField](https://reference.aspose.com/words/java/com.aspose.words/fieldmergefield/).

Následující příklad kódu ukazuje, jak vložit zaškrtávací políčka nebo HTML během operace Mail Merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-MailMergeFormFields.java" >}}

{{% alert color="primary" %}}

Ukázkový soubor tohoto příkladu si můžete stáhnout z [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20destinations%20-%20Fax.docx).

Můžete také zkontrolovat implementaci třídy `HandleMergeField` z [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/DocsExamples/Java/src/main/java/DocsExamples/Mail_Merge_And_Reporting/WorkingWithFields.java).

{{% /alert %}}

## Vidět

* Pro více informací o tom, jak vytvořit šablony v Microsoft Word ručně, zkontrolujte prosím [Vytvoření šablony](https://support.microsoft.com/en-us/office/save-a-word-document-as-a-template-cb17846d-ecec-49d4-82ea-a6f5e3e8b9ae) článek v dokumentaci Microsoft
