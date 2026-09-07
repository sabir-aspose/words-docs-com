---
title: Working with Lists in Python
second_title: Aspose.Words for Python via .NET
articleTitle: Working with Lists
linktitle: Working with Lists
description: "Create, specify formatting and restart lists in a document using Python."
type: docs
weight: 200
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/working-with-lists/
aliases: [/python/working-with-lists/]
timestamp: 2026-02-03-11-08-55
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page demonstrates how to create, format, and manage lists—including multilevel lists and section-based restarts—using Aspose.Words for Python via .NET.

{{% /alert %}}

A list in a Microsoft Word document is a set of paragraph formatting properties. Lists can be used in documents to structure, arrange, and highlight text. Lists are a great way to organize data in documents in a way that makes it easy for readers to absorb and understand key points.

Each list can have up to 9 levels, and formatting properties such as number style, start value, indentation, tab position, and others are defined separately for each level.

In Aspose.Words, working with lists is represented by the [Lists](https://reference.aspose.com/words/python-net/aspose.words.lists/) namespace. However, the [List](https://reference.aspose.com/words/python-net/aspose.words.lists/list/) object always belongs to the [ListCollection](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/).

This article describes programmatically working with lists using Aspose.Words.

## Create Lists by Applying List Formatting

Aspose.Words allows the easy creation of lists by applying list formatting. [DocumentBuilder](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/) provides the [list_format](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/list_format/) property that returns a **ListFormat** object. This object has several methods to start and end a list and to increase/decrease the indent. There are two general types of lists in Microsoft Word: bulleted and numbered:

- To start a bulleted list, call [ListFormat.apply_bullet_default](https://reference.aspose.com/words/python-net/aspose.words.lists/listformat/apply_bullet_default/)
- To start a numbered list, call [ListFormat.apply_number_default](https://reference.aspose.com/words/python-net/aspose.words.lists/listformat/apply_number_default/)

The bullet or number and formatting are added to the current paragraph and all further paragraphs created using **DocumentBuilder** until [remove_numbers](https://reference.aspose.com/words/python-net/aspose.words.lists/listformat/remove_numbers/) is called to stop bulleted list formatting.

In Word documents, lists may consist of up to nine levels. List formatting for each level specifies what bullet or number is used, left indent, space between the bullet and text etc. The following methods change the list level and apply the new level's formatting properties:

- To increase the list level of the current paragraph by one level, call [ListFormat.list_indent](https://reference.aspose.com/words/python-net/aspose.words.lists/listformat/list_indent/)
- To decrease the list level of the current paragraph by one level, call [ListFormat.list_outdent](https://reference.aspose.com/words/python-net/aspose.words.lists/listformat/list_outdent/)

You can also use the [ListFormat.list_level_number](https://reference.aspose.com/words/python-net/aspose.words.lists/listformat/list_level_number/) property to get or set the list level for the paragraph.

{{% alert color="primary" %}}

The list levels are numbered 0 to 8.

{{% /alert %}}

The following code example shows how to build a multilevel list:

{{< gist "aspose-words-gists" "7aba3b36b61737610167905e1bd5f350" "multilevel-list-formatting.py" >}}

## Specify Formatting for a List Level

List-level objects are created automatically when a list is created. Use the properties and methods of the [ListLevel](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/) class to control the formatting of individual levels of a list.

## Restart List for each Section

You can restart a list for each section using the [is_restart_at_each_section](https://reference.aspose.com/words/python-net/aspose.words.lists/list/is_restart_at_each_section/) property. Note that this option is supported only in RTF, DOC and DOCX document formats. This option will be written to DOCX only if OoxmlCompliance is higher then Ecma376.

The following code example shows how to create a list and restart it for each section:

{{< gist "aspose-words-gists" "7aba3b36b61737610167905e1bd5f350" "restart-list-at-each-section.py" >}}