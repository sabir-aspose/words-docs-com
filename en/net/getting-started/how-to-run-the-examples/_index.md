---
title: How to Run the Examples
second_title: Aspose.Words for .NET
articleTitle: How to Run the Examples
linktitle: How to Run the Examples
description: "Download Aspose.Words for .NET examples from our GitHub repository and learn how to run them to become more familiar with the Aspose.Words possibilities and features using C#."
type: docs
weight: 110
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/how-to-run-the-examples/
timestamp: 2024-10-24-11-44-28
---

{{% alert color="grey" %}}

## Purpose Summary

This page describes how to run the provided examples.

{{% /alert %}}

To become more familiar with the Aspose.Words possibilities and features we provide examples that can be downloaded from our GitHub repository, run, and learn in detail.

In this article, you can find the system requirements, as well as information on how to run the examples.

## Software Requirements and Prerequisites

Please make sure you meet the following requirements before downloading and running the examples:

1. Visual Studio Code, Visual Studio 2019.
2. Installed NuGet Package Manager and the latest NuGet API version for Visual Studio.
3. Selected **nuget.org** option in the “Tools → Options" dialog box under "NuGet Package Manager → Package Sources”.
4. An active Internet connection to use the `NuGet` Automatic Package Restore feature in the Examples project. If you do not have an active Internet connection on the machine where the examples are to be executed, check the article [Installation](/words/net/installation/) and manually add a reference to `Aspose.Words.dll` to the Examples project.

## Download and Run the Examples

All Aspose.Words for .NET examples are hosted on [GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET). You can either clone the repository using your favorite GitHub client or download [the ZIP file](https://github.com/aspose-words/Aspose.Words-for-.NET/archive/master.zip).

After getting a copy of the repository, you may find that:

- All the examples are located in the **Examples** folder.
- There are Visual Studio solution files for C# and Xamarin created in Visual Studio 2019.

To run the examples, open the solution file in Visual Studio and build the project:

- For **API Reference** examples, the structure is based on class names, for **Docs** examples it is mostly based on the [Developer Guiled](/words/net/developer-guide/) documentation section.
- On the first run, the dependencies will be automatically downloaded via NuGet.
- The **Data** folder at the root folder of **Examples** contains input files that were used in the examples.
- All examples can be run as unit tests.

{{% alert color="primary" %}}

Please feel free to reach out using our [Aspose.Words Product Family Forum](https://forum.aspose.com/c/words/8) if you have any issues setting up or running the examples.

{{% /alert %}}

## Contribute to Improving the Examples

If you like to add or improve an example, we encourage you to contribute to the project. All examples and showcase projects in this repository are open source and can be freely used in your applications.

You can fork the repository, edit the source code, and create a pull request to contribute. We will review the changes and include them in the repository if found helpful.

## See Also

- [Details on how to install NuGet Package Manager](https://docs.microsoft.com/nuget/guides/install-nuget)

------

## FAQ

1. **Q:** Do I need an Aspose.Words license to run the example projects?  
   **A:** No. The examples are shipped with a temporary evaluation license, so they can be built and executed without a purchased license. If you add your own license file to the project, the examples will run with full functionality and without evaluation restrictions.

2. **Q:** How can I run the examples on a machine that has no Internet connection?  
   **A:** First, download the repository and the required NuGet packages on a machine with Internet access. Then copy the entire `packages` folder (or the `Aspose.Words.dll` file) to the offline machine and add a reference to the DLL manually in the project. After that you can build and run the examples without needing to restore packages online.

3. **Q:** Can I run the examples with .NET 8 or Visual Studio 2022?  
   **A:** Yes. Open the solution in Visual Studio 2022, change the target framework of the example projects to `.NET 8.0` (or any later supported version), restore NuGet packages, and rebuild. The code is compatible with newer .NET versions, but some older sample projects may reference legacy APIs that need minor adjustments.

4. **Q:** Why do I get an “Unable to locate package Aspose.Words” error when building the solution?  
   **A:** This usually means the NuGet source `nuget.org` is not enabled or the machine cannot reach the internet. Verify that `nuget.org` is selected in **Tools → Options → NuGet Package Manager → Package Sources** and that the network allows access to `https://api.nuget.org/v3/index.json`. If you are behind a proxy, configure the proxy settings in Visual Studio or restore the packages manually as described above.