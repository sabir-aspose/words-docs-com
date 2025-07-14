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

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Document-working_with_document_options_and_settings-CleanupUnusedStylesandLists.py" >}}

## Remove Duplicate Information from a Document

You can also use the [duplicateStyle](https://reference.aspose.com/words/nodejs-net/aspose.words/cleanupoptions/duplicatestyle/) property to substitute all duplicate styles with the original one and remove duplicates from a document.

The following code example shows how to remove duplicate styles from a document:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Document-working_with_document_options_and_settings-CleanupDuplicateStyle.py" >}}
