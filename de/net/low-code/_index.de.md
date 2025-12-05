---
title: Low Code
second_title: Aspose.Words für .NET
articleTitle: Arbeiten mit Dokumenten mit LowCode API
linktitle: Low Code
type: docs
description: "Vereinfachen Sie Dokumentenverarbeitungsaufgaben wie Vergleichen, Konvertieren, Teilen, Zusammenführen, Suchen und Ersetzen und andere mit Low Code API. Aspose.Words LowCode API mit sauberer Syntax, schnellen Ergebnissen und minimalem Programmieraufwand."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /de/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words für .NET stellt den [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/)-Namespace bereit, der allgemeine Dokumentenverarbeitungsaufgaben vereinfacht. Dieses API wurde für Entwickler entwickelt, die Vorgänge auf hoher Ebene wie Dokumentenvergleich, Inhaltsextraktion, Bildkonvertierung und Textersetzung mit minimalem Aufwand ausführen möchten.

LowCode API ist ideal für Szenarien, in denen eine schnelle Implementierung wichtiger ist als eine feinkörnige Kontrolle. Schauen wir uns die LowCode -Fähigkeiten von genauer an Aspose.Words für .NET.

{{% alert color="primary" %}}

Es ist wichtig zu beachten, dass Sie mit LowCode API die Dokumentstruktur nicht ändern können.

{{% /alert %}}

## Verfügbare Funktionen in LowCode API

Der `Aspose.Words.LowCode`-Namespace unterstützt derzeit:

* **Converting** Dokumente von einem Format in ein anderes
* **Comparing** Dokumente
* **Mail merging**
* **Reporting** basiert auf LINQ Syntax
* **Merging** Dokumente
* **Search and replace**
* **Digital signing** von Dokumenten
* **Splitting** ein Dokument in Teile nach verschiedenen Kriterien
* Hinzufügen einer **watermark**

{{% alert color="primary" %}}

Bitte beachten Sie, dass eine detaillierte Beschreibung jeder Funktion außerhalb von Low Code im Abschnitt Entwicklerhandbuch zu finden ist.

{{% /alert %}}

## Fließend und nicht fließend API

Aspose.Words für .NET unterstützt sowohl fließend als auch nicht fließend APIs, sodass Entwickler den Stil auswählen können, der ihren Codierungspräferenzen und Projektanforderungen am besten entspricht. Schauen wir uns einige Beispiele an, um zu sehen, wie sich diese beiden Arten von API unterscheiden.

{{% alert color="primary" %}}

In Fluent API können Operationen über einen Kontext (z. B. ComparerContext oder ReplacerContext) konfiguriert und ausgeführt werden. Dieser Kontext enthält allgemeine Optionen. Es stellt sicher, dass alle zugehörigen Methoden mit einer konsistenten Konfiguration arbeiten, wodurch API in komplexen Szenarien leistungsstark und einfach zu verwalten ist.

{{% /alert %}}

### Dokumente vergleichen

Verwenden Sie `LowCode`, um zwei Word Dokumente zu vergleichen und das Ergebnis zu speichern.

**nicht fließendes API-Beispiel:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**fließendes API-Beispiel:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

Sie können auch `CompareOptions` für einen fein abgestimmten Vergleich übergeben.

**nicht fließendes API-Beispiel:**

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

**fließendes API-Beispiel:**

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

### Dokument in Bilder konvertieren

Verwenden Sie `LowCode`, um das Word-Dokument in PDF zu konvertieren.

**nicht fließendes API-Beispiel:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**fließendes API-Beispiel:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Suchen und Ersetzen von Text

Verwenden Sie `LowCode`, um Text im gesamten Dokument schnell zu ersetzen.

**nicht fließendes API-Beispiel:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**fließendes API-Beispiel:**

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

## Warum Aspose.Words Low Code verwenden

Der Namespace **Aspose.Words.LowCode** hilft Ihnen, Dokumentenverarbeitungsaufgaben auf hoher Ebene schnell mit sauberer, lesbarer Syntax zu implementieren. Es ist besonders nützlich für Entwickler, die Geschwindigkeit, Einfachheit und wartbaren Code benötigen, wenn sie mit Word -Dokumenten arbeiten.

Um erweiterte Optionen zu erkunden, können Sie LowCode APIs immer mit dem vollständigen Aspose.Words Objektmodell kombinieren. Weitere Low Code Beispiele finden Sie in [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).