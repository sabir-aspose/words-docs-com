---
title: Working with Bookmarks in Python
second_title: Aspose.Words for Python via .NET
articleTitle: Working with Bookmarks
linktitle: Working with Bookmarks
description: "How to insert, obtain, move, show or hide bookmarks using Python."
type: docs
weight: 180
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/working-with-bookmarks/
aliases: [/python/working-with-bookmarks/]
timestamp: 2026-02-03-11-08-55
---

{{% alert color="grey" %}}
*Purpose Summary. What is this page about?*

This page demonstrates how to use Aspose.Words for Python via .NET to create, retrieve, modify, navigate, and conditionally display bookmarks in Word documents, providing code examples for each operation.
{{% /alert %}}

Bookmarks identify in a Microsoft Word document the locations or fragments that you name and identify for future reference. For example, you might use a bookmark to identify text that you want to revise later. Instead of scrolling through the document to locate the text, you can go to it by using the Bookmark dialog box.

The actions that can be performed with bookmarks using Aspose.Words are the same as the ones you can perform using Microsoft Word. You can insert a new bookmark, delete, move to a bookmark, get or set a bookmark name, get or set text enclosed in it.

## Insert a Bookmark

Use [start_bookmark](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/start_bookmark/) and [end_bookmark](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/end_bookmark/) to create a bookmark by marking its start and end, respectively. Do not forget to pass the same bookmark name to both methods. Bookmarks in a document can overlap and span any range. Badly formed bookmarks or bookmarks with duplicate names will be ignored when the document is saved.

{{% alert color="primary" %}}

All white spaces in the bookmarks were replaced with underscores. This restriction came from Microsoft Word formats, since bookmarks in Word formats like DOCX or DOC cannot have white spaces. However, PDF allows such bookmarks. So now, if you need to use bookmarks in PDF or XPS outlines, you can use them with white spaces.

{{% /alert %}}

The following code example shows how to create a new bookmark:

{{< gist "aspose-words-gists" "80b995172a159ce9559ebaf82c1b4f2d" "create-bookmark.py" >}}

## Obtain Bookmarks

Sometimes it is necessary to obtain a bookmark collection to iterate through bookmarks or for other purposes. Use the [Node.range](https://reference.aspose.com/words/python-net/aspose.words/node/range/) property exposed by any document node that returns a [Range](https://reference.aspose.com/words/python-net/aspose.words/range/) object representing the portion of the document contained in this node. Use this object to retrieve a [BookmarkCollection](https://reference.aspose.com/words/python-net/aspose.words/bookmarkcollection/) and then use the collection indexer to get a specific bookmark.

The following code example shows how to obtain bookmarks from a bookmark collection:

{{< gist "aspose-words-gists" "80b995172a159ce9559ebaf82c1b4f2d" "access-bookmarks.py" >}}

{{% alert color="primary" %}}

You can download the sample file of this example from [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Bookmarks.docx).

{{% /alert %}}

The following code example shows how to get or set a bookmark name and text:

{{< gist "aspose-words-gists" "80b995172a159ce9559ebaf82c1b4f2d" "update-bookmark-data.py" >}}

{{% alert color="primary" %}}

You can download the sample file of this example from [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Bookmarks.docx).

{{% /alert %}}

The following code example shows how to bookmark a table:

{{< gist "aspose-words-gists" "80b995172a159ce9559ebaf82c1b4f2d" "bookmark-table.py" >}}

If you change the name of a bookmark to a name that already exists in the document, no error will be generated and only the first bookmark will be stored when you save the document.

Note that some bookmarks in the document are assigned to form fields. Moving to such a bookmark and inserting text there inserts the text into the form field code. Although this will not invalidate the form field, the inserted text will not be visible because it becomes part of the field code.

The following code example shows how to access columns of the bookmarked table:

{{< gist "aspose-words-gists" "80b995172a159ce9559ebaf82c1b4f2d" "bookmark-table-columns.py" >}}

## Move to a Bookmark

If you need to insert rich content (not just plain text) into a bookmark, you should use [move_to_bookmark](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/move_to_bookmark/) to move the cursor to the bookmark and then use [DocumentBuilder's](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/) methods and properties to insert content.

## Show Hide Bookmark Content

The entire Bookmark (*including the bookmarked content*) can be encapsulated within the True part of the `IF` field using Aspose.Words. It can be in such a way that the `IF` field contains a nested Merge Field in the expression (*Left of Operator*) and depending upon the value of Merge Field, the `IF` field shows or hides the content of Bookmark in Word Document.

The following code example shows how to show/ hide bookmarks:

{{< gist "aspose-words-gists" "80b995172a159ce9559ebaf82c1b4f2d" "show-hide-bookmarks.py" >}}

{{< gist "aspose-words-gists" "80b995172a159ce9559ebaf82c1b4f2d" "show-hide-bookmarked-content.py" >}}