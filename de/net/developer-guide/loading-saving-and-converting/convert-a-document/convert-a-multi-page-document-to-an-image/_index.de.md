---
title: Konvertieren Sie ein mehrseitiges Dokument in ein Bild in C#
second_title: Aspose.Words für .NET
articleTitle: Konvertieren Sie ein mehrseitiges Dokument in ein Bild
linktitle: Konvertieren Sie ein mehrseitiges Dokument in ein Bild
type: docs
description: "Exportieren Sie mehrseitige Dokumente in Rasterbilder (JPG, PNG, GIF, BMP, TIFF, WebP) mit C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /de/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words für .NET ermöglicht Benutzern das Exportieren mehrseitiger Dokumente in Rasterbilder. Dies kann nützlich sein, um Vorschauen, Archive oder visuelle Darstellungen von Dokumenten für nicht bearbeitbare Zwecke zu erstellen.

## Welche Formate unterstützen den mehrseitigen Export?

Aspose.Words unterstützt den mehrseitigen Export in die folgenden Rasterbildformate:

* Jpeg
* Gifs
* Png
* Bmp
* Tiff
* WebP

## So exportieren Sie ein mehrseitiges Dokument in ein Bild

Die Funktion zum Exportieren eines mehrseitigen Dokuments in ein Bild wird mithilfe der Klasse [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) implementiert – Sie können angeben, wie die Seiten beim Speichern in einem Bild organisiert werden sollen:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - speichert nur die erste der angegebenen Seiten
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - Ordnen Sie die Seiten in einem Raster von links nach rechts und von oben nach unten an, während Sie die Anzahl der Spalten angeben
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - Ordnen Sie die Seiten horizontal nebeneinander von links nach rechts in einer einzigen Ausgabe an
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - ordne die Seiten vertikal untereinander in einer einzigen Ausgabe an
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - Ordne jede Seite als separaten Rahmen in einem TIFF -Bild mit mehreren Rahmen an, gilt nur für TIFF-Bildformate

Das folgende Codebeispiel zeigt, wie Sie ein mehrseitiges DOCX -Dokument als JPEG -Bild mit horizontalem Layout speichern:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Sie können auch das Erscheinungsbild der Ausgabedateiseite anpassen – geben Sie [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) und [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/) an.

Das folgende Codebeispiel zeigt, wie Sie ein mehrseitiges DOCX -Dokument als PNG -Bild mit Rasterlayout speichern:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Png);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.PageLayout = MultiPageLayout.Grid(3, 10, 10);

// Customize the background and border.
options.PageLayout.BackColor = Color.LightGray;
options.PageLayout.BorderColor = Color.Blue;
options.PageLayout.BorderWidth = 2;

doc.Save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}