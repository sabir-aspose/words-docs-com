---
title: Inserting HTML Dynamically in Java
second_title: Aspose.Words for Java
articleTitle: Inserting HTML Dynamically
linktitle: Inserting HTML Dynamically
description: "Insert HTML into your document dynamically when building a report in Java."
type: docs
weight: 55
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /java/inserting-html-dynamically/
timestamp: 2024-01-27-14-07-04
---

You can insert HTML to your reports dynamically by using one of the following two options.

The first one is using of an expression tag with an `html` switch applied as follows.

{{< highlight csharp >}}
<<[html_text_expression] -html>>
{{< /highlight >}}

This option is useful when you need to override formatting of some parts of an expression result, for example, highlight a word with a bold or italic font while staying consistent with styles of a template document. For more information on dynamic HTML insertion using this approach, see “Outputting Expression Results”.

The second option for dynamic HTML insertion is using of an `html` tag. An `html` tag denotes a placeholder within a template for an HTML block to be inserted during runtime. Its syntax is defined as follows.

{{< highlight csharp >}}
<<html [html_text_expression]>>
{{< /highlight >}}

**Note** – An `html` tag is forbidden within charts.

While building a report, an expression declared within an `html` tag is evaluated and its result as a string is interpreted as an HTML block which content replaces the `html` tag then.

In its base usage, an `html` tag behaves exactly the same as an expression tag with an `html` switch applied. In particular, it makes the engine to use corresponding styles of a template document. This makes content of a result document look more consistent. However, you can keep source HTML formatting for content being inserted (to make it look like in a browser) by using a `sourceStyles` switch as shown in the following snippet.

{{< highlight csharp >}}
<<html [html_text_expression] -sourceStyles>>
{{< /highlight >}}

------ 

## FAQ

1. **Q:** How do I insert HTML using an expression tag with the `-html` switch?  
   **A:** Place the expression inside double‑angle brackets and add the `-html` switch, e.g., `<<[myHtml] -html>>`. The engine evaluates the expression, treats the result as HTML, and inserts it while applying the template's styles.

2. **Q:** When should I prefer the `html` tag over an expression tag with `-html`?  
   **A:** Use the `html` tag when you want a clear placeholder in the template that will be completely replaced by the evaluated HTML at runtime. It is especially handy for larger HTML blocks or when you need the `sourceStyles` option.

3. **Q:** Can I use the `html` tag inside a chart?  
   **A:** No. The `html` tag is forbidden within chart definitions. Attempting to do so will cause a runtime error. Use plain text or image placeholders inside charts instead.

4. **Q:** How can I preserve the original HTML styling (fonts, colors, etc.) when inserting it?  
   **A:** Add the `-sourceStyles` switch to the `html` tag, e.g., `<<html [myHtml] -sourceStyles>>`. This tells the engine to keep the HTML's own styling rather than mapping it to the template's styles.