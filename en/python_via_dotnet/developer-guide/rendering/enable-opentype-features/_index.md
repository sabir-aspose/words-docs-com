---
title: Enable OpenType Features in Python
second_title: Aspose.Words for Python via .NET
articleTitle: Enable OpenType Features
linktitle: Enable OpenType Features
description: "Advanced typography features using Python."
type: docs
weight: 25
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/enable-opentype-features/
timestamp: 2026-08-17-10-43-57
---

{{% alert color="grey" %}}

## Purpose Summary

This page explains how to enable OpenType font features such as ligatures and stylistic sets.

{{% /alert %}}

OpenType is a font format, introduced to provide better support for international languages and writing systems as compared to PostScript and TrueType. The layout features of OpenType are commonly known as OpenType features.

Aspose.Words is capable of using text shaper objects provided externally. A text shaper represents a font and computes shaping information for a text. A document typically refers to multiple fonts thus a text shaper factory is necessary.

{{% alert color="primary" %}}

Text shaping is only performed when exporting to PDF or XPS formats.

{{% /alert %}}

In a typical application single instance of a text shaper factory is shared among all document instances. Whenever text shaper is created a font file is accessed. Parsing a font file is an expensive operation thus caching is recommended. Aspose.Words implements BasicTextShaperCache class which wraps text shaper factory implementation and caches text shaper instances returned by the wrapped factory.

The following code example shows you how to turn on support of OpenType features.

{{< gist "aspose-words-gists" "b5ab3801a7643f50529361fb177f61f5" "open-type-features.py" >}}