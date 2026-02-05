---
title: Clean Up a Document in Node.js
second_title: Aspose.Words for Node.js via .NET
articleTitle: Clean Up a Document
linktitle: Clean Up a Document
description: "Remove unused or duplicate information to reduce output size and processing time using Node.js. Remove unused styles, unused built-in styles, duplicate styles, or unused lists."
type: docs
weight: 30
ai_search_scope: words_nodejs
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nodejs-net/clean-up-a-document/
timestamp: 2025-07-09-10-05-05
---

Sometimes you may need to remove unused or duplicate information to reduce the size of the output document and processing time.

While you can find and remove unused data, such as styles or lists, or duplicate information manually, it will be much more convenient to do this using features and capabilities provided by Aspose.Words.

The [CleanupOptions](https://reference.aspose.com/words/nodejs-net/aspose.words/cleanupoptions/) class allows you to specify options for document cleaning. To remove duplicate styles or just unused styles or lists from the document, you can use the [cleanup](https://reference.aspose.com/words/nodejs-net/aspose.words/document/cleanup/) method.

## Remove Unused Information from a Document

You can use the [unusedStyles](https://reference.aspose.com/words/nodejs-net/aspose.words/cleanupoptions/unusedstyles/) and [unusedBuiltinStyles](https://reference.aspose.com/words/nodejs-net/aspose.words/cleanupoptions/unusedbuiltinstyles/) properties to detect and remove styles that are marked as "unused".

You can use the [unusedLists](https://reference.aspose.com/words/nodejs-net/aspose.words/cleanupoptions/unusedlists/) property to detect and remove lists and list definitions that are marked as "unused".

The following code example shows how to remove only unused styles from a document:

{{< gist "aspose-words-gists" "c2ead2f41ca20b28eac045c61a41279e" "cleanup-unused-styles-and-lists.js" >}}

## Remove Duplicate Information from a Document

You can also use the [duplicateStyle](https://reference.aspose.com/words/nodejs-net/aspose.words/cleanupoptions/duplicatestyle/) property to substitute all duplicate styles with the original one and remove duplicates from a document.

The following code example shows how to remove duplicate styles from a document:

{{< gist "aspose-words-gists" "c2ead2f41ca20b28eac045c61a41279e" "cleanup-duplicate-style.js" >}}

------ 

## FAQ

1. **Q:** How can I remove unused built‑in styles without affecting custom styles?  
   **A:** Set `CleanupOptions.unusedBuiltinStyles` to `true` while leaving `CleanupOptions.unusedStyles` as `false`. This tells the `Document.cleanup` method to target only the built‑in styles that are not referenced in the document, preserving all custom styles you have defined.

2. **Q:** Can I clean up unused lists but keep list definitions that are used later in the document?  
   **A:** Yes. Enable `CleanupOptions.unusedLists` before calling `Document.cleanup`. The method will delete only those list definitions that have no references; any list that is used anywhere in the document remains intact.

3. **Q:** What does the `duplicateStyle` option do, and when should I use it?  
   **A:** When `CleanupOptions.duplicateStyle` is set to `true`, Aspose.Words replaces every duplicate style with the first occurrence of that style and then removes the duplicates. Use this option when you suspect the document contains many identical style definitions that increase file size unnecessarily.

4. **Q:** I enabled cleanup options but the document size did not change. Why?  
   **A:** The cleanup operation only removes items that are truly unused or duplicated. If the document already has no unused styles, lists, or duplicate styles, the size will remain the same. Verify the options you have enabled and inspect the document to ensure there are removable elements.

5. **Q:** Is it safe to run `Document.cleanup` on a document that contains tracked changes?  
   **A:** Yes. The cleanup process works on the underlying document structure and does not interfere with revision tracking. However, if you also need to remove revisions, call `Document.acceptAllRevisions` before or after cleanup as required.