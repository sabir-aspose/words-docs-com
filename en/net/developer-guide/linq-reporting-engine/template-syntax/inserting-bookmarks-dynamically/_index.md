---
title: Inserting Bookmarks Dynamically in C#
second_title: Aspose.Words for .NET
articleTitle: Inserting Bookmarks Dynamically
linktitle: Inserting Bookmarks Dynamically
description: "Insert bookmarks into your document dynamically when building a report using C#."
type: docs
weight: 70
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /net/inserting-bookmarks-dynamically/
aliases: [/net/template-syntax/#inserting-bookmarks-dynamically]
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*What is this page about?*

This page explains how to insert bookmarks dynamically in reporting templates.

{{% /alert %}}

You can insert bookmarks to your reports dynamically using `bookmark` tags. Syntax of a `bookmark` tag is defined as follows.

{{< highlight csharp >}}
<<bookmark [bookmark_expression]>>
bookmarked_content
<</bookmark>>
{{< /highlight >}}

Here, `bookmark_expression` defines the name of a bookmark to be inserted during runtime. This expression is mandatory and must return a non-empty value. While building a report, `bookmark_expression` is evaluated and its result is used to construct a bookmark start and end that replace corresponding opening and closing `bookmark` tags respectively.

**Note** – A `bookmark` tag cannot be used within a chart.
