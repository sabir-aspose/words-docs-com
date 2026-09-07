---
title: How to Add Group Shape into Word File
second_title: Aspose.Words for Python via .NET
articleTitle: Working with Group Shape in Word Documents
linktitle: Working with Group Shape in Word Documents
description: "Add group shape into a document using Python."
type: docs
weight: 290
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/how-to-add-group-shape-into-a-word-document/
aliases: [/python/how-to-add-group-shape-into-a-word-document/]
timestamp: 2026-02-03-11-08-55
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page shows how to create a GroupShape—by adding individual Shape objects—to a Word document using Aspose.Words for Python via .NET.

{{% /alert %}}

Sometimes you need to add a group shape into a Word document. Such a group shape consists of multiple shapes.

In Microsoft Word, you can quickly add a group shape using the Group command/button. An individual shape in a group can be moved separately.

In Aspose.Words it is very easy to add a group shape using the [GroupShape](https://reference.aspose.com/words/python-net/aspose.words.drawing/groupshape/) class. **Shape** is created separately using the [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/) class and then added to the [GroupShape](https://reference.aspose.com/words/python-net/aspose.words.drawing/groupshape/) object using the [append_child](https://reference.aspose.com/words/python-net/aspose.words/compositenode/append_child/) method.

The following code example shows how to add a group shape into a Word document:

{{< gist "aspose-words-gists" "9b7beaa557bceeb51164ef9d43bf0cc7" "add-group-shape.py" >}}

{{% alert color="primary" %}}

Below are some of the `Shape` types supported in Aspose.Words:

- [Rectangle](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapetype/#rectangle)
- [RoundRectangle](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapetype/#round_rectangle)
- [Ellipse](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapetype/#ellipse)
- [Diamond](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapetype/#diamond)
- [Triangle](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapetype/#triangle)
- [RightTriangle](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapetype/#right_triangle)
- [Parallelogram](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapetype/#parallelogram)
- [Trapezoid](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapetype/#trapezoid)
- [Hexagon](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapetype/#hexagon)
- [Octagon](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapetype/#octagon)

For complete list, please check the [ShapeType](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapetype/) class.

{{% /alert %}}