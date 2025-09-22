---
title: How to Add Group Shape into Word File
second_title: Aspose.Words for Node.js via .NET
articleTitle: Working with Group Shape in Word Documents
linktitle: Working with Group Shape in Word Documents
description: "Add group shape into a document using Node.js."
type: docs
weight: 290
ai_search_scope: words_nodejs
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nodejs-net/how-to-add-group-shape-into-a-word-document/
timestamp: 2025-07-09-10-05-05
---

Sometimes you need to add a group shape into a Word document. Such a group shape consists of multiple shapes.

In Microsoft Word, you can quickly add a group shape using the Group command/button. An individual shape in a group can be moved separately.

In Aspose.Words it is very easy to add a group shape using [GroupShape](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/groupshape/) class. Shape is created separately using [Shape](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shape/) class and then added in [GroupShape](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/groupshape/) object using [appendChild](https://reference.aspose.com/words/nodejs-net/aspose.words/compositenode/appendChild/) method.

The following code example shows how to add a group shape into a Word document:

{{< gist "aspose-words-gists" "072edc4bbb0dd0eebf1f61f610bd8d36" "add-group-shape.cs" >}}

{{% alert color="primary" %}}

Below are some of the `Shape` types supported in Aspose.Words. For complete list, please see [Aspose.Words.Drawing.ShapeType](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapetype/) enumeration

- [Rectangle](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapetype/)
- [RoundRectangle](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapetype/)
- [Ellipse](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapetype/)
- [Diamond](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapetype/)
- [Triangle](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapetype/)
- [RightTriangle](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapetype/)
- [Parallelogram](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapetype/)
- [Trapezoid](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapetype/)
- [Hexagon](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapetype/)
- [Octagon](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shapetype/)

{{% /alert %}}