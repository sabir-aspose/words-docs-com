---  
title: Clone a Document in Node.js  
second_title: Aspose.Words for Node.js via .NET  
articleTitle: Clone a Document  
linktitle: Clone a Document  
type: docs  
description: "Clone a document to get its identical copy using Node.js. When creating a copy, nodes and properties of the original document are cloned."  
weight: 70  
ai_search_scope: words_nodejs  
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"  
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"  
url: /nodejs-net/clone-a-document/  
timestamp: 2025-07-09-10-05-05  
---  

Cloning a document is the process of creating an identical copy of an original document, which can improve performance and save you from potential memory leaks.

This article will explain the main use cases of cloning a document and how to create a document clone using Aspose.Words.

## Operations with Cloning Documents  

The clone operation allows you to make the process of creating documents faster as you will not need to load and parse a document from a file every time.

After creating a clone of your document, you will be able to edit it and perform different operations on it, for example, compare it with the original document, append or insert it into another document. You can also modify cloned elements or their content before inserting them into another document.

## Creating a Document Clone  

Aspose.Words allows you to clone a document using the [clone](https://reference.aspose.com/words/nodejs-net/aspose.words/document/clone/) method that performs a deep copy of the document and returns it. In other words, it will get a full copy of the DOM. The [clone](https://reference.aspose.com/words/nodejs-net/aspose.words/document/clone/) method speeds up the documents generation, and you only need one line of code to get a copy of your document.

Cloning produces a new document with the same contents as the original, but with a unique copy of each of the original document's nodes. You can also apply the clone operation to a document node by using the node [clone](https://reference.aspose.com/words/nodejs-net/aspose.words/document/clone/) method, which allows you to duplicate composite document nodes with and without their child nodes.

{{% alert color="primary" %}}

Note that when applying the cloning method all document properties will be cloned.

{{% /alert %}}

The following code example shows how to clone a document and create a duplicate of a section in that document:

{{< gist "aspose-words-gists" "4140b2f1857750e685e7bf1b2d9ba8dd" "clone-document.js" >}}

------  

## FAQ  

1. **Q:** How do I clone an entire document in Node.js?  
   **A:** Use the `Document.clone()` method. It creates a deep copy of the document, including all nodes, styles, and document properties, and returns a new `Document` instance that can be edited independently of the original.  

2. **Q:** Can I clone only a specific node, such as a section or paragraph?  
   **A:** Yes. Any node that derives from `Node` (e.g., `Section`, `Paragraph`) provides a `clone()` method. Calling `section.clone()` returns a new `Section` object that can be inserted into another document.  

3. **Q:** Does cloning copy custom document properties and built‑in settings?  
   **A:** The clone operation performs a deep copy, so all built‑in properties (e.g., page setup, headers/footers) and custom document properties are duplicated in the new document.  

4. **Q:** Is the cloning operation thread‑safe?  
   **A:** Cloning itself is safe, but the source `Document` should not be modified concurrently while the clone is being created. Ensure exclusive access to the original document during the clone call.  

5. **Q:** After cloning, can I modify the clone without affecting the original document?  
   **A:** Absolutely. The cloned document is a separate object with its own node tree. Any changes you make to the clone (e.g., inserting sections, editing text) will not impact the original document.  