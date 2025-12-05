---
title: Low Code
second_title: Aspose.Words pro .NET
articleTitle: Práce s dokumenty pomocí LowCode API
linktitle: Low Code
type: docs
description: "Zjednodušte úkoly zpracování dokumentů, jako je porovnání, převod, rozdělení, sloučení, hledání a nahrazení a další pomocí Low Code API. Aspose.Words LowCode API s čistou syntaxí, rychlými výsledky a minimálním kódovacím úsilím."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cs/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words Pro .NET poskytuje obor názvů [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/), což zjednodušuje běžné úlohy zpracování dokumentů. Tento API je určen pro vývojáře, kteří chtějí provádět operace na vysoké úrovni, jako je porovnávání dokumentů, extrakce obsahu, konverze obrázků a nahrazení textu s minimálním úsilím.

LowCode API je ideální pro scénáře, kde je rychlá implementace důležitější než jemnozrnná kontrola. Podívejme se blíže na schopnosti LowCode Aspose.Words pro .NET.

{{% alert color="primary" %}}

Je důležité si uvědomit, že LowCode API neumožňuje změnit strukturu dokumentu.

{{% /alert %}}

## Dostupné funkce v LowCode API

Obor názvů `Aspose.Words.LowCode` aktuálně podporuje:

* **Converting** dokumenty z jednoho formátu do druhého
* **Comparing** dokumenty
* **Mail merging**
* **Reporting** na základě syntaxe LINQ
* **Merging** dokumenty
* **Search and replace**
* **Digital signing** dokumentů
* **Splitting** dokument na části podle různých kritérií
* Přidání **watermark**

{{% alert color="primary" %}}

Vezměte prosím na vědomí, že podrobný popis každé funkce mimo Low Code najdete v sekci Průvodce pro vývojáře.

{{% /alert %}}

## Plynule a plynule API

Aspose.Words pro .NET podporuje Fluent i non-Fluent APIs, což vývojářům umožňuje zvolit styl, který nejlépe vyhovuje jejich preferencím kódování a potřebám projektu. Podívejme se na několik příkladů, abychom zjistili, jak se tyto dva typy API liší.

{{% alert color="primary" %}}

V aplikaci Fluent API lze operace konfigurovat a provádět prostřednictvím kontextu (například ComparerContext nebo ReplacerContext). Tento kontext obsahuje běžné možnosti. Zajišťuje, že všechny související metody pracují s konzistentní konfigurací, díky čemuž je API výkonný a snadno ovladatelný ve složitých scénářích.

{{% /alert %}}

### Porovnat Dokumenty

Použijte `LowCode` k porovnání dvou dokumentů Word a uložení výsledku.

**příklad non-fluent api:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**příklad fluent api:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

Můžete také předat `CompareOptions` pro vyladěné srovnání.

**příklad non-fluent api:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

CompareOptions options = new CompareOptions
{
    IgnoreFormatting = true,
    IgnoreCaseChanges = true
};

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc, options);
{{< /highlight >}}

**příklad fluent api:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

ComparerContext comparerContext = new ComparerContext();
comparerContext.CompareOptions.IgnoreCaseChanges = true;

Comparer.Create(comparerContext)
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.3.docx")
   .Execute();
{{< /highlight >}}

### Převést dokument na obrázky

Použijte `LowCode` pro převod Word dokumentu na PDF.

**příklad non-fluent api:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**příklad fluent api:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Najít a nahradit Text

Použijte `LowCode` k rychlému nahrazení textu v celém dokumentu.

**příklad non-fluent api:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**příklad fluent api:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";

ReplacerContext replacerContext = new ReplacerContext();
replacerContext.SetReplacement("ReplaceMe", "Replacement");

Replacer.Create(replacerContext)
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

## Proč Používat Aspose.Words Low Code

Obor názvů **Aspose.Words.LowCode** vám pomůže rychle implementovat úkoly zpracování dokumentů na vysoké úrovni s čistou a čitelnou syntaxí. Je zvláště užitečný pro vývojáře, kteří potřebují rychlost, jednoduchost a udržovatelný kód při práci s dokumenty Word.

Chcete-li prozkoumat pokročilejší možnosti, můžete vždy kombinovat LowCode APIs s úplným objektovým modelem Aspose.Words. Podívejte se na další příklady Low Code v [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).