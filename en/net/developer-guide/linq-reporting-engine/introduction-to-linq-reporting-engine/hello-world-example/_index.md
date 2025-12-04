---
title: Hello World Example in C#
second_title: Aspose.Words for .NET
articleTitle: Hello World Example
linktitle: Hello World Example
description: "Create Hello world example to start working with LINQ Reporting Engine to build a report in C#."
type: docs
weight: 30
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/hello-world-example/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*What is this page about?*

This page explains the “Hello World” example as the simplest introduction to Aspose.Words.

{{% /alert %}}

{{% alert color="primary" %}}

A "Hello, World" example is traditionally used to introduce features of a programming language or software with a simple use case. Here is the example for LINQ Reporting Engine.

{{% /alert %}}

Assume that you have the `Sender` class defined in your application as follows:

{{< gist "aspose-words" "9a306a41bb6aea8adfcabf5a575c5718" "Examples-CSharp-LINQ-Sender-Sender.cs" >}}

To produce a report containing a message of a concrete sender on its behalf, you can use a template document with the following content.

{{< highlight csharp >}}
<<[s.Name]>> says: "<<[s.Message]>>."
{{< /highlight >}}

To build a report from the template, you can use the following source code.

{{< gist "aspose-words" "9a306a41bb6aea8adfcabf5a575c5718" "Examples-CSharp-LINQ-HelloWorld-HelloWorld.cs" >}}

After the source code is executed, the template document is populated with the data about the sender, and the document becomes a ready report with the following content.

{{< highlight csharp >}}
LINQ Reporting Engine says: "Hello, World."
{{< /highlight >}}

After the report document is built, you can save it or perform any other tasks on it using [Aspose.Words API](https://reference.aspose.com/words/net/) in your code.
