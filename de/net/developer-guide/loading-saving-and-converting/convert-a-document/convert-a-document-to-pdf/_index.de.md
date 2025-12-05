---
title: Word zu PDF konvertieren in C#
second_title: Aspose.Words für .NET
articleTitle: Dokument zu PDF umwandeln
linktitle: Dokument zu PDF umwandeln
description: "Word zu PDF konvertieren in C#. Einfache Codebeispiele für DOCX zu PDF Konvertierung. Unterstützt alle Word-Formate und Bilder."
type: docs
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /de/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Die Möglichkeit, Dokumente einfach und zuverlässig von einem Format in ein anderes zu konvertieren, ist ein Hauptmerkmal von Aspose.Words. PDF ist eines der beliebtesten Formate für die Umwandlung – es ist ein Format mit festem Layout, das das ursprüngliche Erscheinungsbild eines Dokuments beim Rendern auf verschiedenen Plattformen beibehält. Der Begriff "Rendern" wird in Aspose.Words verwendet, um den Prozess der Konvertierung eines Dokuments in ein Dateiformat zu beschreiben, das paginiert ist oder das Konzept von Seiten hat.

## Word-Dokument zu PDF konvertieren

Die Konvertierung von Word zu PDF ist ein ziemlich komplexer Prozess, der mehrere Berechnungsstufen erfordert. Die Layout-Engine von Aspose.Words imitiert die Funktionsweise der Seiten-Layout-Engine von Microsoft Word, wodurch PDF-Ausgabedokumente so nah wie möglich an dem aussehen, was Sie in Microsoft Word sehen können.

Mit Aspose.Words können Sie ein Dokument programmgesteuert von Word-Formaten wie DOC oder DOCX zu PDF umwandeln, ohne Microsoft Office zu verwenden. Dieser Artikel erklärt, wie Sie diese Umwandlung durchführen.

{{% alert color="primary" %}}

Beachten Sie, dass die Anzahl der Seiten in einem Dokument die Konvertierungszeit beeinflusst.

{{% /alert %}}

### DOCX oder DOC zu PDF konvertieren

Das Umwandeln vom DOC- oder DOCX-Dokumentformat in das PDF-Format in Aspose.Words ist sehr einfach und kann mit nur zwei Codezeilen erreicht werden, die:

1. Laden Sie Ihr Dokument in ein [Document](https://reference.aspose.com/words/net/aspose.words/document/)-Objekt mit einem seiner Konstruktoren, indem Sie den Dokumentnamen mit seiner Formaterweiterung angeben.
1. Rufen Sie eine der [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/)-Methoden für das **Document**-Objekt auf und geben Sie das gewünschte Ausgabeformat als PDF an, indem Sie einen Dateinamen mit der Erweiterung ".PDF" eingeben.

Das folgende Codebeispiel zeigt, wie Sie ein Dokument von DOCX zu PDF mit der [Save](https://reference.aspose.com/words/net/aspose.words/document/save/)-Methode konvertieren:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Sie können die Vorlagendatei dieses Beispiels von [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx) herunterladen.

{{% alert color="primary" %}}

Manchmal ist es notwendig, zusätzliche Optionen anzugeben, die das Ergebnis des Speicherns eines Dokuments als PDF beeinflussen können. Diese Optionen können mit der [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)-Klasse angegeben werden, die Eigenschaften enthält, die bestimmen, wie die PDF-Ausgabe angezeigt wird.

Beachten Sie, dass Sie mit derselben Technik jedes Dokument im Fließtext-Format in das PDF-Format überführen können.

{{% /alert %}}

### Zu verschiedenen PDF-Standards konvertieren

Aspose.Words bietet die [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/)-Aufzählung zur Unterstützung der Umwandlung von DOC oder DOCX in verschiedene PDF-Formatstandards (wie PDF 1.7, PDF 1.5 usw.).

Das folgende Codebeispiel zeigt, wie Sie ein Dokument zu PDF 1.7 mit [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) mit Konformität zu PDF17 umwandeln:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Bilder zu PDF konvertieren

Die Konvertierung zu PDF ist nicht auf Microsoft Word-Dokumentformate beschränkt. Jedes von Aspose.Words unterstützte Format, einschließlich programmgesteuert erstellter, kann auch zu PDF gewandelt werden. Zum Beispiel können wir einseitige Bilder wie JPEG, PNG, BMP, EMF oder WMF sowie mehrseitige Bilder wie TIFF und GIF zu PDF umwandeln.

Das folgende Codebeispiel zeigt, wie JPEG- und TIFF-Bilder zu PDF konvertiert werden:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Damit dieser Code funktioniert, müssen Sie Verweise auf Aspose.Words und `System.Drawing` zu Ihrem Projekt hinzufügen.

## PDF-Ausgabegröße reduzieren

Beim Speichern als PDF können Sie angeben, ob Sie die Ausgabe optimieren möchten. Dazu müssen Sie das [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/)-Flag auf true setzen, und dann werden redundante verschachtelte und leere Leinwände entfernt, benachbarte Glyphen mit derselben Formatierung werden verkettet.

Das folgende Codebeispiel zeigt, wie die Ausgabe optimiert wird:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Die Verwendung der **OptimizeOutput**-Eigenschaft kann die Genauigkeit der Inhaltsanzeige beeinträchtigen.

{{% /alert %}}

## Siehe auch

- Der Artikel [Rendern](/words/de/net/rendering/) für weitere Informationen über die Formate mit fester Seite und Fließtext-Layout
- Der Artikel [Umwandlung in festes Seitenformat](/words/de/net/converting-to-fixed-page-format/#what-is-a-page-layout) für weitere Informationen über das Seitenlayout
- Der Artikel [Rendering-Optionen beim Konvertieren zu PDF angeben](/words/de/net/specify-rendering-options-when-converting-to-pdf/) für weitere Informationen über die Verwendung der `PdfSaveOptions`-Klasse
- Der Artikel [Lernen Sie die Funktionen der Konvertierung zu PDF/A und PDF/UA](/words/de/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) kennen, der beschreibt, welcher PDF-Standard und die entsprechenden ISO für PDF-Standards von Aspose.Words unterstützt werden
- Der Artikel [Welcher PDF-Standard ist besser zu wählen](/words/de/net/which-pdf-standard-is-better-to-choose/) zur Bestimmung, welche PDF-Standards für welche Fälle sinnvoll sind

- Der Artikel [Arbeiten mit PDF/A oder PDF/UA](/words/de/net/working-with-pdfa-or-pdfua/) beschreibt die Anforderungen an den Dokumentinhalt in PDF/A- und PDF/UA-Formaten – hauptsächlich die Anforderungen an Struktur und Schriften

- Der Artikel [Warnungen zu Barrierefreiheitsproblemen beim Speichern in PDF/A und PDF/UA](/words/de/net/warnings-when-saving-to-pdfa-and-pdfua/) beschreibt, welche Anforderungen an die Barrierefreiheit von Inhalten PDF/A und PDF/UA stellen
