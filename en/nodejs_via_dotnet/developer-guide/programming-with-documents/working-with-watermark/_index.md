---
title: Working with Watermark in Node.js
second_title: Aspose.Words for Node.js via .NET
articleTitle: Working with Watermark
linktitle: Working with Watermark
description: "Create and manage watermarks in a document using Node.js."
type: docs
weight: 340
ai_search_scope: words_nodejs
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nodejs-net/working-with-watermark/
timestamp: 2025-07-09-10-05-05
---

This topic discusses how to work programmatically with watermark using Aspose.Words. A watermark is a background image that displays behind the text in a document. A watermark can contain a text or an image represented by the [Watermark](https://reference.aspose.com/words/nodejs-net/aspose.words/watermark/) class.

{{% alert color="primary" %}}

**Try online**

You can try this functionality with our [Free online document watermark](https://products.aspose.app/words/watermark).

{{% /alert %}}

## How to Add a Watermark to a Document

In Microsoft Word, a watermark can easily be inserted in a document using the Insert Watermark command. Aspose.Words provides the [Watermark](https://reference.aspose.com/words/nodejs-net/aspose.words/watermark/) class to add or remove watermark in documents. Aspose.Words provides the [WatermarkType](https://reference.aspose.com/words/nodejs-net/aspose.words/watermarktype/) enumeration defining three possible types of watermarks ([Text](https://reference.aspose.com/words/nodejs-net/aspose.words/watermarktype/), [Image](https://reference.aspose.com/words/nodejs-net/aspose.words/watermarktype/), and [None](https://reference.aspose.com/words/nodejs-net/aspose.words/watermarktype/)) to work with. 

### Add Text Watermark

The following code example demonstrates how to insert a text watermark in a document by defining [TextWatermarkOptions](https://reference.aspose.com/words/nodejs-net/aspose.words/textwatermarkoptions/) using the [setText](https://reference.aspose.com/words/nodejs-net/aspose.words/watermark/setText/) method:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Add Image Watermark

The following code example demonstrates how to insert an image watermark in a document by defining [ImageWatermarkOptions](https://reference.aspose.com/words/nodejs-net/aspose.words/imagewatermarkoptions/) using the [setImage](https://reference.aspose.com/words/nodejs-net/aspose.words/watermark/setImage/#jsimage) method:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Image watermark can be inserted as image, string, or stream.

The watermark can also be inserted using shape class as well. It is very easy to insert any shape or image into a header or footer and thus create a watermark of any imaginable type.

The following code example inserts a watermark into a Word document:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

You can download the template file of this example from [here](https://github.com/aspose-words/Aspose.Words-for-Node.js-via-.NET/tree/main/Data/Document.docx). 

{{% /alert %}}


## Remove Watermark from a Document

The [Watermark](https://reference.aspose.com/words/nodejs-net/aspose.words/watermark/) class provides the remove method to remove the watermark from a document.

The following code example shows how to remove a watermark from documents:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

If the watermarks are added using the [Shape](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shape/) class object then to remove the watermark from a document you have to set only the name of watermark shape during inserting and then remove watermark shape by an assigned name.

The following code example show you how to set the name of the watermark shape and remove it from the document:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Add a Watermark in Table Cell

Sometimes you need to insert a watermark/image into a table's cell and display it outside the table, you can use the [isLayoutInCell](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapebase/isLayoutInCell/) property. This property gets or sets a flag indicating whether the shape is displayed inside a table or outside of it. Note that this property works only when you optimize the document for Microsoft Word 2010 using the [optimizeFor](https://reference.aspose.com/words/nodejs-net/aspose.words.settings/compatibilityoptions/optimizeFor/) method.

The following code example shows how to use this property:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
