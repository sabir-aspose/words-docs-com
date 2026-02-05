---
title: Setting Background Color Dynamically in Java
second_title: Aspose.Words for Java
articleTitle: Setting Background Color Dynamically
linktitle: Setting Background Color Dynamically
description: "Set text background color for document contents dynamically when building a report in Java."
type: docs
weight: 90
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /java/setting-background-color-dynamically/
timestamp: 2024-01-27-14-07-04
---

You can set text background color for document contents dynamically using `backColor` tags. Syntax of a `backColor` tag is defined as follows.

{{< highlight csharp >}}
<<backColor [color_expression]>>
content_to_be_colored
<</backColor>>
{{< /highlight >}}

**Note** – A `backColor` tag can be used anywhere in a template document except charts.

An expression declared within an opening `backColor` tag defines a text background color to be applied during runtime. The expression must return a value of one of the following types:

- A string containing the name of a known color, that is, the case-insensitive name of a member of the [KnownColor](https://docs.microsoft.com/en-us/dotnet/api/system.drawing.knowncolor?view=net-6.0) enumeration like in the following example.
{{< highlight csharp >}}
<<backColor [“red”]>>text with red background<</backColor>>
{{< /highlight >}}
- A string containing an HTML color code like in the following example.{{< highlight csharp >}}
<<backColor [“#F08080”]>>text with light coral background<</backColor>>
{{< /highlight >}}
- An integer value defining RGB (red, green, blue) components of the color like in the following example.
{{< highlight csharp >}}
<<backColor [0xFFFF00]>>text with yellow background<</backColor>>
{{< /highlight >}}
- A value of the [Color](https://docs.oracle.com/javase/7/docs/api/java/awt/Color.html) type.

While building a report, an expression declared within an opening `backColor` tag is evaluated and document content between the tag and its corresponding closing tag is colored accordingly. The opening and closing `backColor` tags are removed then.

**Note** – Within a document block to be colored using a `backColor` tag, elements having a text background color already applied are not affected during runtime.

You can use `backColor` tags nested into each other. Also, you can normally use `backColor` tags within data bands and conditional blocks like in the following example.

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

Given that `items` is an enumeration of `ColoredItem` instances, you can use the following template to output every item into a separate paragraph colored dynamically.

{{< highlight csharp >}}
<<foreach [item in items]>><<backColor [item.getColor()]>><<[item.getName()]>><</backColor>>
<</foreach>>
{{< /highlight >}}

To output every item into a separate table row colored dynamically, you can use the following template.

<table class="setting-background-color-dynamically">
	<tbody>
		<tr>
			<td>&lt;&lt;foreach [item in items]>>&lt;&lt;backColor [item.getColor()]>>&lt;&lt;[item.getName()]>></td>
			<td>&lt;&lt;[item.getDescription()]>>&lt;&lt;/backColor>>&lt;&lt;/foreach>></td>
		</tr>
	</tbody>
</table>

**Note** – Start and end `backColor` tags can be located either in paragraphs of a single story (or table cell) or in rows of a single document table in the same way as `foreach` tags.

Also, you can use a `backColor` tag to set a solid-fill color for a shape dynamically by performing the following steps:

1. Add a required shape to your template.
1. Set the shape’s fill to none (that is, “No fill”).
1. Inside the shape’s textbox, add opening and closing `backColor` tags so that they to enclose the whole text inside the textbox, if any, like in the following example.
{{< highlight csharp >}}
<<backColor [“red”]>><<text inside shape&lt;&lt;/backColor>>
{{< /highlight >}}

During runtime, an expression declared within the opening `backColor` tag is evaluated and the shape’s solid‑fill color is set accordingly. The opening and closing `backColor` tags are removed then.

------ 

## FAQ

1. **Q:** What types of values can I use in a `backColor` tag expression?  
   **A:** The expression may return a string with a known color name (e.g., “red”), a string with an HTML hex code (e.g., “#F08080”), an integer representing an RGB value (e.g., `0xFFFF00`), or a `java.awt.Color` object.

2. **Q:** Can `backColor` tags be nested inside each other?  
   **A:** Yes. Nested `backColor` tags are supported; the innermost tag overrides the outer one for the enclosed text, and all tags are stripped after processing.

3. **Q:** How do I apply a dynamic background color to a shape’s text?  
   **A:** Insert a shape with “No fill”, place opening and closing `backColor` tags inside the shape’s textbox around the text, and use an expression that returns a supported color value. At runtime the shape’s solid‑fill color will be set to the evaluated color.

4. **Q:** Are `backColor` tags usable inside tables or data‑band blocks such as `foreach`?  
   **A:** Absolutely. `backColor` tags work the same way inside table cells, rows, or any data band. They may span across cells as long as they remain within the same story.

5. **Q:** What happens to text that already has a background color when a `backColor` tag is applied?  
   **A:** Existing background colors are left unchanged; the `backColor` tag only affects text that does not already have a background color applied.