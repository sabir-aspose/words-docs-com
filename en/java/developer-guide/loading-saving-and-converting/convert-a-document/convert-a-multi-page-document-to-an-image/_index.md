---
title: Convert a Multi-page Document to an Image in Java
second_title: Aspose.Words for Java
articleTitle: Convert a Multi-page Document to an Image
linktitle: Convert a Multi-page Document to an Image
type: docs
description: "Export multi-page documents to raster images (JPG, PNG, GIF, BMP, TIFF, WebP) using Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words for Java allows users to export multi-page documents to raster images. This can be useful for generating previews, archives, or visual representations of documents for non-editable use.

## What Formats Support Multi-page Export?

Aspose.Words supports multi-page export to the following raster image formats:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## How to Export a Multi-page Document to an Image

The feature of exporting a multi-page document to an image is implemented using the [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) class – you can specify how the pages should be organized when saving to an image:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) – save only the first of the specified pages
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) – arrange the pages in a grid, left-to-right and top-to-bottom, while specifying the number of columns
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) – arrange the pages horizontally side-by-side, left-to-right, in a single output
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) – arrange the pages vertically one below the other in a single output
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) – arrange each page as a separate frame in a multi-frame TIFF image, applies only to TIFF image formats

The following code example shows how to save a multi-page DOCX document as JPEG image with Horizontal layout:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

You can also customize the output file page appearance – specify [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor), and [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

The following code example shows how to save a multi-page DOCX document as PNG image with Grid layout:

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