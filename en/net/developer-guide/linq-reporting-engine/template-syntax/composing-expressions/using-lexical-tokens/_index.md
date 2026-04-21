---
title: Using Lexical Tokens in C#
second_title: Aspose.Words for .NET
articleTitle: Using Lexical Tokens
linktitle: Using Lexical Tokens
description: "Use lexical tokens in template expressions when building a report in C#."
type: docs
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/using-lexical-tokens/
timestamp: 2024-10-21-11-17-44
---

{{% alert color="grey" %}}

## Purpose Summary

This page explains how lexical tokens work within template expressions.

{{% /alert %}}

The following table describes lexical tokens that you can use in template expressions and restrictions on these tokens’ usage comparing with C# Language Specification 5.0.

| Token | Restrictions |
| :- | :- |
| **Keyword** | Only the following tokens are reserved as keywords: `true`, `false`, `null`, `new`, and `in`. |
| **Identifier** | - The feature of keyword escaping through the “@” character is not supported.<br>- Unicode character escapes are not permitted in identifiers. |
| **Literal** | None. |
| **Operator** | See “Using Operators.” |

You can use the following identifiers that are not preceded by a member access operator in template expressions:

- The name of a passed data source object
- The name of an iteration variable within its scope (see “Outputting Sequential Data” for more information)
- The name of a common variable after it is declared (see “Using Variables” for more information)
- The name of a lambda function parameter within the scope of the lambda function
- A fully or partially qualified name of a type that is known by the engine (see “Setting up Known External Types” for more information)
- The name of a member of an object that is determined as follows: 
  - Inside a data band body, the object is resolved to the innermost iteration variable.
  - Outside a data band body, the object is resolved to a passed data source.

The feature of the omitting of an object identifier while accessing the object’s members is also known as the contextual object member access. See “Using Contextual Object Member Access” for more information.

------ 

## FAQ

1. **Q:** Which keywords are reserved in template expressions?  
   **A:** Only `true`, `false`, `null`, `new`, and `in` are treated as reserved keywords. All other identifiers can be used freely.

2. **Q:** Can I escape a reserved keyword with the “@” character in a template expression?  
   **A:** No. The “@” keyword‑escaping syntax that exists in C# is not supported in Aspose.Words template expressions. Use a different identifier name instead.

3. **Q:** Are Unicode escape sequences allowed in identifiers?  
   **A:** No. Identifiers must be written using literal Unicode characters; escape sequences such as `\uXXXX` are not permitted.

4. **Q:** How do I access a member of the current data object without writing the object name?  
   **A:** Use contextual object member access. Inside a data band the engine resolves the member to the innermost iteration variable; outside a data band it resolves to the passed data source object.

5. **Q:** Where can I find the list of operators that are valid in template expressions?  
   **A:** The supported operators are documented in the “Using Operators” section of the reporting engine guide. Common arithmetic (`+`, `-`, `*`, `/`), comparison (`==`, `!=`, `<`, `>`, `<=`, `>=`), logical (`&&`, `||`, `!`) and other operators are available there.