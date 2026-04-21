---
title: Clean Up a Document in C#
second_title: Aspose.Words for .NET
articleTitle: Clean Up a Document
linktitle: Clean Up a Document
description: "Remove unused or duplicate information to reduce output size and processing time using C#. Remove unused styles, unused built-in styles, duplicate styles, or unused lists."
type: docs
weight: 30
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/clean-up-a-document/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

## Purpose Summary

This page outlines how to clean up unnecessary or redundant content in a Word document using Aspose.Words.

{{% /alert %}}

Sometimes you may need to remove unused or duplicate information to reduce the size of the output document and processing time.

While you can find and remove unused data, such as styles or lists, or duplicate information manually, it will be much more convenient to do this using features and capabilities provided by Aspose.Words.

The [CleanupOptions](https://reference.aspose.com/words/net/aspose.words/cleanupoptions/) class allows you to specify options for document cleaning. To remove duplicate styles or just unused styles or lists from the document, you can use the [Cleanup](https://reference.aspose.com/words/net/aspose.words/document/cleanup/) method.

## Remove Unused Information from a Document

You can use the [UnusedStyles](https://reference.aspose.com/words/net/aspose.words/cleanupoptions/unusedstyles/) and [UnusedBuiltinStyles](https://reference.aspose.com/words/net/aspose.words/cleanupoptions/unusedbuiltinstyles/) properties to detect and remove styles that are marked as "unused".

You can use the [UnusedLists](https://reference.aspose.com/words/net/aspose.words/cleanupoptions/unusedlists/) property to detect and remove lists and list definitions that are marked as "unused".

The following code example shows how to remove only unused styles from a document:

{{< gist "aspose-words-gists" "669f3d08f45b14f75f9d2cb17fa1056a" "cleanup-unused-styles-and-lists.cs" >}}

## Remove Duplicate Information from a Document

You can also use the [DuplicateStyle](https://reference.aspose.com/words/net/aspose.words/cleanupoptions/duplicatestyle/) property to substitute all duplicate styles with the original one and remove duplicates from a document.

The following code example shows how to remove duplicate styles from a document:

{{< gist "aspose-words-gists" "669f3d08f45b14f75f9d2cb17fa1056a" "cleanup-duplicate-style.cs" >}}

------  

## FAQ
1. **Q:** How can I remove only the unused styles from a document?  
   **A:** Create a `CleanupOptions` instance, set `UnusedStyles` to `true`, and call `document.Cleanup(options)`. This removes styles that are not applied anywhere in the document while leaving used styles intact.

2. **Q:** What is the difference between `UnusedBuiltinStyles` and `UnusedStyles`?  
   **A:** `UnusedBuiltinStyles` targets the built‑in Word styles (e.g., Normal, Heading 1) that are not used, whereas `UnusedStyles` applies to custom styles defined in the document. Enabling both removes all unused style definitions.

3. **Q:** Can I clean up duplicate styles in a single operation?  
   **A:** Yes. Set the `DuplicateStyle` property of `CleanupOptions` to `true` and invoke `document.Cleanup(options)`. Aspose.Words will replace duplicate style definitions with a single original style and delete the duplicates.