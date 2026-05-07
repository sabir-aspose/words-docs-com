---
title: Inserting Images Dynamically in C#
second_title: Aspose.Words for .NET
articleTitle: Inserting Images Dynamically
linktitle: Inserting Images Dynamically
description: "Insert images into your document dynamically when building a report using C#."
type: docs
weight: 60
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/inserting-images-dynamically/
aliases: [/net/template-syntax/#inserting-images-dynamically]
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

## Purpose Summary

This page describes inserting images dynamically.

{{% /alert %}}

You can insert images to your reports dynamically using `image` tags. To declare a dynamically inserted image within your template, do the following steps:

1. Add a textbox to your template at the place where you want an image to be inserted.
1. Set common image attributes such as frame, size, and others for the textbox, making the textbox look like a blank inserted image.
1. Specify an `image` tag within the textbox using the following syntax.

{{< highlight csharp >}}
<<image [image_expression]>>
{{< /highlight >}}

The expression declared within an `image` tag is used by the engine to build an image to be inserted. The expression must return a value of one of the following types:

- A byte array containing an image data
- A [Stream](https://docs.microsoft.com/en-us/dotnet/api/system.io.stream?view=net-6.0) instance able to read an image data
- An [Image](https://docs.microsoft.com/en-us/dotnet/api/system.drawing.image?view=dotnet-plat-ext-6.0) object
- A string containing an image URI, path, or Base64-encoded image data

While building a report, the following procedure is applied to an `image` tag:

1. The expression declared within the tag is evaluated and its result is used to form an image.
1. The corresponding textbox is filled with this image.
1. The tag is removed from the textbox. 

**Note** – If the expression declared within an `image` tag returns a stream object, then it is closed by the engine as soon as the corresponding image is built.

By default, the engine stretches an image filling a textbox to the size of the textbox without preserving the ratio of the image. However, you can change this behavior in the following ways:

- To keep the size of the textbox and stretch the image within bounds of the textbox preserving the ratio of the image, use the `keepRatio` switch as follows.
{{< highlight csharp >}}
<<image [image_expression] -keepRatio>>
{{< /highlight >}}
- To keep the width of the textbox and change its height according to the ratio of the image, use the `fitHeight` switch as follows.
{{< highlight csharp >}}
<<image [image_expression] -fitHeight>>
{{< /highlight >}}
- To keep the height of the textbox and change its width according to the ratio of the image, use the `fitWidth` switch as follows.
{{< highlight csharp >}}
<<image [image_expression] -fitWidth>>
{{< /highlight >}}
- To change the size of the textbox according to the size of the image, use the `fitSize` switch as follows.
{{< highlight csharp >}}
<<image [image_expression] -fitSize>>
{{< /highlight >}}
- To change the size of the textbox according to the size of the image without increasing the size of the textbox, use the `fitSizeLim` switch as follows.
{{< highlight csharp >}}
<<image [image_expression] -fitSizeLim>>
{{< /highlight >}}

**Note** – If the size of the image is greater than the size of the textbox, then the `fitSizeLim` switch acts like `fitHeight` or `fitWidth`. Otherwise, the `fitSizeLim` switch acts like `fitSize`.

## Limitations and Considerations

## Related APIs

------

## FAQ

1. **Q:** What data types can be returned by the image expression?  
   **A:** The expression may return a `byte[]` containing raw image bytes, a `System.IO.Stream` that can read the image data, a `System.Drawing.Image` object, or a `string` that holds an image URI, a file path, or a Base64‑encoded image.

2. **Q:** How does the engine treat a `Stream` returned from the image expression?  
   **A:** After the image is built, the engine automatically closes the `Stream`. You do not need to close it manually, and you should not use the stream after the tag is processed.

3. **Q:** Which switch should I use to keep the original aspect ratio of the image?  
   **A:** Use the `-keepRatio` switch. It stretches the image to fill the textbox while preserving its width‑to‑height ratio.

4. **Q:** How can I make the textbox automatically resize to match the image dimensions?  
   **A:** Apply the `-fitSize` switch. The engine will adjust the textbox size so that it exactly matches the size of the inserted image.

5. **Q:** What does the `-fitSizeLim` switch do, and when should I use it?  
   **A:** `-fitSizeLim` resizes the textbox to the image size but never makes the textbox larger than its original dimensions. If the image is larger, the switch behaves like `-fitHeight` or `-fitWidth`; otherwise, it behaves like `-fitSize`. Use it when you want to limit the textbox growth while still fitting the image proportionally.