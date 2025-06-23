---
title: Převod vícestránkového dokumentu na obrázek v Java
second_title: Aspose.Words pro Java
articleTitle: Převod vícestránkového dokumentu na obrázek
linktitle: Převod vícestránkového dokumentu na obrázek
type: docs
description: "Export vícestránkových dokumentů do rastrových obrázků (JPG, PNG, GIF, BMP, TIFF, WebP) pomocí Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words pro Java umožňuje uživatelům exportovat vícestránkové dokumenty do rastrových obrázků. To může být užitečné pro generování náhledů, archivů nebo vizuálních reprezentací dokumentů pro neupravitelné použití.

## Jaké formáty podporují vícestránkový Export?

Aspose.Words podporuje vícestránkový export do následujících formátů rastrových obrázků:

* JPEG
* GIF
* GIF
* BMP
* TIFF
* WebP

## Jak exportovat vícestránkový dokument do obrázku

Funkce exportu vícestránkového dokumentu do obrázku je implementována pomocí třídy [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) - můžete určit, jak by měly být stránky uspořádány při ukládání do obrázku:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - uložte pouze první ze zadaných stránek
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - uspořádejte stránky do mřížky, zleva doprava a shora dolů, přičemž zadejte počet sloupců
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - uspořádejte stránky vodorovně vedle sebe, zleva doprava, do jednoho výstupu
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - uspořádejte stránky svisle pod sebou do jednoho výstupu
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - uspořádejte každou stránku jako samostatný rámeček v obrázku s více snímky TIFF, platí pouze pro formáty obrázků TIFF 

Následující příklad kódu ukazuje, jak uložit vícestránkový dokument DOCX jako obrázek JPEG s horizontálním rozložením:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Můžete také přizpůsobit vzhled stránky výstupního souboru-zadejte [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) a [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

Následující příklad kódu ukazuje, jak uložit vícestránkový dokument DOCX jako obrázek PNG s rozložením mřížky:

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