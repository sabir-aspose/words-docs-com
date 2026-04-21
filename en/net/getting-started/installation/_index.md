---  
title: Installation  
second_title: Aspose.Words for .NET  
articleTitle: Installation  
linktitle: Installation  
description: "Install Aspose.Words for .NET using Visual Studio tools such as Manage NuGet Packages or Package Manager Console and the MSI installer. Use the Full Trust permission set in C#."  
type: docs  
weight: 10  
ai_search_scope: words_net  
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"  
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"  
url: /net/installation/  
timestamp: 2024-01-27-14-07-04  
---  

{{% alert color="grey" %}}

## Purpose Summary

This page describes installation steps for Aspose.Words.

{{% /alert %}}

Make sure your machine meets the [system requirements](/words/net/system-requirements/) before you begin.

This article explains how to install Aspose.Words for .NET on your computer.

## Install or Update Aspose.Words for .NET using Manage NuGet Packages {#install-or-update-aspose-words-for-net-using-nuget}

NuGet is the easiest way to download and install [Aspose.Words for .NET](https://www.nuget.org/packages/Aspose.Words/) APIs. To do this, follow these steps:

1. Open *Microsoft Visual Studio* and *Manage NuGet Packages* from the menu to open package manager
2. Search for "aspose" or "aspose.words" to find the desired Aspose API<br>
   <img src="aspose-words-nuget.png" alt="aspose-words-nuget" style="width:800px"/>
3. Select the desired Aspose API and click "Install"

The selected API will be downloaded and referenced in your project.

You can also update Aspose.Words for .NET to the desired version using *Manage NuGet Packages*.

## Install or Update Aspose.Words using Package Manager Console

You can also install or update Aspose.Words for .NET APIs using the *Package Manager Console*. To do this, follow these steps:

1. Open *Microsoft Visual Studio* and *Package Manager Console* from the menu to open package manager console<br>
   <img src="aspose-words-nuget-update.png" alt="aspose-words-nuget-update" style="width:600px"/>
2. Type the command `Install-Package Aspose.Words` and press Enter to install the latest full release into your application<br>
   <img src="aspose-words-nuget-update-2.png" alt="aspose-words-nuget-update-2" style="width:600px"/><br>
   {{% alert color="primary" %}}In addition, you can add the `-prerelease` suffix to the command to specify that the latest release, including hotfixes, should also be installed.{{% /alert %}}
3. Once downloaded, you will see confirmation messages<br>
   <img src="aspose-words-nuget-istalled.png" alt="aspose-words-nuget-istalled" style="width:600px"/><br>
   {{% alert color="primary" %}}If you are unfamiliar with the [Aspose EULA](https://about.aspose.com/legal/eula/), it is recommended to read the license referenced in the URL.{{% /alert %}}
4. Now you may find that Aspose.Words has been successfully added and referenced in your application for you<br>
   <img src="aspose-words-nuget-references.png" alt="aspose-words-nuget-references" style="width:400px"/>

In *Package Manager Console*, you can also use the `Update-Package Aspose.Words` command to check for updates to the Aspose.Words package and install them if present. You can also add the `-prerelease` suffix to update the latest release.

## Install Aspose.Words for .NET using Installer

Aspose.Words for .NET can be installed by direct downloading the MSI installer from the [downloads section](https://releases.aspose.com/words/).

{{% alert color="primary" %}}

You must be logged in to download the installer. If you are not registered yet, you can may sign up for free.

{{% /alert %}}

To Install Aspose.Words for .NET, follow these steps:

1. Download `Aspose.Words_{LatestVersion}.msi` from the [downloads section](https://releases.aspose.com/words/)
2. Doble-click the downloaded file, thereby starting the setup wizard, follow the setup wizard instructions<br>
   <img src="aspose-words-setup-1.png" alt="aspose-words-setup-1" style="width:500px"/>
3. When the setup wizard completes the installation, the required files will be available in the folder at the provided folder path<br>
   <img src="aspose-words-setup-4.jpg" alt="aspose-words-setup-4" style="width:500px"/>
4. Open your solution/project in Visual Studio
5. Right-click your project in *Solution Explorer* and add the reference to installed assemblies
6. Aspose.Words for .NET installed assemblies will appear in extensions under the Assemblies section – just select the required DLL component<br>
   <img src="aspose-words-setup-5.png" alt="aspose-words-setup-5" style="width:800px"/>
7. Finally, click OK

## Considerations When Running in a Shared Server Environment

All Aspose .NET components are recommended to run with the *Full Trust* permission set. This is because Aspose .NET component sometimes needs access to registry settings and files located in places other than the virtual directory, such as reading fonts. Furthermore, `Aspose.NET` components are based on core .NET system classes, some of which also require *Full Trust* permission to run in some cases.

Internet Service Providers hosting multiple applications from different companies mostly enforce *Medium Trust* security level. In the case of .NET 2.0, such a security level may impose the following constraints, which may affect the ability of Aspose.Words to perform properly:

- **RegistryPermission** is not available. This means that you cannot access the registry, which is required to enumerate installed fonts when rendering documents.
- **FileIOPermission** is restricted. This means that you can only access files in your application’s virtual directory hierarchy. This also potentially means fonts cannot be read during export.

For these reasons specified above, it is recommended to run Aspose.Words with Full Trust permissions. You may find that some of library features will work when performing different tasks with Medium trust, and some will not, for example, rendering. This can be related to GDI+ image processing calls.

------  

## FAQ

1. **Q:** How do I apply my Aspose.Words license after installing the library?  
   **A:** Add the license file (e.g., `Aspose.Words.lic`) to your project and load it at runtime with `License license = new License(); license.SetLicense("Aspose.Words.lic");`. This should be done before any Aspose.Words API calls to ensure the evaluation mode is disabled.

2. **Q:** Are licenses from newer Aspose.Words versions compatible with older library versions?  
   **A:** Yes. Aspose licenses are generally backward compatible; a license generated for a newer version works with older versions of Aspose.Words. However, features introduced after the older version will not be available.

3. **Q:** Do I need to reinstall the license when I update Aspose.Words via NuGet?  
   **A:** No. The license file is part of your application, not the NuGet package. After updating the package, keep the same license file in your project and continue loading it as before.

4. **Q:** Why does Aspose.Words require Full Trust, and can I run it under Medium Trust?  
   **A:** Full Trust is needed for operations that access the registry (font enumeration) and the file system outside the application folder. Under Medium Trust, some features—especially rendering to images or PDFs—may fail. If you must use Medium Trust, limit operations to those that do not require external resources.

5. **Q:** What should I do if the installer does not add the assemblies to the GAC or Visual Studio reference list?  
   **A:** Manually add a reference to the installed DLLs (e.g., `Aspose.Words.dll`) by right‑clicking the project → *Add Reference* → *Browse* to the installation folder. Ensure the target framework of your project matches the DLL version.