---
title: OLE Objects and Online Video
second_title: Aspose.Words for Node.js via .NET
articleTitle: Working with OLE Objects and Online Video
linktitle: Working with OLE Objects and Online Video
description: "Insert ole objects or onlin vodeo into a document using Node.js."
type: docs
weight: 360
ai_search_scope: words_nodejs
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nodejs-net/working-with-ole-objects/
timestamp: 2025-07-09-10-05-05
---

OLE (Object Linking and Embedding) is a technology by which users can work with documents containing "objects" created or edited by third-party applications. That is, OLE allows an editing application to export these "objects" to another editing application and then import them with additional content.

In this article, we will talk about inserting an OLE object and setting its properties, as well as inserting an online video into a document.

## Insert OLE Object

If you want OLE Object, call the [insertOleObject](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/insertoleobject/) method and pass it the **ProgId** explicitly with other parameters.

The following code example shows how to insert OLE Object into a document:

{{< gist "aspose-words-gists" "82ca803e5833cb807b7e1c5111066cb0" "insert-ole-object.js" >}}

### Insert OLE Object as an Icon

OLE objects can also be inserted into documents as images.

The following code example shows how to insert OLE Object as an icon. For this purpose, the [DocumentBuilder](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/) class exposes the [insertOleObjectAsIcon](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/insertoleobjectasicon/) method:

{{< gist "aspose-words-gists" "82ca803e5833cb807b7e1c5111066cb0" "insert-ole-object-as-icon.js" >}}

## Insert Online Video

Online video can be inserted into Word document from the *"Insert" > "Online Video"* tab. You can insert an online video into a document at the current location by calling the [insertOnlineVideo](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/insertonlinevideo/) method.

The [DocumentBuilder](https://reference.aspose.com/words/nodejs-net/aspose.words/documentbuilder/) class introduces four overloads of this method. The first one works with the most popular video resources and takes the `URL` of the video as a parameter. For example, the first overload supports simple insertion of online videos from [YouTube](https://www.youtube.com/) and [Vimeo](https://vimeo.com/) resources.

The following code example shows how to insert an online video from *Vimeo* into a document:

{{< gist "aspose-words-gists" "82ca803e5833cb807b7e1c5111066cb0" "insert-online-video.js" >}}

The second overload works with all other video resources and takes embedded HTML code as a parameter. The HTML code for embedding a video may vary depending on the provider, so contact the respective provider for details.

{{% alert color="primary" %}}

Please note that the document will be automatically optimized for MS Word 2013 to show video.

{{% /alert %}}
