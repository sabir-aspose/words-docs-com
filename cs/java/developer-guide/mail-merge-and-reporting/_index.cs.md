---
title: Mail Merge a hlášení v Java
second_title: Aspose.Words pro Java
articleTitle: Mail Merge a podávání zpráv
linktitle: Mail Merge a podávání zpráv
type: docs
description: "Mail Merge je oblíbená funkce pro rychlé vytváření dokumentů. Aspose.Words pro Java vezme standardní funkci Mail Merge a posune ji o mnoho kroků dopředu a promění ji v plnohodnotné řešení pro podávání zpráv, které vám umožní vytvářet ještě složitější dokumenty, jako jsou zprávy, katalogy, zásoby a faktury."
keywords: "how to use Mail Merge Java"
weight: 40
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cs/java/mail-merge-and-reporting/
timestamp: 2024-01-27-14-07-04
---

Mail Merge je populární funkce pro rychlé a snadné vytváření dokumentů, jako jsou dopisy, štítky a obálky. Aspose.Words umožňuje generovat dokumenty ze šablon s Mail Merge poli.

Pole Mail Merge je pole, které můžete vložit do šablony mail merge a zahrnout do výstupních dokumentů konkrétní hodnoty ze záznamu zdroje dat. Můžete například vložit pole sloučení do šablony e-mailu, aby pozdrav měl spíše křestní jméno příjemce než obecné "Ahoj!". Aspose.Words umístí data z externího zdroje, jako je databáze nebo soubor, do těchto polí a naformátuje je. Výsledný dokument se uloží do zadané složky.

Aspose.Words využívá standardní funkci Mail Merge a posouvá ji o mnoho kroků dopředu, čímž se stává plnohodnotným řešením pro podávání zpráv, které vám umožní vytvářet ještě složitější dokumenty, jako jsou zprávy, katalogy, zásoby a faktury. Zde je několik výhod řešení pro podávání zpráv Aspose.Words:

- Návrh sestav v Microsoft Word pomocí standardních polí Mail Merge
- Definujte oblasti v dokumentu, které rostou, například podrobné řádky pořadí
- Vkládání obrázků během mail merge
- Spusťte libovolnou vlastní logiku, Ovládejte formátování nebo vkládejte složitý obsah pomocí obslužných rutin událostí Mail Merge
- Vyplňte dokumenty daty z jakéhokoli typu zdroje dat

## Mechanismus a hlavní složky Mail Merge {#mechanism-and-main-components-of-a-mail-merge-operation}

Aspose.Words poskytuje možnost načítat dokumenty v různých [supported formats](https://reference.aspose.com/words/java/com.aspose.words/loadformat/) a poté umožňuje uživatelům provádět operaci Mail Merge.

Načtený dokument obvykle umožňuje ukládat slučovací pole, například dokument ve formátu DOCX. Existují však formáty, které taková pole neukládají, například TXT. Pokud Aspose.Words podporuje načítání takových formátů souborů, můžete přidat slučovací pole přímo do modelu dokumentu, uložit dokument pohodlným [supported format](https://reference.aspose.com/words/java/com.aspose.words/saveformat/) a provést operaci Mail Merge.

Operace Mail Merge sloučí vaše *mail merge template* a vaše *data source* a vygeneruje jednotlivé *merged documents*.

## Co je Mail Merge šablona {#what-is-a-mail-merge-template}

Cílem použití operace mail merge pomocí šablony sloučení je zjednodušit proces vytváření dokumentu.

Existuje několik způsobů, jak vytvořit a navrhnout šablonu sloučení. Můžete použít Microsoft Word a šablona sloučení nemusí být šablonou Microsoft Word, to je dokument ve formátu DOT nebo DOTX, může to být běžný dokument ve formátu DOC nebo DOCX. Do této šablony musíte vložit některá speciální pole s názvem sloučit pole na místech, kam chcete později vložit data ze zdroje dat. Nebo můžete programově vytvořit šablonu sloučení pomocí třídy [DocumentBuilder](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/).

Šablona sloučení obsahuje hlavní text, který by měl být stejný ve všech výstupních dokumentech po provedení operace Mail Merge. Pro šablonu můžete použít libovolný formát, pokud do ní můžete přidat slučovací pole. Všechna pole sloučení ve vaší šabloně budou vyplněna ze zdroje dat během operace Mail Merge.

## Zdroje dat pro operaci Mail Merge {#data-source-types-for-a-mail-merge-operation}

Aspose.Words Mail Merge přijímá různé zdroje dat. To může být buď DataTable, DataView, DataSet, IDataReader, pole hodnot podporované ADO .NET nebo vlastní zdroje dat reprezentované implementacemi [IMailMergeDataSource](https://reference.aspose.com/words/java/com.aspose.words/imailmergedatasource/).

Zdroj dat obsahuje všechny informace, které jsou vytaženy během operace Mail Merge za účelem přizpůsobení jednotlivých e-mailů a dokumentů. Zdroje dat lze vytvářet ručně nebo generovat reportováním z existující databáze nebo aplikace. Pokud máte data ve formátu XML, můžete je načíst a sloučit s DataSet. Operace Mail Merge projde všechny záznamy zdroje dat a vloží je do polí Mail Merge v dokumentu. Můžete implementovat některá rozhraní mail merge, například [IMailMergeDataSourceRoot](https://reference.aspose.com/words/java/com.aspose.words/imailmergedatasourceroot/), a sloučit data z jakéhokoli zdroje dat, včetně dotazu LINQ, souboru XML nebo obchodních objektů.

Následující příklad kódu ukazuje, jak načíst datovou tabulku jako zdroj dat pro operaci Mail Merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ExecuteMailMergeWithRegions-ExecuteMailMergeWithRegions.java" >}}

{{% alert color="primary" %}}

Ukázkový soubor tohoto příkladu si můžete stáhnout z [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20destinations%20-%20Orders.docx).

{{% /alert %}}

## Sloučené dokumenty operace Mail Merge {#merged-documents-of-a-mail-merge-operation}

Sloučený dokument je výsledkem operace Mail Merge při sloučení šablony se zdrojem dat. Všechna slučovací pole ve sloučeném dokumentu jsou nahrazena skutečnými daty ze zdroje dat.

Následující obrázek ukazuje příklad šablony sloučení se sloučenými poli před provedením operace Mail Merge.

![mail-merge-and-reporting-aspose-words-java-1](mail-merge-and-reporting-1.jpg)

Následující obrázek ukazuje příklad výstupního sloučeného dokumentu v důsledku provedení operace Mail Merge.

![mail-merge-and-reporting-aspose-words-java-2](mail-merge-and-reporting-2.jpg)

## Vidět

- [Práce s Mail Merge šablonami v Word](https://docs.microsoft.com/en-us/power-platform/admin/work-mail-merge-templates)
