---
title: Working with Ranges in Python
second_title: Aspose.Words for Python via .NET
articleTitle: Working with Ranges
linktitle: Working with Ranges
description: "Work with ranges in a document using Python."
type: docs
weight: 130
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/working-with-ranges/
aliases: [/python/working-with-ranges/]
timestamp: 2026-02-03-11-08-55
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page explains how to use the Aspose.Words Range object in Python via .NET to access and modify document content, and provides code examples for retrieving plain text and deleting text within a range.

{{% /alert %}}

{{% alert color="primary" %}}

In Aspose.Words, a Range is a “flat window” into an otherwise tree-like model of the document.

{{% /alert %}}

If you have worked with Microsoft Word Automation, you probably know that one of the main tools to examine and modify document content is the **Range** object. **Range** is like a "window" into the document content and formatting.

Aspose.Words also has the [Range](https://reference.aspose.com/words/python-net/aspose.words/range/) class and it is designed to look and act similarly to **Range** in Microsoft Word. Although **Range** cannot cover an arbitrary portion of a document and does not have a **Start** and **End**, you can access the range covered by any document node including the [Document](https://reference.aspose.com/words/python-net/aspose.words/document/) itself. In other words, each node has its own range. The **Range** object allows you to access and modify text, bookmarks and form fields within the range.

## Retrieve Plain Text

Use the [text](https://reference.aspose.com/words/python-net/aspose.words/range/text/) property to retrieve plain, unformatted text of the range.

The following code example shows how to get a plain, unformatted text of a range:

{{< gist "aspose-words-gists" "add91ac6b670b016c322c0c3d23d5af9" "ranges-get-text.py" >}}

{{% alert color="primary" %}}

You can download the sample file of this example from [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}

## Delete Text

Range allows the deletion of all characters of the range by calling [delete](https://reference.aspose.com/words/python-net/aspose.words/range/delete/).

The following code example shows how to delete all characters of a range:

{{< gist "aspose-words-gists" "add91ac6b670b016c322c0c3d23d5af9" "ranges-delete-text.py" >}}

{{% alert color="primary" %}}

You can download the sample file of this example from [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}