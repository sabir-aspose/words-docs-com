---
title: Document Processing Interruption in C#
second_title: Aspose.Words for .NET
articleTitle: Document Processing Interruption
linktitle: Document Processing Interruption
description: "How to use the .NET CancellationToken in Aspose.Words to safely interrupt long-running document processing tasks in C#"
type: docs
weight: 70
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/document-processing-interruption/
timestamp: 2025-10-15-11-08-55
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page explains how to detect and handle processing interruptions for long-running document tasks.

{{% /alert %}}

Document processing in .NET applications can involve complex and time-consuming operations, such as loading and saving large files, building the document layout, updating fields, or retrieving external resources.

Sometimes it is necessary to gracefully interrupt document processing without forcibly terminating the application or leaving resources in an inconsistent state. To ensure greater control over these long-running tasks, the processing flow can be managed using appropriate callbacks.

## CancellationToken for Interrupting Document Processing

.NET has a widely used `CancellationToken` structure. It is a built-in mechanism for safely and controlled closure of asynchronous operations.

The `CancellationToken` structure in .NET provides a standardized mechanism that allows developers to monitor and respond to cancellation requests during asynchronous or long-running operations.

It is useful to know that Aspose.Words also allows to interrupt document processing using callbacks, where a `CancellationToken` can be used as a process interruption trigger.

## How to Use a CancellationToken

By integrating a `CancellationToken` into your document processing logic, you can safely and efficiently stop the operation when needed.

The following code example shows how to use a `CancellationToken` to interrupt a document processing task:

{{< highlight csharp >}}
// Arrange
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    // Simulate user cancel after short delay
    _ = Task.Run(async () =>
    {
        await Task.Delay(20);
        cts.Cancel();
    });

    try
    {
        ProcessDocument(cts.Token);
    }
    catch (OperationCanceledException ex)
    {
        Console.WriteLine(ex.Message);
    }
}
{{< /highlight >}}

{{< highlight csharp >}}
public static void ProcessDocument(CancellationToken token)
{
    CancelationCallback cancelationCallback = new CancelationCallback(token);

    LoadOptions loadOptions = new LoadOptions();
    loadOptions.ProgressCallback = cancelationCallback;
    loadOptions.ResourceLoadingCallback = cancelationCallback;

    SaveOptions saveOptions = new PdfSaveOptions();
    saveOptions.ProgressCallback = cancelationCallback;

    Document doc = new Document(@"C:\Temp\in.docx", loadOptions);
    doc.LayoutOptions.Callback = cancelationCallback;
    doc.FieldOptions.FieldUpdatingProgressCallback = cancelationCallback;

    doc.Save(@"C:\Temp\out.pdf", saveOptions);
}
{{< /highlight >}}

{{< highlight csharp >}}
private class CancelationCallback : 
    IDocumentLoadingCallback,
    IDocumentSavingCallback,
    IPageLayoutCallback,
    IFieldUpdatingProgressCallback,
    IResourceLoadingCallback
{
    public CancelationCallback(CancellationToken token)
    {
        mToken = token;
    }

    void IDocumentLoadingCallback.Notify(DocumentLoadingArgs args)
    {
        ThrowIfCancellationRequested("Document processing is canceled at the document loading stage.");
    }

    void IDocumentSavingCallback.Notify(DocumentSavingArgs args)
    {
        ThrowIfCancellationRequested("Document processing is canceled at the document saving stage.");
    }

    void IPageLayoutCallback.Notify(PageLayoutCallbackArgs args)
    {
        ThrowIfCancellationRequested("Document processing is canceled at the building document layout stage.");
    }

    void IFieldUpdatingProgressCallback.Notify(FieldUpdatingProgressArgs args)
    {
        ThrowIfCancellationRequested("Document processing is canceled at the field updating stage.");
    }

    ResourceLoadingAction IResourceLoadingCallback.ResourceLoading(ResourceLoadingArgs args)
    {
        try
        {
            return mToken.IsCancellationRequested ? ResourceLoadingAction.Skip : ResourceLoadingAction.Default;
        }
        finally
        {
            ThrowIfCancellationRequested("Document processing is canceled at the loading external resources stage.");
        }
    }

    private void ThrowIfCancellationRequested(string message)
    {
        if (mToken.IsCancellationRequested)
            throw new OperationCanceledException(message, mToken);
    }

    private CancellationToken mToken;
}
{{< /highlight >}}

## Document Processing Interruption Using Low Code

If complex document processing is not required, a similar approach using Low Code can be used. In this case, you will need an overload of the [Execute](https://reference.aspose.com/words/net/aspose.words.lowcode/processor/execute/#execute_1) method that accepts a `CancellationToken` as a parameter.

The following code example shows how to interrupt a document processing task with Low Code:

{{< highlight csharp >}}
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    // Simulate user cancel after short delay
    Task.Run(() => {
        Thread.Sleep(20);
        cts.Cancel();
    });

    try
    {
        Converter.Create().From(MyDir + "Simple.docx").To(ArtifactsDir + "Processor.ExecuteAsync.pdf").Execute(cts.Token);
    }
    catch (OperationCanceledException ex)
    {
        Console.WriteLine($"Cancellation reason: '{ex.Message}'");
    }
}
{{< /highlight >}}