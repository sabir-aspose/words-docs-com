---
title: Low Code
second_title: Aspose.Words voor .NET
articleTitle: Werken met documenten met LowCode API
linktitle: Low Code
type: docs
description: "Vereenvoudig documentverwerkingstaken zoals vergelijken, converteren, splitsen, samenvoegen, zoeken en vervangen, en anderen met behulp van Low Code API. Aspose.Words LowCode API met schone syntaxis, snelle resultaten en minimale coderingsinspanning."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nl/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words voor .NET biedt de [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/) naamruimte, die veelvoorkomende documentverwerkingstaken vereenvoudigt. Deze API is ontworpen voor ontwikkelaars die op hoog niveau bewerkingen willen uitvoeren, zoals documentvergelijking, inhoudsextractie, afbeeldingsconversie en tekstvervanging met minimale inspanning.

De LowCode API is ideaal voor scenario ' s waar snelle implementatie belangrijker is dan fijnkorrelige controle. Laten we eens kijken naar de LowCode mogelijkheden van Aspose.Words voor .NET.

{{% alert color="primary" %}}

Het is belangrijk op te merken dat de LowCode API u niet toestaat om de documentstructuur te wijzigen.

{{% /alert %}}

## Beschikbare functies in LowCode API

De `Aspose.Words.LowCode` naamruimte ondersteunt momenteel:

* **Converting** documenten van de ene indeling naar de andere
* **Comparing** documenten
* **Mail merging**
* **Reporting** gebaseerd op LINQ syntaxis
* **Merging** documenten
* **Search and replace**
* **Digital signing** van documenten
* **Splitting** een document in delen met verschillende criteria
* Een **watermark**toevoegen

{{% alert color="primary" %}}

Houd er rekening mee dat een gedetailleerde beschrijving van elke functie buiten Low Code te vinden is in de sectie Ontwikkelaarshandleiding.

{{% /alert %}}

## Vloeiend en niet-vloeiend API

Aspose.Words voor .NET ondersteunt zowel vloeiend als niet-vloeiend APIs, waardoor ontwikkelaars de stijl kunnen kiezen die het beste past bij hun coderingsvoorkeuren en projectbehoeften. Laten we eens kijken naar enkele voorbeelden om te zien hoe deze twee soorten API verschillen.

{{% alert color="primary" %}}

In de Fluent API kunnen bewerkingen worden geconfigureerd en uitgevoerd via een context (zoals ComparerContext of ReplacerContext). Deze context bevat gemeenschappelijke opties. Het zorgt ervoor dat alle gerelateerde methoden werken met een consistente configuratie, waardoor de API krachtig en eenvoudig te beheren is in complexe scenario ' s.

{{% /alert %}}

### Documenten Vergelijken

Gebruik `LowCode` om twee Word documenten te vergelijken en het resultaat op te slaan.

**niet-vloeiend api voorbeeld:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**vloeiend api voorbeeld:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

U kunt `CompareOptions` ook doorgeven voor een fijn afgestemde vergelijking.

**niet-vloeiend api voorbeeld:**

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

**vloeiend api voorbeeld:**

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

### Document converteren naar afbeeldingen

Gebruik `LowCode` om Word document te converteren naar PDF.

**niet-vloeiend api voorbeeld:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**vloeiend api voorbeeld:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Tekst zoeken en vervangen

Gebruik `LowCode` om snel tekst in het hele document te vervangen.

**niet-vloeiend api voorbeeld:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**vloeiend api voorbeeld:**

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

## Waarom Aspose.Words Low CodeGebruiken

Met de naamruimte **Aspose.Words.LowCode** kunt u snel documentverwerkingstaken op hoog niveau implementeren met een schone, leesbare syntaxis. Het is vooral handig voor ontwikkelaars die snelheid, eenvoud en onderhoudbare code nodig hebben bij het werken met Word documenten.

Om meer geavanceerde opties te verkennen, kunt u LowCode APIs altijd combineren met het volledige Aspose.Words objectmodel. Zie meer Low Code voorbeelden in de [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).