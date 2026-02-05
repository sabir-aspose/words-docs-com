---
title: Using Extension Methods in Java
second_title: Aspose.Words for Java
articleTitle: Using Extension Methods
linktitle: Using Extension Methods
description: "Use extension methods in template expressions when building a report in Java."
type: docs
weight: 40
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /java/using-extension-methods/
timestamp: 2024-01-27-14-07-04
---

LINQ Reporting Engine enables you to use the following built-in extension methods in template expressions:

- Extension methods mimicking the ones for `IEnumerable<T>` (see "Appendix A. Enumeration Extension Methods" for more information)
- Extension methods for iteration variables (see "Using Extension Methods of Iteration Variables" for more information)

------ 

## FAQ

1. **Q:** How do I call an extension method inside a LINQ Reporting Engine template?  
   **A:** Use the standard tag syntax and place the method after the variable, e.g., `<<item.Where(p => p.Age > 30)>>`. The engine resolves the method at runtime and returns the filtered collection.

2. **Q:** Which enumeration‑style extension methods are available by default?  
   **A:** Methods that exist on `IEnumerable<T>` such as `Where`, `Select`, `OrderBy`, `Take`, `Skip`, `Count`, and `Any` are provided out‑of‑the‑box for use in template expressions.

3. **Q:** Can I use extension methods on the iteration variable itself (e.g., the index of a `foreach` loop)?  
   **A:** Yes. The engine supplies helpers like `Index`, `IsFirst`, `IsLast`, and `IsEven` that can be called directly on the iteration variable, for example `<<item.IsFirst>>`.

4. **Q:** Is it possible to add my own custom extension methods for use in Java templates?  
   **A:** Custom extension methods are not supported in the template language. Only the built‑in methods listed in the documentation can be used.

5. **Q:** Are the same extension methods available when using Aspose.Words for .NET or other platforms?  
   **A:** The set of built‑in extension methods is consistent across platforms, but the exact syntax may differ (e.g., C# uses `{{ }}` while Java uses `<< >>`). Refer to the platform‑specific documentation for details.