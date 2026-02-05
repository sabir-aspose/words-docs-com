---
title: Work with Office Add-ins in C++
second_title: Aspose.Words for C++
articleTitle: Work with Office Add-ins
linktitle: Work with Office Add-ins
description: "Aspose.Words for C++ provides various classes for working with Office Add-ins. You can add Task Pane via web extension and customize the pane and extension properties."
type: docs
weight: 50
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cpp/work-with-office-add-ins/
aliases: [/cpp/working-with-web-extensions/]
timestamp: 2024-01-27-14-07-04
---

Sometimes you might want to give access to interface controls that run code to modify documents. Aspose.Words API provides the `WebExtensions` namespace, which grants various classes to customize elements and attributes extending the XML vocabulary for representing Office Add-ins.

WebExtensions namespace can be conditionally divided into:

* Objects for working with the task pane
* Objects for working with web extensions

## Using Task Panes

The the task panes are interface surfaces that are displayed on the right side of the window in Microsoft Word. Task pane allows users to access interface controls that can run code to modify documents.

For example, using Aspose.Words API, you can add a task pane add‑in and customize its appearance.

## Using Web Extensions

Web Extensions are tools that expand the capabilities of Office applications and interact with Office document content. Web Extensions provide additional functionality to Office clients for improving user experience.

Aspose.Words provides the ability to add Web Extensions of the Task Pane type using the [WebExtension](https://reference.aspose.com/words/cpp/aspose.words.webextensions/webextension/) and [TaskPane](https://reference.aspose.com/words/cpp/aspose.words.webextensions/taskpane/) classes, and also allows you to customize the pane and extension properties.

The following code example shows how to create task panes and add to web extension task panes with basic properties: 

{{< gist "aspose-words-gists" "d55d8631947d283b1f0da99afa06c492" "cpp-Programming-Documents-Document-WorkingWithWebExtension-UsingWebExtensionTaskPanes.cpp" >}}

To see a list of task pane add‑ins, use the [WebExtensionTaskPanes](https://reference.aspose.com/words/cpp/aspose.words/document/get_webextensiontaskpanes/) property.

The following code example shows how to get such a list of add‑ins:

{{< gist "aspose-words-gists" "d55d8631947d283b1f0da99afa06c492" "cpp-Programming-Documents-Document-WorkingWithWebExtension-GetListOfAddins.cpp" >}}

------ 

## FAQ

1. **Q:** How do I add a task pane add‑in to a Word document using C++?  
   **A:** Create a `WebExtension` object, instantiate a `TaskPane` with the desired properties (e.g., `Id`, `Title`, `Visible`), add the task pane to the web extension via `WebExtension::AddTaskPane`, and then attach the web extension to the document with `Document::AddWebExtension`. The API handles the underlying XML for the Office add‑in.

2. **Q:** How can I retrieve the list of task pane add‑ins that are already attached to a document?  
   **A:** Use the `Document::GetWebExtensionTaskPanes()` method, which returns a collection of `WebExtensionTaskPane` objects. Iterate over the collection to read properties such as `Id`, `Title`, and `Visible`.

3. **Q:** Which properties can I customize for a task pane when creating it?  
   **A:** You can set properties like `Id`, `Title`, `Visible`, `DockState`, `Width`, and `Height` on the `TaskPane` object. These values control how the pane appears in Word and whether it is shown by default.

4. **Q:** Do I need a license to use the WebExtensions API in Aspose.Words for C++?  
   **A:** Yes. All Aspose.Words features, including WebExtensions, require a valid Aspose.Words for C++ license. Apply the license at the start of your application using `License license; license.SetLicense("Aspose.Words.CPP.lic");`.

5. **Q:** Can I add multiple task pane add‑ins to the same document?  
   **A:** Absolutely. Create a separate `TaskPane` instance for each add‑in, add each to the same `WebExtension`, and then attach the web extension to the document. Each pane will appear as an individual task pane in Word.