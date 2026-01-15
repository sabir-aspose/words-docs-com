---
title: Clean Up a Document in Python
second_title: Aspose.Words for Python via .NET
articleTitle: Clean Up a Document
linktitle: Clean Up a Document
description: "Remove unused or duplicate information to reduce output size and processing time using Python. Remove unused styles, unused built-in styles, duplicate styles, or unused lists."
type: docs
weight: 30
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/clean-up-a-document/
aliases: [/python/clean-up-a-document/]
timestamp: 2024-01-27-14-07-04
---

Sometimes you may need to remove unused or duplicate information to reduce the size of the output document and processing time.

While you can find and remove unused data, such as styles or lists, or duplicate information manually, it will be much more convenient to do this using features and capabilities provided by Aspose.Words.

The [CleanupOptions](https://reference.aspose.com/words/python-net/aspose.words/cleanupoptions/) class allows you to specify options for document cleaning. To remove duplicate styles or just unused styles or lists from the document, you can use the [cleanup](https://reference.aspose.com/words/python-net/aspose.words/document/cleanup/) method.

## Remove Unused Information from a Document

You can use the [unused_styles](https://reference.aspose.com/words/python-net/aspose.words/cleanupoptions/unused_styles/) and [unused_builtin_styles](https://reference.aspose.com/words/python-net/aspose.words/cleanupoptions/unused_builtin_styles/) properties to detect and remove styles that are marked as "unused".

You can use the [unused_lists](https://reference.aspose.com/words/python-net/aspose.words/cleanupoptions/unused_lists/) property to detect and remove lists and list definitions that are marked as "unused".

The following code example shows how to remove only unused styles from a document:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Document-working_with_document_options_and_settings-CleanupUnusedStylesandLists.py" >}}

## Remove Duplicate Information from a Document

You can also use the [duplicate_style](https://reference.aspose.com/words/python-net/aspose.words/cleanupoptions/duplicate_style/) property to substitute all duplicate styles with the original one and remove duplicates from a document.

The following code example shows how to remove duplicate styles from a document:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Document-working_with_document_options_and_settings-CleanupDuplicateStyle.py" >}}

```

------ 

## FAQ

1. **Q:** How can I remove unused styles from a Word document using Aspose.Words for Python?  
   **A:** Create a `CleanupOptions` instance, set its `unused_styles` (and optionally `unused_builtin_styles`) property to `True`, and call `Document.cleanup(options)`. The method scans the document and deletes any style that is not referenced.

2. **Q:** What is the purpose of the `duplicate_style` option?  
   **A:** When `duplicate_style` is set to `True`, Aspose.Words replaces every duplicate style with the first occurrence of that style and then removes the redundant definitions, reducing file size and simplifying style management.

3. **Q:** Can the cleanup operation also delete unused lists?  
   **A:** Yes. Set the `unused_lists` property of `CleanupOptions` to `True` before invoking `Document.cleanup`. This removes list definitions that are not used anywhere in the document.

4. **Q:** Does the cleanup process affect content in headers, footers, or footnotes?  
   **A:** Cleanup examines the entire document, including headers, footers, footnotes, and endnotes. Unused styles or lists that are only referenced in those sections will be retained; otherwise, they will be removed.

5. **Q:** How can I verify which styles or lists were removed after cleanup?  
   **A:** After calling `cleanup`, you can iterate through `Document.styles` or `Document.lists` to see the remaining items. Comparing the counts before and after the operation gives a quick indication of what was removed.