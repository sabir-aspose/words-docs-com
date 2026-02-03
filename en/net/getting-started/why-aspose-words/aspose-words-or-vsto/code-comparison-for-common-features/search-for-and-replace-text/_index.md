---
title: Find and Replace Text
second_title: Aspose.Words for .NET
articleTitle: Find and Replace Text
linktitle: Find and Replace Text
description: "Find and replace text from a document part easily and fast instead of using VSTO in C#."
type: docs
weight: 90
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/search-for-and-replace-text/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page explains how to search for and replace text across the entire document.

{{% /alert %}}

## VSTO

{{< highlight csharp >}}
Word.Application wordApp = Application;
wordApp.Documents.Open("Search and Replace.doc");
object replaceAll = Word.WdReplace.wdReplaceAll;
this.Application.Selection.Find.ClearFormatting();
this.Application.Selection.Find.Text = "find me";
this.Application.Selection.Find.Replacement.ClearFormatting();
this.Application.Selection.Find.Replacement.Text = "Found";
this.Application.Selection.Find.Execute(
	ref missing, ref missing, ref missing, ref missing, ref missing,
	ref missing, ref missing, ref missing, ref missing, ref missing,
	ref replaceAll, ref missing, ref missing, ref missing, ref missing);
{{< /highlight >}}

## Aspose.Words

{{< highlight csharp >}}
Document doc = new Document("Search and Replace.doc");
doc.Range.Replace("find me", "found", false, true);
doc.Save("Search and Replace.doc");
{{< /highlight >}}

## Download Sample Code

- [Github](https://github.com/asposemarketplace/Aspose_for_VSTO/releases/download/Aspose.Words1.0/Search.for.and.Replace.text.Asose.Words.zip)
