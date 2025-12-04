---
title: Working with Types in Java
second_title: Aspose.Words for Java
articleTitle: Working with Types
linktitle: Working with Types
description: "Use external visible types in template expressions when building a report in Java."
type: docs
weight: 20
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /java/working-with-types/
timestamp: 2024-01-27-14-07-04
---

LINQ Reporting Engine enables you to use external visible types in template expressions. A *visible* type is a public type which outer types (if any) are public as well. You can use a data source object of any visible type to pass it to the engine.

However, you can use the identifier of a visible type in template expressions only if the following additional requirements are met:

- The type is not void.
- The type does not represent an array.
- The type identifier does not contain generic type arguments.

Also, the engine enables you to use anonymous types in template expressions. Such types are useful while composing expressions with grouping by multiple keys. See “Appendix A. Enumeration Extension Methods” for the examples.
