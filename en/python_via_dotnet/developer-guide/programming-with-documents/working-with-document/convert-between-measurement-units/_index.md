---
title: Convert Between Measurement Units
second_title: Aspose.Words for Python via .NET
articleTitle: Convert Between Measurement Units
linktitle: Convert Between Measurement Units
description: "Aspose.Words for Python via .NET can help you with how to convert between measurement units, for example, inches to points and points to inches, pixels to points, points to pixels."
type: docs
weight: 20
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/convert-between-measurement-units/
aliases: [/python/convert-between-measurement-units/]
timestamp: 2026-02-03-11-08-55
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page demonstrates how to use Aspose.Words for Python via .NET's `ConvertUtil` class to convert between measurement units such as inches, points, pixels, and millimeters, including examples of setting page properties in inches.

{{% /alert %}}

Most of the object properties provided in the Aspose.Words API that represent some measurement, such as width or height, margins, and various distances, accept values in points, where 1 inch equals 72 points. Sometimes this is not convenient and points need to be converted to other units.

Aspose.Words provides the [ConvertUtil](https://reference.aspose.com/words/python-net/aspose.words/convertutil/) class that provides helper functions to convert between various measurement units. It enables to convert:

- inches, pixels, and millimeters to points
- points to inches and pixels
- pixels from one resolution to another

Converting pixels to points and vice versa can be performed at 96 dpi (dots per inch) resolutions or specified dpi resolution.

The [ConvertUtil](https://reference.aspose.com/words/python-net/aspose.words/convertutil/) class is especially useful when setting various page properties because, for instance, inches are more common measurement units than points.

The following code example shows how to specify page properties in inches:

{{< gist "aspose-words-gists" "1c0fc25570ac4cf773afe35e217e35aa" "convert-between-measurement-units.py" >}}

## FAQ

1. **Q:** How do I convert inches to points?  
   **A:** Use `ConvertUtil.inch_to_point`. The method takes a floating‑point value representing inches and returns the equivalent number of points (1 inch = 72 points).  
   ```python
   import aspose.words as aw

   inches = 2.5
   points = aw.ConvertUtil.inch_to_point(inches)
   print(f"{inches} inches = {points} points")
   ```

2. **Q:** How do I convert points to inches?  
   **A:** Call `ConvertUtil.point_to_inch`. It receives a point value and returns the measurement in inches.  
   ```python
   import aspose.words as aw

   points = 180
   inches = aw.ConvertUtil.point_to_inch(points)
   print(f"{points} points = {inches} inches")
   ```

3. **Q:** How can I convert pixels to points at the default 96 dpi resolution?  
   **A:** Use `ConvertUtil.pixel_to_point`. When you omit the DPI argument, 96 dpi is assumed.  
   ```python
   import aspose.words as aw

   pixels = 300
   points = aw.ConvertUtil.pixel_to_point(pixels)   # 96 dpi is used automatically
   print(f"{pixels} pixels = {points} points at 96 dpi")
   ```

4. **Q:** How do I convert points to pixels with a custom DPI?  
   **A:** Use `ConvertUtil.point_to_pixel` and pass the desired DPI value.  
   ```python
   import aspose.words as aw

   points = 72
   dpi = 150
   pixels = aw.ConvertUtil.point_to_pixel(points, dpi)
   print(f"{points} points = {pixels} pixels at {dpi} dpi")
   ```

5. **Q:** I get an error saying `'ConvertUtil' has no attribute 'point_to_twip'`. Why?  
   **A:** The `ConvertUtil` class does not provide a `point_to_twip` method. Twips are a legacy unit (1 point = 20 twips) and must be converted manually: multiply the point value by 20.  
   ```python
   points = 5
   twips = points * 20
   print(f"{points} points = {twips} twips")
   ```
   If you need a dedicated helper, create a small wrapper function that performs this multiplication.