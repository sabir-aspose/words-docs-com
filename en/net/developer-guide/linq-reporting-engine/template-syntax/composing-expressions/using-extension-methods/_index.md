---
title: Using Extension Methods in C#
second_title: Aspose.Words for .NET
articleTitle: Using Extension Methods
linktitle: Using Extension Methods
description: "Use extension methods in template expressions when building a report in C#."
type: docs
weight: 40
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/using-extension-methods-linq/
timestamp: 2024-02-16-10-54-23
---

{{% alert color="grey" %}}

## Purpose Summary

This page explains how to use extension methods within LINQ Reporting Engine templates.

{{% /alert %}}

LINQ Reporting Engine enables you to use the following built‑in extension methods in template expressions:

- Extension methods mimicking the ones for `IEnumerable<T>` (see "Appendix A. Enumeration Extension Methods" for more information)
- Extension methods for iteration variables (see "Using Extension Methods of Iteration Variables" for more information)

**Note** – Extension methods, other than the built‑in ones, can be used only in the form of plain static methods in template expressions.

------ 

## FAQ

1. **Q:** How can I call a custom static method as an extension method in a LINQ Reporting Engine template?  
   **A:** Place the method in a public static class, make the method itself public static, and reference it directly in the template expression using the full class name, e.g., `MyUtilities.FormatDate(DateTime.Now)`. No additional registration is required.

2. **Q:** Are the built‑in extension methods available for iteration variables such as `$row$`?  
   **A:** Yes. Iteration variables expose the same enumeration extension methods as `IEnumerable<T>`, so you can write expressions like `$row$.Where(r => r.Price > 100)` directly in the template.

3. **Q:** Can I use full LINQ query operators like `Select` or `OrderBy` inside a template expression?  
   **A:** Only the extension methods listed in the documentation are supported. Full LINQ syntax is not available in template expressions; use the provided enumeration extension methods instead.

4. **Q:** Why do I receive a “Method not found” error when using an extension method in a template?  
   **A:** The method must be public, static, and located in an assembly that the reporting engine can load. Also ensure the method signature uses only supported parameter types (primitive types, `string`, `DateTime`, etc.). Overloads with unsupported types will cause the engine to fail to locate the method.

5. **Q:** Can I return a custom object type from an extension method used in a template?  
   **A:** The engine can render only primitive types, `string`, and `DateTime` directly. If your method returns a custom type, convert it to a supported type (e.g., `ToString()`) before using it in the template.