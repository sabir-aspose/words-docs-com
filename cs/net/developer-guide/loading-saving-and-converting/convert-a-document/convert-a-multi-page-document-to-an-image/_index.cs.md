---
title: Převod vícestránkového dokumentu na obrázek v C#
second_title: Aspose.Words pro .NET
articleTitle: Převod vícestránkového dokumentu na obrázek
linktitle: Převod vícestránkového dokumentu na obrázek
type: docs
description: "Export vícestránkových dokumentů do rastrových obrázků (JPG, PNG, GIF, BMP, TIFF, WebP) Použití C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words pro .NET umožňuje uživatelům exportovat vícestránkové dokumenty do rastrových obrázků. To může být užitečné pro generování náhledů, archivů nebo vizuálních reprezentací dokumentů pro neupravitelné použití.

## Jaké formáty podporují vícestránkový Export?

Aspose.Words podporuje vícestránkový export do následujících formátů rastrových obrázků:

* JPEG
* GIF
* GIF
* BMP
* TIFF
* WebP

## Jak exportovat vícestránkový dokument do obrázku

Funkce exportu vícestránkového dokumentu do obrázku je implementována pomocí třídy [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) - můžete určit, jak by měly být stránky uspořádány při ukládání do obrázku:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - uložte pouze první ze zadaných stránek
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - uspořádejte stránky do mřížky, zleva doprava a shora dolů, přičemž zadejte počet sloupců
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - uspořádejte stránky vodorovně vedle sebe, zleva doprava, do jednoho výstupu
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - uspořádejte stránky svisle pod sebou do jednoho výstupu
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - uspořádejte každou stránku jako samostatný rámeček v obrázku s více snímky TIFF, platí pouze pro formáty obrázků TIFF 

Následující příklad kódu ukazuje, jak uložit vícestránkový dokument DOCX jako obrázek JPEG s horizontálním rozložením:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Můžete také přizpůsobit vzhled stránky výstupního souboru-zadejte [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) a [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

Následující příklad kódu ukazuje, jak uložit vícestránkový dokument DOCX jako obrázek PNG s rozložením mřížky:

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