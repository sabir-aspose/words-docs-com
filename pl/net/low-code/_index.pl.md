---
title: Low Code
second_title: Aspose.Words dla .NET
articleTitle: Praca z dokumentami przy użyciu LowCode API
linktitle: Low Code
type: docs
description: "Uprość zadania przetwarzania dokumentów, takie jak porównywanie, konwertowanie, dzielenie, scalanie, znajdowanie i zastępowanie oraz inne przy użyciu Low Code API. Aspose.Words LowCode API z czystą składnią, szybkimi wynikami i minimalnym wysiłkiem kodowania."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pl/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words dla .NET zapewnia przestrzeń nazw [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/), która upraszcza typowe zadania przetwarzania dokumentów. Ten API jest przeznaczony dla programistów, którzy chcą wykonywać operacje na wysokim poziomie, takie jak porównywanie dokumentów, ekstrakcja treści, Konwersja obrazu i zastępowanie tekstu przy minimalnym wysiłku.

LowCode API jest idealny do scenariuszy, w których szybka implementacja jest ważniejsza niż kontrola drobnoziarnista. Przyjrzyjmy się bliżej możliwościom LowCode Aspose.Words dla .NET.

{{% alert color="primary" %}}

Ważne jest, aby pamiętać, że LowCode API nie pozwala na zmianę struktury dokumentu.

{{% /alert %}}

## Dostępne funkcje w LowCode API

Przestrzeń nazw `Aspose.Words.LowCode` obsługuje obecnie:

* **Converting** dokumenty z jednego formatu do drugiego
* **Comparing** dokumenty
* **Mail merging**
* **Reporting** Na podstawie składni LINQ
* **Merging** dokumenty
* **Search and replace**
* **Digital signing** dokumentów
* **Splitting** dokument podzielony na części według różnych kryteriów
* Dodawanie **watermark**

{{% alert color="primary" %}}

Należy pamiętać, że szczegółowy opis każdej funkcji poza Low Code można znaleźć w sekcji Przewodnik dla programistów.

{{% /alert %}}

## Biegły i nie biegły API

Aspose.Words dla .NET obsługuje zarówno Fluent, jak i Non-Fluent APIs, umożliwiając programistom wybór stylu, który najlepiej pasuje do ich preferencji kodowania i potrzeb projektu. Spójrzmy na kilka przykładów, aby zobaczyć, jak te dwa typy API różnią się.

{{% alert color="primary" %}}

W Fluent API operacje można konfigurować i wykonywać za pomocą kontekstu (takiego jak ComparerContext LUB ReplacerContext). Ten kontekst zawiera typowe opcje. Zapewnia, że wszystkie powiązane metody działają w spójnej konfiguracji, dzięki czemu API jest wydajny i łatwy w zarządzaniu w złożonych scenariuszach.

{{% /alert %}}

### Porównaj Dokumenty

Użyj `LowCode`, aby porównać dwa dokumenty Word i zapisać wynik.

**non-fluent api przykład:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**fluent api przykład:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

Możesz także przekazać `CompareOptions` do precyzyjnego porównania.

**non-fluent api przykład:**

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

**fluent api przykład:**

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

### Konwertuj dokument na obrazy

Użyj `LowCode`, aby przekonwertować dokument Word na PDF.

**non-fluent api przykład:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**fluent api przykład:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Znajdź i zamień tekst

Użyj `LowCode`, aby szybko zastąpić tekst w całym dokumencie.

**non-fluent api przykład:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**fluent api przykład:**

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

## Dlaczego Warto Używać Aspose.Words Low Code

Przestrzeń nazw **Aspose.Words.LowCode** pomaga szybko wdrażać zadania przetwarzania dokumentów wysokiego poziomu dzięki czystej, czytelnej składni. Jest to szczególnie przydatne dla programistów, którzy potrzebują szybkości, prostoty i łatwego w utrzymaniu kodu podczas pracy z dokumentami Word.

Aby poznać bardziej zaawansowane opcje, zawsze możesz połączyć LowCode APIs z pełnym modelem obiektowym Aspose.Words. Zobacz więcej przykładów Low Code w [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).