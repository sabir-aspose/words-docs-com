---
title: Konwertuj wielostronicowy dokument na obraz w Python
second_title: Aspose.Words dla Python
articleTitle: Konwertuj wielostronicowy dokument na obraz
linktitle: Konwertuj wielostronicowy dokument na obraz
type: docs
description: "Eksportuj wielostronicowe dokumenty do obrazów rastrowych(JPG, PNG, GIF, BMP, TIFF, WebP) używając Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pl/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words for Python via .NET umożliwia użytkownikom eksportowanie wielostronicowych dokumentów do obrazów rastrowych. Może to być przydatne do generowania podglądów, archiwów lub wizualnych reprezentacji dokumentów do użytku nieedytowalnego.

## Jakie formaty obsługują eksport wielostronicowy?

Aspose.Words obsługuje wielostronicowy eksport do następujących formatów obrazów rastrowych:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Jak wyeksportować wielostronicowy dokument do obrazu

Funkcja eksportowania wielostronicowego dokumentu do obrazu jest zaimplementowana przy użyciu klasy [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) – możesz określić sposób organizacji stron podczas zapisywania na obrazie:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - Zapisz tylko pierwszą z podanych stron
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - ułóż strony w siatce, od lewej do prawej i od góry do dołu, określając liczbę kolumn
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - ułóż strony poziomo obok siebie, od lewej do prawej, w jednym wyjściu
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - ułóż strony pionowo jedna pod drugą w jednym wyjściu
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - Rozmieść każdą stronę jako osobną ramkę w obrazie z wieloma klatkami TIFF, dotyczy tylko formatów obrazów TIFF 

Poniższy przykład kodu pokazuje, jak zapisać wielostronicowy dokument DOCX jako obraz JPEG z układem poziomym:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Możesz także dostosować wygląd strony pliku wyjściowego-określ [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) i [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

Poniższy przykład kodu pokazuje, jak zapisać wielostronicowy dokument DOCX jako obraz PNG z układem siatki:

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