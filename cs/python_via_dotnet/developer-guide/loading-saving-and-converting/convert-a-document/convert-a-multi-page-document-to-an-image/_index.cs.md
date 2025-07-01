---
title: Převod vícestránkového dokumentu na obrázek v Python
second_title: Aspose.Words pro Python
articleTitle: Převod vícestránkového dokumentu na obrázek
linktitle: Převod vícestránkového dokumentu na obrázek
type: docs
description: "Export vícestránkových dokumentů do rastrových obrázků (JPG, PNG, GIF, BMP, TIFF, WebP) Pomocí Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words pro Python via .NET umožňuje uživatelům exportovat vícestránkové dokumenty do rastrových obrázků. To může být užitečné pro generování náhledů, archivů nebo vizuálních reprezentací dokumentů pro neupravitelné použití.

## Jaké formáty podporují vícestránkový Export?

Aspose.Words podporuje vícestránkový export do následujících formátů rastrových obrázků:

* JPEG
* GIF
* GIF
* BMP
* TIFF
* WebP

## Jak exportovat vícestránkový dokument do obrázku

Funkce exportu vícestránkového dokumentu do obrázku je implementována pomocí třídy [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) - můžete určit, jak by měly být stránky uspořádány při ukládání do obrázku:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - uložte pouze první ze zadaných stránek
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - uspořádejte stránky do mřížky, zleva doprava a shora dolů, přičemž zadejte počet sloupců
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - uspořádejte stránky vodorovně vedle sebe, zleva doprava, do jednoho výstupu
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - uspořádejte stránky svisle pod sebou do jednoho výstupu
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - uspořádejte každou stránku jako samostatný rámeček v obrázku s více snímky TIFF, platí pouze pro formáty obrázků TIFF 

Následující příklad kódu ukazuje, jak uložit vícestránkový dokument DOCX jako obrázek JPEG s horizontálním rozložením:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Můžete také přizpůsobit vzhled stránky výstupního souboru-zadejte [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) a [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

Následující příklad kódu ukazuje, jak uložit vícestránkový dokument DOCX jako obrázek PNG s rozložením mřížky:

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