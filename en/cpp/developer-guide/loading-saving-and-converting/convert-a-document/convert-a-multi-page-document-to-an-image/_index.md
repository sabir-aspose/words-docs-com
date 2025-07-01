---
title: Convert a Multi-page Document to an Image in C++
second_title: Aspose.Words for C++
articleTitle: Convert a Multi-page Document to an Image
linktitle: Convert a Multi-page Document to an Image
type: docs
description: "Export multi-page documents to raster images (JPG, PNG, GIF, BMP, TIFF, WebP) using C++."
weight: 45
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cpp/convert-a-multi-page-document-to-an-image/
timestamp: 2025-07-01-11-12-25
---

Aspose.Words for C++ allows users to export multi-page documents to raster images. This can be useful for generating previews, archives, or visual representations of documents for non-editable use.

## What Formats Support Multi-page Export?

Aspose.Words supports multi-page export to the following raster image formats:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## How to Export a Multi-page Document to an Image

The feature of exporting a multi-page document to an image is implemented using the [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/) class – you can specify how the pages should be organized when saving to an image:

* **SinglePage** – save only the first of the specified pages
* **Grid** – arrange the pages in a grid, left-to-right and top-to-bottom, while specifying the number of columns
* **Horizontal** – arrange the pages horizontally side-by-side, left-to-right, in a single output
* **Vertical** – arrange the pages vertically one below the other in a single output
* **TiffFrames** – arrange each page as a separate frame in a multi-frame TIFF image, applies only to TIFF image formats

The following code example shows how to save a multi-page DOCX document as JPEG image with Horizontal layout:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

You can also customize the output file page appearance – specify **BackColor**, **BorderColor**, and **BorderWidth**.

The following code example shows how to save a multi-page DOCX document as PNG image with Grid layout:

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