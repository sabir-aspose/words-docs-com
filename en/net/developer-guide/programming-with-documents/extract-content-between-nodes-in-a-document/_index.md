---
title: How to Extract Content Between Document Nodes
second_title: Aspose.Words for .NET
articleTitle: Extract Content Between Nodes in a Document
linktitle: Extract Content Between Nodes
description: "Extracting document content in different using C#."
type: docs
weight: 140
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/how-to-extract-selected-content-between-nodes-in-a-document/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page describes how to extract selected content between nodes in a document.

{{% /alert %}}

When working with documents, it is important to be able to easily extract content from a specific range within a document. However, the content may consist of complex elements such as paragraphs, tables, images, etc.

Regardless of what content needs to be extracted, the method to extract that content will always be determined by which nodes are selected to extract content between. These can be entire text bodies or simple text runs.

There are many possible situations and therefore many different node types to consider when extracting content. For example, you might want to extract content between:

- Two specific paragraphs
- Specific runs of text
- Fields of various types, such as merge fields
- Start and end ranges of a bookmark or comment
- Various bodies of text contained in separate sections

In some situations, you may even need to combine different node types, such as extracting content between a paragraph and a field, or between a run and a bookmark.

This article provides the code implementation for extracting text between different nodes, as well as examples of common scenarios.

{{% alert color="primary" %}}

These examples are just a few demonstrations of the many possibilities. We plan for the text extraction functionality to be part of the public API in the future, and no extra code will be required. In the meantime, feel free to post your requests regarding this functionality on the [Aspose.Words forum](https://forum.aspose.com/c/words/8).

{{% /alert %}}

## Why Extract Content

Often the goal of extracting the content is to duplicate or save it separately in a new document. For example, you can extract content and:

- Copy it into a separate document
- Convert a specific part of a document to PDF or image
- Duplicate the content in the document many times
- Work with extracted content separate from the rest of the document

This can be easily achieved using Aspose.Words and the code implementation below.

## Extracting Content Algorithm

The code in this section addresses all of the possible situations described above with one generalized and reusable method. The general outline of this technique involves:

1. Gathering the nodes which dictate the area of content that will be extracted from your document. Retrieving these nodes is handled by the user in their code, based on what they want to be extracted.
1. Passing these nodes to the **ExtractContent** method provided below. You must also pass a boolean parameter which states whether these nodes, acting as markers, should be included in the extraction or not.
1. Retrieving a list of cloned content (copied nodes) specified to be extracted. You can use this list of nodes in any applicable way, for example, creating a new document containing only the selected content.

## How to Extract Content

To extract the content from your document you need to call the **ExtractContent** method below and pass the appropriate parameters. The underlying basis of this method involves finding block level nodes (paragraphs and tables) and cloning them to create identical copies. If the marker nodes passed are block level then the method is able to simply copy the content on that level and add it to the array.

However if the marker nodes are inline (a child of a paragraph) then the situation becomes more complex, as it is necessary to split the paragraph at the inline node, be it a run, bookmark fields etc. Content in the cloned parent nodes not present between the markers is removed. This process is used to ensure that the inline nodes will still retain the formatting of the parent paragraph. The method will also run checks on the nodes passed as parameters and throws an exception if either node is invalid. The parameters to be passed to this method are:

1. **StartNode** and **EndNode**. The first two parameters are the nodes which define where the extraction of the content is to begin and to end at respectively. These nodes can be both block level ([Paragraph](https://reference.aspose.com/words/net/aspose.words/paragraph/) , [Table](https://reference.aspose.com/words/net/aspose.words.tables/table/)) or inline level (e.g [Run](https://reference.aspose.com/words/net/aspose.words/run/) , [FieldStart](https://reference.aspose.com/words/net/aspose.words.fields/fieldstart/) , [BookmarkStart](https://reference.aspose.com/words/net/aspose.words/bookmark/bookmarkstart/) etc.):
   1. To pass a field you should pass the corresponding **FieldStart** object
   1. To pass bookmarks, the **BookmarkStart** and [BookmarkEnd](https://reference.aspose.com/words/net/aspose.words/bookmark/bookmarkend/) nodes should be passed
   1. To pass comments, the [CommentRangeStart](https://reference.aspose.com/words/net/aspose.words.commentrangestart/) and [CommentRangeEnd](https://reference.aspose.com/words/net/aspose.words.commentrangeend/) nodes should be used
1. **IsInclusive**. Defines if the markers are included in the extraction or not. If this option is set to false and the same node or consecutive nodes are passed, then an empty list will be returned:
   1. If a **FieldStart** node is passed then this option defines if the whole field is to be included or excluded
   1. If a **BookmarkStart** or **BookmarkEnd** node is passed, this option defines if the bookmark is included or just the content between the bookmark range.
   1. If a **CommentRangeStart** or **CommentRangeEnd** node is passed, this option defines if the comment itself is to be included or just the content in the comment range.

The implementation of the **ExtractContent** method you can find [on Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/DocsExamples/DocsExamples/Programming%20with%20Documents/Contents%20Management/Extract%20content%20helper.cs). This method will be referred to in the scenarios in this article.

We will also define a custom method to easily generate a document from extracted nodes. This method is used in many of the scenarios below and simply creates a new document and imports the extracted content into it.

The following code example shows how to take a list of nodes and inserts them into a new document:

{{< gist "aspose-words-gists" "1f94e59ea4838ffac2f0edf921f67060" "generate-document.cs" >}}

## Extract Content Between Paragraphs

... (remaining content unchanged) ...

## Extract Images from Shapes

You may need to extract document images to perform some tasks. Aspose.Words allows you to do this as well.

The following code example shows how to extract images from a document:

{{< gist "aspose-words-gists" "1f94e59ea4838ffac2f0edf921f67060" "extract-images.cs" >}}

------ 

## FAQ

1. **Q:** How do I control whether the start and end marker nodes are included in the extracted content?  
   **A:** Pass a Boolean value to the `IsInclusive` parameter of the `ExtractContent` method. Set it to `true` to include the marker nodes (e.g., the whole field or bookmark), or `false` to exclude them and extract only the content between the markers.

2. **Q:** Can I extract content between nodes that belong to different sections of the document?  
   **A:** Yes. Retrieve the desired nodes from their respective sections (e.g., using `Document.GetChild` or `Section.FirstParagraph`) and pass those nodes to `ExtractContent`. The method works across sections as long as both nodes belong to the same `Document` instance.

3. **Q:** After extracting nodes, how can I obtain plain text without any formatting or control characters?  
   **A:** Create a new `Document`, import the extracted nodes, then either call `newDocument.GetText()` for raw text with control characters or `newDocument.Save(stream, SaveFormat.Text)` to get clean plain‑text output. Using `SaveFormat.Text` removes formatting and Word control characters.

4. **Q:** Why does `ExtractContent` throw an exception about invalid nodes?  
   **A:** This usually occurs when the start or end node is `null`, belongs to a different `Document`, or the start node appears after the end node in the document order. Verify that both nodes are non‑null, belong to the same document, and that the start node precedes the end node before calling the method.