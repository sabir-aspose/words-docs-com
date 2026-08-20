---
title: Asian Typography in C#
second_title: Aspose.Words for .NET
articleTitle: Working with Asian Typography
linktitle: Working with Asian Typography
description: "Work with Asian typography using C#. Adjust Space between Asian and Latin text in C#."
type: docs
weight: 240
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/working-with-asian-typography/
timestamp: 2024-02-01-16-17-05
---

{{% alert color="grey" %}}

## Purpose Summary

This page explains how to work with Asian typography features such as line breaking and character spacing.

{{% /alert %}}

Asian Typography is a set of options for text paragraphs in documents written in Asian languages.

Aspose.Words supports Asian Typography using the [ParagraphFormat](https://reference.aspose.com/words/net/aspose.words/paragraphformat/) class and some of its properties.

## Automatically Adjust Space between Asian and Latin Text or Numbers

If you are designing a template with both East Asian and Latin text and  want to enhance the appearance of your form template by controlling the spaces between both types of text, you can configure your form template to automatically adjust the spaces between these two types of text. To achieve this, you can use [AddSpaceBetweenFarEastAndAlpha](https://reference.aspose.com/words/net/aspose.words/paragraphformat/addspacebetweenfareastandalpha/) and [AddSpaceBetweenFarEastAndDigit](https://reference.aspose.com/words/net/aspose.words/paragraphformat/addspacebetweenfareastanddigit/) properties of the `ParagraphFormat` class.

The following code example shows how to use **AddSpaceBetweenFarEastAndAlpha** and **AddSpaceBetweenFarEastAndDigit** properties:

{{< gist "aspose-words-gists" "4f54ffd5c7580f0d146b53e52d986f38" "space-between-asian-and-latin-text.cs" >}}

## Set Line Break Options

The Asian Typography tab of the paragraph properties dialog box in Microsoft Word has line break group. The options of this group can be set using the [FarEastLineBreakControl](https://reference.aspose.com/words/net/aspose.words/paragraphformat/fareastlinebreakcontrol/), [WordWrap](https://reference.aspose.com/words/net/aspose.words/paragraphformat/wordwrap/), [HangingPunctuation](https://reference.aspose.com/words/net/aspose.words/paragraphformat/hangingpunctuation/) properties of the **ParagraphFormat** class.

The following code example shows how to use these properties:

{{< gist "aspose-words-gists" "4f54ffd5c7580f0d146b53e52d986f38" "asian-typography-line-break-group.cs" >}}

## Related APIs

- [ParagraphFormat](https://reference.aspose.com/words/net/aspose.words/paragraphformat/)