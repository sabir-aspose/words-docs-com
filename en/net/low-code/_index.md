---
title: Low Code
second_title: Aspose.Words for .NET
articleTitle: Work with Documents Using LowCode API
linktitle: Low Code
type: docs
description: "Simplify document processing tasks like compare, convert, split, merge, find and replace, and others using Low Code API. Aspose.Words LowCode API with clean syntax, fast results, and minimal coding effort."
weight: 33
url: /net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words for .NET provides the [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/) namespace, which simplifies common document processing tasks. This API is designed for developers who want to accomplish high-level operations such as document comparison, content extraction, image conversion, and text replacement with minimal effort.

The LowCode API is ideal for scenarios where quick implementation is more important than fine-grained control. Let's take a closer look at the LowCode capabilities of Aspose.Words for .NET.

{{% alert color="primary" %}}

It is important to note that the LowCode API does not allow you to change the document structure.

{{% /alert %}}

## Available Features in LowCode API

The `Aspose.Words.LowCode` namespace currently supports:

* **Converting** documents from one format to another
* **Comparing** documents
* **Mail merging**
* **Reporting** based on LINQ syntax
* **Merging** documents
* **Search and replace**
* **Digital signing** of documents
* **Splitting** a document into parts using different criteria
* Adding a **watermark**

{{% alert color="primary" %}}

Please note that a detailed description of each function outside of Low Code can be found in the Developer Guide section.

{{% /alert %}}

## Fluent and Non-Fluent API

Aspose.Words for .NET supports both Fluent and Non-Fluent APIs, allowing developers to choose the style that best fits their coding preferences and project needs. Let's look at some examples to see how these two types of API differ.

{{% alert color="primary" %}}

In the Fluent API, operations can be configured and executed through a context (such as ComparerContext or ReplacerContext). This context contains common options. It ensures that all related methods operate with a consistent configuration, making the API powerful and easy to manage in complex scenarios.

{{% /alert %}}

### Compare Documents

Use `LowCode` to compare two Word documents and save the result.

**non-non-fluent api example:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**fluent api example:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

You can also pass `CompareOptions` for fine-tuned comparison.

**non-fluent api example:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

CompareOptions options = new CompareOptions
{
    IgnoreFormatting = true,
    IgnoreCaseChanges = true
};

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc, options);
{{< /highlight >}}

**fluent api example:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

ComparerContext comparerContext = new ComparerContext();
comparerContext.CompareOptions.IgnoreCaseChanges = true;

Comparer.Create(comparerContext)
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.3.docx")
   .Execute();
{{< /highlight >}}

### Convert Document to Images

Use `LowCode` to convert Word document to PDF.

**non-fluent api example:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**fluent api example:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Find and Replace Text

Use `LowCode` to quickly replace text across the entire document.

**non-fluent api example:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**fluent api example:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";

ReplacerContext replacerContext = new ReplacerContext();
replacerContext.SetReplacement("ReplaceMe", "Replacement");

Replacer.Create(replacerContext)
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

## Why Use Aspose.Words Low Code

The **Aspose.Words.LowCode** namespace helps you implement high-level document processing tasks quickly with clean, readable syntax. It is especially useful for developers who need speed, simplicity, and maintainable code when working with Word documents.

To explore more advanced options, you can always combine LowCode APIs with the full Aspose.Words object model. See more Low Code examples in the [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).