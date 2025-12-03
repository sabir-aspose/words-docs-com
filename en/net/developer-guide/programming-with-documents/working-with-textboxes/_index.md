---
title: Working with TextBoxes in C#
second_title: Aspose.Words for .NET
articleTitle: Working with TextBoxes
linktitle: Working with TextBoxes
description: "Introduction to linked textboxes feature in Aspose.Words for .NET."
type: docs
weight: 250
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /net/working-with-textboxes/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*What is this page about?*

This page explains how to work with textboxes in documents.

{{% /alert %}}

In Aspose.Words, the [TextBox](https://reference.aspose.com/words/net/aspose.words.drawing/textbox/) class is used to specify how text is displayed inside a shape. It exposes a public property named **Parent** to get the parent shape for the text box so that the customer can find the linked [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/) from the associated **TextBox**.

## Creating a Link

The **TextBox** class provides [IsValidLinkTarget](https://reference.aspose.com/words/net/aspose.words.drawing/textbox/isvalidlinktarget/) method in order to check whether the **TextBox** can be linked to the target **Textbox**.

The following code example shows how to check if the `TextBox` can be linked to the target Textbox:

{{< gist "aspose-words-gists" "68b6041746b3d6bf5137cff8e6385b5f" "create-link.cs" >}}

## Check TextBox Sequence

There are several ways to display text in a shape. The [TextBox](https://reference.aspose.com/words/net/aspose.words.drawing/shape/textbox/) can be the Head, Middle, or Tail of a sequence.

The following code example shows how to check if **TextBox** is a Head, Tail, or Middle of the sequence:

{{< gist "aspose-words-gists" "68b6041746b3d6bf5137cff8e6385b5f" "check-sequence.cs" >}}

## Breaking a Link

Using the [BreakForwardLink](https://reference.aspose.com/words/net/aspose.words.drawing/textbox/breakforwardlink/) method you can break the link to the next **TextBox**.

The following code example shows how to break a link for a **TextBox**:

{{< gist "aspose-words-gists" "68b6041746b3d6bf5137cff8e6385b5f" "break-link.cs" >}}
