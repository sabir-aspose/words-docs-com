---
title: Working with TextBoxes in Node.js
second_title: Aspose.Words for Node.js via .NET
articleTitle: Working with TextBoxes
linktitle: Working with TextBoxes
description: "Work with textboxes in a document using Node.js."
type: docs
weight: 250
ai_search_scope: words_nodejs
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nodejs-net/working-with-textboxes/
timestamp: 2025-07-09-10-05-05
---

In Aspose.Words, [TextBox](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/textbox/) class is used to specify how a text is displayed inside a shape. It provides a public property named as [parent](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/textbox/parent/) to get the parent shape for the text box to allow customer to find linked [Shape](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shape/) from linked [TextBox](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/textbox/).

## Creating a Link

[TextBox](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/textbox/) class provides [isValidLinkTarget](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/textbox/isValidLinkTarget/) method in order to check whether the [TextBox](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/textbox/) can be linked to the target Textbox.

The following code example shows how to check if the `TextBox` can be linked to the target Textbox:

{{< gist "aspose-words-gists" "e78f2e5545401312af45ab0be0f09bb2" "create-link.js" >}}

## Check TextBox Sequence

There are several ways to display text in a shape. The [textBox](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shape/textBox/) can be the Head, Middle, or Tail of a sequence.

The following code example shows how to check if **TextBox** is a Head, Tail, or Middle of the sequence:

{{< gist "aspose-words-gists" "e78f2e5545401312af45ab0be0f09bb2" "check-sequence.js" >}}

## Breaking a Link

Using the [textBox](https://reference.aspose.com/words/nodejs-net/aspose.words.drawing/shape/textBox/) method you can break the link to the next **TextBox**.

The following code example shows how to break a link for a **TextBox**:

{{< gist "aspose-words-gists" "e78f2e5545401312af45ab0be0f09bb2" "break-link.js" >}}
