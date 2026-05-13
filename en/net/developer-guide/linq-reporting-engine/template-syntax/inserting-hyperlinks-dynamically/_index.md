---
title: Inserting Hyperlinks Dynamically in C#
second_title: Aspose.Words for .NET
articleTitle: Inserting Hyperlinks Dynamically
linktitle: Inserting Hyperlinks Dynamically
description: "Insert hyperlinks into your document dynamically when building a report using C#."
type: docs
weight: 80
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/inserting-hyperlinks-dynamically/
aliases: [/net/template-syntax/#inserting-hyperlinks-dynamically]
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

## Purpose Summary

This page explains inserting hyperlinks dynamically.

{{% /alert %}}

You can insert hyperlinks to your reports dynamically using `link` tags. Syntax of a `link` tag is defined as follows.

{{< highlight csharp >}}
<<link [uri_or_bookmark_expression] [display_text_expression]>>
{{< /highlight >}}

Here, `uri_or_bookmark_expression` defines URI or the name of a bookmark within the same document for a hyperlink to be inserted dynamically. This expression is mandatory and must return a non-empty value.

In turn, `display_text_expression` defines text to be displayed for the hyperlink. This expression is optional. If it is omitted or returns an empty value, then during runtime, a value of `uri_or_bookmark_expression` is used as display text as well.

**Note** – Values of both `uri_or_bookmark_expression` and `display_text_expression` can be of any types. During runtime, `Object.ToString()` is invoked to get textual representations of these expressions’ values, which is useful for expressions of types like [URI](https://docs.microsoft.com/en-us/dotnet/api/system.uri?view=net-6.0), for example. 

While building a report, `uri_or_bookmark_expression` and `display_text_expression` are evaluated and their results are used to construct a hyperlink that replaces the corresponding `link` tag then. If `uri_or_bookmark_expression` returns the name of a bookmark in the same document, then the hyperlink navigates to the bookmark. Otherwise, the hyperlink navigates to a corresponding external resource.

**Note** – A `link` tag cannot be used within a chart.

------

## FAQ

1. **Q:** How can I link to a bookmark that exists in the same document?  
   **A:** Pass the bookmark name as the `uri_or_bookmark_expression`. At runtime the engine resolves the name to the corresponding bookmark and creates an internal hyperlink that jumps to that location.

2. **Q:** What is displayed if I omit the `display_text_expression`?  
   **A:** When the display text is omitted or evaluates to an empty string, the engine uses the string representation of `uri_or_bookmark_expression` as the visible text of the hyperlink.

3. **Q:** Can I provide a `System.Uri` object as the link target?  
   **A:** Yes. Any object is accepted; its `ToString()` result is used. Supplying a `Uri` instance works directly and the generated hyperlink points to the URI represented by that object.

4. **Q:** Why does a hyperlink not work when I place a `link` tag inside a chart?  
   **A:** The `link` tag is not supported inside chart elements. Move the tag outside the chart or use a different approach (e.g., inserting the hyperlink after the chart is rendered) to avoid this limitation.

5. **Q:** How can I make the hyperlink open in a new browser window or tab?  
   **A:** The `link` tag itself does not expose a target attribute. To control the opening behavior, generate the hyperlink as an HTML `<a>` element with `target="_blank"` using the `InsertHtml` method, or post‑process the document to set the appropriate field code.