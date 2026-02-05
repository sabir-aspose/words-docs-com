---
title: Working with VBA Macros in Java
second_title: Aspose.Words for Java
articleTitle: Working with VBA Macros
linktitle: Working with VBA Macros
description: "Working with document VBA projects using Java."
type: docs
weight: 410
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /java/working-with-vba-macros/
timestamp: 2024-01-27-14-07-04
---

Visual Basic for Applications (VBA) for Microsoft Word is a simple but powerful programming language that can be used to extend the functionality. Aspose.Words API provides three classes to get access to the VBA project source code:

- The [VBAProject](https://reference.aspose.com/words/java/com.aspose.words/vbaproject/) class provides access to the VBA project information
- The [VBAModulesCollection](https://reference.aspose.com/words/java/com.aspose.words/vbamodulecollection/) class returns the collection of VBA project modules
- The [VbaModule](https://reference.aspose.com/words/java/com.aspose.words/vbamodule/) class provides access to the VBA project module

## Create a VBA Project

Aspose.Words API provides the [VbaProject](https://reference.aspose.com/words/java/com.aspose.words/document/#getVbaProject) property to get or set VbaProject in the document.

The following code example demonstrates how to create a VBA project and VBA Module along with basic properties e.g. Name and Type:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithVbaMacros-CreateVbaProject.java" >}}

## Read Macros

Aspose.Words also provides users with the ability to read VBA macros.

The following code example shows how to read VBA Macros from the document:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithVbaMacros-ReadVbaMacros.java" >}}

## Modify Macros

Using Aspose.Words, users can modify VBA macros.

The following code example shows how to modify VBA Macros using the [SourceCode](https://reference.aspose.com/words/java/com.aspose.words/vbamodule/#getSourceCode) property:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithVbaMacros-ModifyVbaMacros.java" >}}

## Clone VBA Project

With Aspose.Words it is also possible to clone VBA projects.

The following code example demonstrates how to clone the VBA Project using the [Clone](https://reference.aspose.com/words/java/com.aspose.words/vbaproject/#deepClone) property which creates a copy of the existing project:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithVbaMacros-CloneVbaProject.java" >}}

## Clone VBA Module

You can also clone VBA modules if needed.

The following code example demonstrates how to clone the VBA Module using the [Clone](https://reference.aspose.com/words/java/com.aspose.words/vbaproject/#deepClone) property which creates a copy of the existing project. 

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithVbaMacros-CloneVbaModule.java" >}}

------ 

## FAQ

1. **Q:** How do I apply an Aspose.Words license when working with VBA macros in Java?  
   **A:** Load the license file using `License license = new License(); license.setLicense("Aspose.Words.Java.lic");` before creating or loading any document. The license must be set once per application domain; otherwise, the library runs in evaluation mode and may add watermarks.

2. **Q:** Can Aspose.Words execute VBA macros embedded in a Word document?  
   **A:** No. Aspose.Words can read, modify, and clone VBA projects, but it does not execute VBA code. Execution of macros must be performed in Microsoft Word or another environment that supports VBA.

3. **Q:** How can I read the source code of a specific VBA module?  
   **A:** Retrieve the module from the `VBAModulesCollection` and use the `getSourceCode()` method:  
   ```java
   VbaModule module = document.getVbaProject().getModules().getByName("Module1");
   String source = module.getSourceCode();
   ```

4. **Q:** What is the recommended way to modify the source code of a VBA macro?  
   **A:** Use the `setSourceCode(String)` method on the `VbaModule` instance after obtaining the module. Save the document afterwards to persist the changes.

5. **Q:** How do I clone an entire VBA project or a single module?  
   **A:** Both `VbaProject` and `VbaModule` implement a deep clone method. Call `VbaProject clonedProject = originalProject.deepClone();` or `VbaModule clonedModule = originalModule.deepClone();` and assign the cloned object to the target document.