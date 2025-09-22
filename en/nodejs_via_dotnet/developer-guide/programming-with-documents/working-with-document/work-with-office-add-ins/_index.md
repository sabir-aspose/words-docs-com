---
title: Work with Office Add-ins in Node.js
second_title: Aspose.Words for Node.js via .NET
articleTitle: Work with Office Add-ins
linktitle: Work with Office Add-ins
description: "Aspose.Words for Node.js via .NET provides various classes for working with Office Add-ins. You can add Task Pane via web extension and customize the pane and extension properties."
type: docs
weight: 50
ai_search_scope: words_nodejs
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nodejs-net/work-with-office-add-ins/
timestamp: 2025-07-09-10-05-05
---

Sometimes you might want to give access to interface controls that run code to modify documents. Aspose.Words API provides the [webextensions](https://reference.aspose.com/words/nodejs-net/aspose.words.webextensions/) module, which grants various classes to customize elements and attributes extending the XML vocabulary for representing Office Add-ins.

WebExtensions namespace can be conditionally divided into:

* Objects for working with the task pane
* Objects for working with web extensions

## Using Task Panes

The task panes are interface surfaces that are displayed on the right side of the window in Microsoft Word. Task pane allows users to access interface controls that can run code to modify documents.

For example, using Aspose.Words API, you can add a task pane add-in and customize its appearance.

## Using Web Extensions

Web Extensions are tools that expand the capabilities of Office applications and interact with Office document content. Web Extensions provide additional functionality to Office clients for improving user experience.

Aspose.Words provides the ability to add Web Extensions of the Task Pane type using the [WebExtension](https://reference.aspose.com/words/nodejs-net/aspose.words/webextension/) and [TaskPane](https://reference.aspose.com/words/nodejs-net/aspose.words.webextensions/taskpane/) classes, and also allows you to customize the pane and extension properties.

The following code example shows how to create task panes and add to web extension task panes with basic properties: 

{{< gist "aspose-words-gists" "8c31c018ea71c92828223776b1a113f7" "web-extension-task-panes.cs" >}}

To see a list of task pane add-ins, use the [webExtensionTaskPanes](https://reference.aspose.com/words/nodejs-net/aspose.words/document/webextensiontaskpanes/) property.

The following code example shows how to get such a list of add-ins:

{{< gist "aspose-words-gists" "8c31c018ea71c92828223776b1a113f7" "get-list-of-addins.cs" >}}
