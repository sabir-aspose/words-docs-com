---
title: Setting Text Color Dynamically in Java
second_title: Aspose.Words for Java
articleTitle: Setting Text Color Dynamically
linktitle: Setting Text Color Dynamically
description: "Set font text color for document contents dynamically when building a report in Java."
type: docs
weight: 85
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /java/setting-text-color-dynamically/
timestamp: 2024-01-27-14-07-04
---

You can set a font color for text contents dynamically using `textColor` tags. Syntax of a `textColor` tag is defined as follows.

{{< highlight csharp >}}
<<textColor [color_expression]>>
content_to_be_colored
<</textColor>>
{{< /highlight >}}

**Note** – A `textColor` tag can be used anywhere in a template document except charts.

An expression declared within an opening `textColor` tag defines a text font color to be applied during runtime. The expression must return a value of one of the following types:

- A string containing the name of a known color, that is, the case-insensitive name of a member of the [KnownColor](https://docs.microsoft.com/en-us/dotnet/api/system.drawing.knowncolor?view=net-6.0) enumeration like in the following example.
  {{< highlight csharp >}}
  <<textColor [“red”]>>text with red font<</textColor>>
  {{< /highlight >}}
- A string containing an HTML color code like in the following example.
  {{< highlight csharp >}}
  <<textColor [“#F08080”]>>text with light coral font<</textColor>>
  {{< /highlight >}}
- An integer value defining RGB (red, green, blue) components of the color like in the following example.
  {{< highlight csharp >}}
  <<textColor [0xFFFF00]>>text with yellow font<</textColor>>
  {{< /highlight >}}
- A value of the [Color](https://docs.microsoft.com/en-us/dotnet/api/system.drawing.color?view=net-6.0) type.

While building a report, an expression declared within an opening `textColor` tag is evaluated and text content between the tag and its corresponding closing tag is colored accordingly. The opening and closing `textColor` tags are removed then.

**Note** – Within a text block to be colored using a `textColor` tag, elements having a text font color already applied are not affected during runtime.

You can use `textColor` tags nested into each other. Also, you can normally use `textColor` tags within data bands and conditional blocks like in the following example.

Assume that you have the `ColoredItem` class defined in your application as follows.

{{< highlight csharp >}}
public class ColoredItem
{
	public String getName() { ... }
	public String getDescription() { ... }
	public Color getColor() { ... }
	...
}
{{< /highlight >}}

Given that `items` is an enumeration of `ColoredItem` instances, you can use the following template to output every item into a separate paragraph, which text is colored dynamically.

{{< highlight csharp >}}
<<foreach [item in items]>><<textColor [item.getColor()]>><<[item.getName()]>><</textColor>>
<</foreach>>
{{< /highlight >}}

To output every item into a separate table row, which text is colored dynamically, you can use the following template.

<table class="setting-text-color-dynamically">
	<tbody>
		<tr>
			<td>&lt;&lt;foreach [item in items]>>&lt;&lt;textColor [item.getColor()]>>&lt;&lt;[item.getName()]>></td>
			<td>&lt;&lt;[item.getDescription()]>>&lt;&lt;/textColor>>&lt;&lt;/foreach>></td>
		</tr>
	</tbody>
</table>

**Note** – Start and end `textColor` tags can be located either in paragraphs of a single story (or table cell) or in rows of a single document table in the same way as `foreach` tags.

------ 

## FAQ

1. **Q:** How can I specify a color using a hexadecimal HTML code in a `textColor` tag?  
   **A:** Place the hex code as a string inside the tag's expression, e.g., `<<textColor ["#1E90FF"]>>`. The engine parses the string and applies the corresponding RGB color at runtime.

2. **Q:** Is it possible to pass a `java.awt.Color` object returned from a method to the `textColor` tag?  
   **A:** Yes. The expression can return a `Color` instance, such as `<<textColor [item.getColor()]>>`. The tag will use the exact RGB values of the returned `Color` object.

3. **Q:** What happens if the text already has a color applied before the `textColor` tag is evaluated?  
   **A:** The existing color is preserved; the `textColor` tag only affects text that does **not** already have a color defined. This prevents overriding manually set colors.

4. **Q:** Can I nest `textColor` tags or use them inside a `foreach` loop?  
   **A:** Both are supported. Nested tags allow hierarchical coloring, and using `textColor` inside `foreach` lets you apply a different color for each iteration based on the data source.

5. **Q:** I receive a “Tag end is unexpected” error when using `textColor`. What could be wrong?  
   **A:** The error usually indicates a mismatched opening/closing tag or an invalid expression. Ensure the opening tag is `<<textColor [expression]>>` and the closing tag is exactly `<</textColor>>`, with no extra characters or missing brackets.