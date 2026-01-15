---
title: Convert a Multi-page Document to an Image in Python
second_title: Aspose.Words for Python
articleTitle: Convert a Multi-page Document to an Image
linktitle: Convert a Multi-page Document to an Image
type: docs
description: "Export multi-page documents to raster images (JPG, PNG, GIF, BMP, TIFF, WebP) using Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words for Python via .NET allows users to export multi-page documents to raster images. This can be useful for generating previews, archives, or visual representations of documents for non-editable use.

## What Formats Support Multi-page Export?

Aspose.Words supports multi-page export to the following raster image formats:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## How to Export a Multi-page Document to an Image

The feature of exporting a multi-page document to an image is implemented using the [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) class – you can specify how the pages should be organized when saving to an image:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) – save only the first of the specified pages
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) – arrange the pages in a grid, left-to-right and top-to-bottom, while specifying the number of columns
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) – arrange the pages horizontally side-by-side, left-to-right, in a single output
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) – arrange the pages vertically one below the other in a single output
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) – arrange each page as a separate frame in a multi-frame TIFF image, applies only to TIFF image formats

The following code example shows how to save a multi-page DOCX document as JPEG image with Horizontal layout:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

You can also customize the output file page appearance – specify [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/), and [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

The following code example shows how to save a multi-page DOCX document as PNG image with Grid layout:

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

doc.save(file_name='ImageSaveOptions.GridLayout.png', save_options=options)
{{< /highlight >}}

------ 

## FAQ

1. **Q:** How can I export only specific pages of a document to an image?  
   **A:** Use the `PageSet` property of `ImageSaveOptions`. For example:  
   ```csharp
   options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
   options.page_set = aw.saving.PageSet(ranges=[aw.saving.PageRange(1, 2)])   // export pages 2-3, PageSet has zero-based index
   doc.save('SelectedPages.jpg', options)
   ```

2. **Q:** How do I change the resolution (DPI) of the exported image?  
   **A:** Set the `vertical_resolution` or `horizontal_resolution` property on `ImageSaveOptions`. Higher DPI yields larger, higher‑quality images:  
   ```csharp
   options = aw.saving.ImageSaveOptions(aw.SaveFormat.PNG)
   options.horizontal_resolution = 72   // 72 DPI
   doc.save('HighRes.png', options)
   ```

3. **Q:** Can I create a multi‑frame TIFF where each page is a separate frame?  
   **A:** Yes. Choose the `TiffFrames` layout and save using the TIFF format:  
   ```csharp
   options = aw.saving.ImageSaveOptions(aw.SaveFormat.TIFF)
   options.page_layout = aw.saving.MultiPageLayout.tiff_frames()
   doc.save('MultiFrame.tiff', options)
   ```

4. **Q:** What is the difference between `SinglePage` and `Grid` layouts?  
   **A:** `SinglePage` saves only the first page (or the page specified by `PageSet`). `Grid` arranges multiple pages in a matrix, letting you define the number of columns and spacing between pages.

5. **Q:** How can I customize the background and border of the layout?  
   **A:** Use the `back_color`, `border_color`, and `border_width` properties of the `page_layout` object:  
   ```csharp
   options.page_layout.back_color = aspose.pydrawing.Color.white
   options.page_layout.border_color = aspose.pydrawing.Color.black
   options.page_layout.border_width = 1
   ```