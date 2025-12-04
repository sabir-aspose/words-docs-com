---
title: Add Bookmark
second_title: Aspose.Words for .NET
articleTitle: Add Bookmark
linktitle: Add Bookmark
description: "Add a bookmark into a document easily and fast instead of using VSTO in C#."
type: docs
weight: 70
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/add-bookmark/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*What is this page about?*

This page outlines how to add bookmarks to a Word document programmatically using Aspose.Words.

{{% /alert %}}

## VSTO

{{< highlight csharp >}}
Word.Application wordApp = Application;
wordApp.Documents.Open("Add Bookmark.doc");
Document extendedDocument = Globals.Factory.GetVstoObject(this.Application.ActiveDocument);
Bookmark firstParagraph = extendedDocument.Controls.AddBookmark(
	extendedDocument.Paragraphs[1].Range, "FirstParagraph");
{{< /highlight >}}

## Aspose.Words

{{< highlight csharp >}}
Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);
builder.StartBookmark("MyBookmark");
builder.Writeln("Text inside a bookmark.");
builder.EndBookmark("MyBookmark");
doc.Save("Adding Bookmark.doc");
{{< /highlight >}}

## Download Sample Code

- [Github](https://github.com/asposemarketplace/Aspose_for_VSTO/releases/download/Aspose.Words1.0/Add.Bookmark.Aspose.Words.zip)
