---
title: Konvertieren Sie ein mehrseitiges Dokument in ein Bild in Java
second_title: Aspose.Words für Java
articleTitle: Konvertieren Sie ein mehrseitiges Dokument in ein Bild
linktitle: Konvertieren Sie ein mehrseitiges Dokument in ein Bild
type: docs
description: "Exportieren Sie mehrseitige Dokumente in Rasterbilder (JPG, PNG, GIF, BMP, TIFF, WebP) mit Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /de/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words für Java ermöglicht Benutzern das Exportieren mehrseitiger Dokumente in Rasterbilder. Dies kann nützlich sein, um Vorschauen, Archive oder visuelle Darstellungen von Dokumenten für nicht bearbeitbare Zwecke zu erstellen.

## Welche Formate unterstützen den mehrseitigen Export?

Aspose.Words unterstützt den mehrseitigen Export in die folgenden Rasterbildformate:

* Jpeg
* Gifs
* Png
* Bmp
* Tiff
* WebP

## So exportieren Sie ein mehrseitiges Dokument in ein Bild

Die Funktion zum Exportieren eines mehrseitigen Dokuments in ein Bild wird mithilfe der Klasse [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) implementiert – Sie können angeben, wie die Seiten beim Speichern in einem Bild organisiert werden sollen:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - speichert nur die erste der angegebenen Seiten
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - Ordnen Sie die Seiten in einem Raster von links nach rechts und von oben nach unten an, während Sie die Anzahl der Spalten angeben
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - Ordnen Sie die Seiten horizontal nebeneinander von links nach rechts in einer einzigen Ausgabe an
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - ordne die Seiten vertikal untereinander in einer einzigen Ausgabe an
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - Ordne jede Seite als separaten Rahmen in einem TIFF -Bild mit mehreren Rahmen an, gilt nur für TIFF-Bildformate

Das folgende Codebeispiel zeigt, wie Sie ein mehrseitiges DOCX -Dokument als JPEG -Bild mit horizontalem Layout speichern:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Sie können auch das Erscheinungsbild der Ausgabedateiseite anpassen – geben Sie [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) und [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth) an.

Das folgende Codebeispiel zeigt, wie Sie ein mehrseitiges DOCX -Dokument als PNG -Bild mit Rasterlayout speichern:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.PNG);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.setPageLayout(MultiPageLayout.grid(3, 10f, 10f));

// Customize the background and border.
options.getPageLayout().setBackColor(Color.lightGray);
options.getPageLayout().setBorderColor(Color.BLUE);
options.getPageLayout().setBorderWidth(2f);

doc.save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}