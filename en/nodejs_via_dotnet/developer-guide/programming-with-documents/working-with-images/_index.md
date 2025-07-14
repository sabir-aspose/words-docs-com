---
title: Working with Images in Node.js
second_title: Aspose.Words for Node.js via .NET
articleTitle: Working with Images
linktitle: Working with Images
description: "Create and manage images of various formats in a document using Node.js."
type: docs
weight: 300
ai_search_scope: words_nodejs
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nodejs-net/working-with-images/
timestamp: 2025-07-09-10-05-05
---

Aspose.Words allows users to work with images in a very flexible way. In this article, you can explore only some of the possibilities of working with images.

## Inserting an Image

[DocumentBuilder](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/) provides several overloads of the the [insertImage](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/insertImage/) method that allows you to insert an inline or floating image. If the image is an EMF or WMF metafile, it will be inserted into the document in metafile format. All other images will be stored in PNG format. The **insert_image** method can use images from different sources:

- From a file or `URL` by passing a string parameter
- From a stream by passing a `Stream` parameter
- From a byte array by passing a byte array parameter

For each of the **insert_image** methods, there are further overloads which allow you to insert an image with the following options:
- Inline or floating at a specific position, for example, **insert_image**
- Percentage scale or custom size; furthermore, the [DocumentBuilder.insertImage](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/insertImage/) method returns a [Shape](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shape/) object that was just created and inserted so you can further modify properties of the [Shape](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shape/)

### Inserting an Inline Image

Pass a single string representing a file that contains the image to [insertImage](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/insertImage/) to insert the image into the document as an inline graphic.

The following code example shows how to insert an inline image at the cursor position into a document:

{{< highlight python >}}
doc = aw.Document()
builder = aw.DocumentBuilder(doc)

builder.insert_image(docs_base.images_dir + "Logo.jpg")

doc.save(docs_base.artifacts_dir+"WorkingWithImages.document_builder_insert_inline_image.doc")
{{< /highlight >}}

### Inserting a Floating (Absolutely Positioned) Image

The following code example shows how to insert a floating image from a file or `URL` at a specified position and size:

{{< highlight python >}}
doc = aw.Document()
builder = aw.DocumentBuilder(doc)

builder.insert_image(docs_base.images_dir + "Logo.jpg",
    aw.drawing.RelativeHorizontalPosition.MARGIN,
    100,
    aw.drawing.RelativeVerticalPosition.MARGIN,
    100,
    200,
    100,
    aw.drawing.WrapType.SQUARE)

doc.save(docs_base.artifacts_dir+"WorkingWithImages.document_builder_insert_floating_image.doc")
{{< /highlight >}}

## How to Extract Images from a Document

All images are stored inside [Shape](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shape/) nodes in a [Document](https://reference.aspose.com/words/nodejs-net/aspose.words/document/). To extract all images or images having specific type from the document, follow these steps:

- Use the [Document.getChildNodes](https://reference.aspose.com/words/nodejs-net/aspose.words/compositenode/getChildNodes/) method to select all [Shape](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shape/) nodes.
- Iterate through resulting node collections.
- Check the [Shape.hasImage](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shape/hasimage/) boolean property.
- Extract image data using the [Shape.imageData](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shape/imagedata/) property.
- Save image data to a file.

The following code example shows how to extract images from a document and save them as files:

You can download the template file of this example from [here](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Images.docx).

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Contents Management-extract_content-ExtractImagesToFiles.py" >}}

{{% alert color="primary" %}}

You can download the sample file of this example from [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Images.docx).

{{% /alert %}}

## How to Insert Barcode on each Page of a Document

This example demonstrates you to add the same or different barcodes on all or specific pages of a Word document. There is no direct way to add barcodes on all pages of a document but you can use the [moveToSection](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/moveToSection/), [moveToHeaderFooter](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/moveToHeaderFooter/) and [insertImage](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/insertImage/) methods to move to any section or headers/footers and insert the barcode images as you can see in the following code.

The following code example Inserts a barcode image on each page of a document.

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_images-InsertBarcodeImage.py" >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_images-InsertBarcodeIntoFooter.py" >}}

## Lock Aspect Ratio of Image

The aspect ratio of a geometric shape is the ratio of its sizes in different dimensions. You can lock the aspect ratio of the image using [aspectRatioLocked](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapebase/aspectratiolocked/). The default value of the shape's aspect ratio depends on the [ShapeType](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shadowtype/). It is `True` for [ShapeType.Image](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shadowtype/) and `False` for other shape types.

The following code example shows how to work with aspect ratio:

{{< highlight python >}}
doc = aw.Document()
builder = aw.DocumentBuilder(doc)

shape = builder.insert_image(docs_base.images_dir + "Logo.jpg")
shape.aspect_ratio_locked = False

doc.save(docs_base.artifacts_dir+"WorkingWithImages.set_aspect_ratio_locked.doc")
{{< /highlight >}}

## How to Get Actual Bounds of Shape in Points

If you want the actual bounding box of the shape as rendered on the page, you can achieve this by using the [boundsInPoints2](https://reference.aspose.com/words/nodejs-net/aspose.words.rendering/noderendererbase/boundsinpoints2/) property.

The following code example shows how to use this property:

{{< highlight python >}}
doc = aw.Document()
builder = aw.DocumentBuilder(doc)

shape = builder.insert_image(docs_base.images_dir + "Logo.jpg")
shape.aspect_ratio_locked = False

print("\nGets the actual bounds of the shape in points.")
rect = shape.get_shape_renderer().bounds_in_points
print(f"{rect.x}, {rect.y}, {rect.width}, {rect.height}")
{{< /highlight >}}

## Crop Images

The cropping of an image usually refers to the removal of the unwanted outer parts of an image to help improve the framing. It is also used for the removal of some of the portions of an image to increase the focus on a particular area.

The following code example shows how to achieve this using Aspose.Words API:

{{< highlight python >}}
# The path to the documents directory.
inputPath = docs_base.images_dir + "Logo.jpg"
outputPath = docs_base.artifacts_dir + "cropped_logo.jpg"

self.crop_image(inputPath,outputPath, 100, 90, 200, 200)
{{< /highlight >}}

{{< highlight python >}}
@staticmethod
def crop_image(inPath : str, outPath : str, left : int, top : int, width : int, height : int) :
    
    doc = aw.Document();
    builder = aw.DocumentBuilder(doc)
    
    croppedImage = builder.insert_image(inPath)
    
    src_width_points = croppedImage.width
    src_height_points = croppedImage.height
    
    croppedImage.width = aw.ConvertUtil.pixel_to_point(width)
    croppedImage.height = aw.ConvertUtil.pixel_to_point(height)
    
    widthRatio = croppedImage.width / src_width_points
    heightRatio = croppedImage.height / src_height_points
    
    if (widthRatio< 1) :
        croppedImage.image_data.crop_right = 1 - widthRatio
    
    if (heightRatio< 1) :
        croppedImage.image_data.crop_bottom = 1 - heightRatio
    
    leftToWidth = aw.ConvertUtil.pixel_to_point(left) / src_width_points
    topToHeight = aw.ConvertUtil.pixel_to_point(top) / src_height_points
    
    croppedImage.image_data.crop_left = leftToWidth
    croppedImage.image_data.crop_right = croppedImage.image_data.crop_right - leftToWidth
    
    croppedImage.image_data.crop_top = topToHeight
    croppedImage.image_data.crop_bottom = croppedImage.image_data.crop_bottom - topToHeight
    
    croppedImage.get_shape_renderer().save(outPath, aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG))
{{< /highlight >}}

## Saving Images as WMF

Aspose.Words provides functionality to save all the available images in a document to [WMF](https://docs.fileformat.com/image/wmf/) format while converting DOCX to RTF.

The following code example shows how to save images as WMF with RTF save options:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-File Formats and Conversions-Save Options-working_with_rtf_save_options-SavingImagesAsWmf.py" >}}
