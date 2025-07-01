---
title: Konvertieren Sie ein mehrseitiges Dokument in ein Bild in Python
second_title: Aspose.Words für Python
articleTitle: Konvertieren Sie ein mehrseitiges Dokument in ein Bild
linktitle: Konvertieren Sie ein mehrseitiges Dokument in ein Bild
type: docs
description: "Exportieren Sie mehrseitige Dokumente in Rasterbilder (JPG, PNG, GIF, BMP, TIFF, WebP) mit Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /de/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words für Python via .NET ermöglicht Benutzern das Exportieren mehrseitiger Dokumente in Rasterbilder. Dies kann nützlich sein, um Vorschauen, Archive oder visuelle Darstellungen von Dokumenten für nicht bearbeitbare Zwecke zu erstellen.

## Welche Formate unterstützen den mehrseitigen Export?

Aspose.Words unterstützt den mehrseitigen Export in die folgenden Rasterbildformate:

* Jpeg
* Gifs
* Png
* Bmp
* Tiff
* WebP

## So exportieren Sie ein mehrseitiges Dokument in ein Bild

Die Funktion zum Exportieren eines mehrseitigen Dokuments in ein Bild wird mithilfe der Klasse [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) implementiert – Sie können angeben, wie die Seiten beim Speichern in einem Bild organisiert werden sollen:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - speichert nur die erste der angegebenen Seiten
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - Ordnen Sie die Seiten in einem Raster von links nach rechts und von oben nach unten an, während Sie die Anzahl der Spalten angeben
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - Ordnen Sie die Seiten horizontal nebeneinander von links nach rechts in einer einzigen Ausgabe an
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - ordne die Seiten vertikal untereinander in einer einzigen Ausgabe an
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - Ordne jede Seite als separaten Rahmen in einem TIFF -Bild mit mehreren Rahmen an, gilt nur für TIFF-Bildformate

Das folgende Codebeispiel zeigt, wie Sie ein mehrseitiges DOCX -Dokument als JPEG -Bild mit horizontalem Layout speichern:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Sie können auch das Erscheinungsbild der Ausgabedateiseite anpassen – geben Sie [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) und [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/) an.

Das folgende Codebeispiel zeigt, wie Sie ein mehrseitiges DOCX -Dokument als PNG -Bild mit Rasterlayout speichern:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.PNG)
# Set up a grid layout with:
# - 3 columns per row.
# - 10pts spacing between pages (horizontal and vertical).
options.page_layout = aw.saving.MultiPageLayout.grid(3, 10, 10)

# Customize the background and border.
options.page_layout.back_color = aspose.pydrawing.Color.light_gray
options.page_layout.border_color = aspose.pydrawing.Color.blue
options.page_layout.border_width = 2

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}