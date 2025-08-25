---
title: Convert a Multi-page Document to an Image in C#
second_title: Aspose.Words for .NET
articleTitle: Convert a Multi-page Document to an Image
linktitle: Convert a Multi-page Document to an Image
type: docs
description: "Export multi-page documents to raster images (JPG, PNG, GIF, BMP, TIFF, WebP) using C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words for .NET allows users to export multi-page documents to raster images. This can be useful for generating previews, archives, or visual representations of documents for non-editable use.

## What Formats Support Multi-page Export?

Aspose.Words supports multi-page export to the following raster image formats:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## How to Export a Multi-page Document to an Image

The feature of exporting a multi-page document to an image is implemented using the [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) class – you can specify how the pages should be organized when saving to an image:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) – save only the first of the specified pages
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) – arrange the pages in a grid, left-to-right and top-to-bottom, while specifying the number of columns
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) – arrange the pages horizontally side-by-side, left-to-right, in a single output
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) – arrange the pages vertically one below the other in a single output
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) – arrange each page as a separate frame in a multi-frame TIFF image, applies only to TIFF image formats

The following code example shows how to save a multi-page DOCX document as JPEG image with Horizontal layout:

{{< gist "aspose-words-gists" "8eeaafcfcc55d78505f0f378ad8c6907" "horizontal-layout.cs" >}}

You can also customize the output file page appearance – specify [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/), and [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

The following code example shows how to save a multi-page DOCX document as PNG image with Grid layout:

{{< gist "aspose-words-gists" "8eeaafcfcc55d78505f0f378ad8c6907" "grid-layout.cs" >}}