---
title: Inlining Syntax Error Messages into Templates in Java
second_title: Aspose.Words for Java
articleTitle: Inlining Syntax Error Messages into Templates
linktitle: Inlining Syntax Error Messages into Templates
description: "Learn how to enable inline syntax error message into the template document at the exact position using LINQ in Java."
type: docs
weight: 80
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /java/inlining-syntax-error-messages-into-templates/
timestamp: 2024-01-27-14-07-04
---

By default, LINQ Reporting Engine throws an exception when encounters a template syntax error. Such an exception provides information on a reason of the error and specifies a tag or expression part where the error is encountered. In most cases, this information is enough to find a place in a template causing the error and fix it.

However, when dealing with complex templates containing a large number of tags, it becomes harder to find an exact place in a template causing an error. To make things easier, the engine supports the `ReportBuildOptions.INLINE_ERROR_MESSAGES` option that enables inlining of a syntax error message into a template document at an exact position where the error occurs during runtime. 

**Note** – A template syntax error message is written using a bold font to make it more apparent.

Consider the following template.

{{< highlight xml >}}
<<var [name]>>
{{< /highlight >}}

By default, such a template causes the engine to throw an exception while building a report. However, when `ReportBuildOptions.INLINE_ERROR_MESSAGES` is applied, no exception is thrown and the report looks as follows then.

{{< highlight xml >}}
<<var [name] Error! An assignment operator is expected. >>
{{< /highlight >}}

**Note** – Only messages describing errors in template syntax can be inlined; messages describing errors encountered during expressions' evaluation cannot.

When `ReportBuildOptions.INLINE_ERROR_MESSAGES` is applied, a `Boolean` value returned by a `ReportingEngine.buildReport` overload indicates whether building of a report was finished successfully or was interrupted because of a template syntax error. This enables you to process reports which building succeeded or failed differently as shown in the following code snippet.

{{< highlight java >}}
ReportingEngine engine = new ReportingEngine();
engine.setOptions(ReportBuildOptions.INLINE_ERROR_MESSAGES);

if (engine.buildReport(...))
{
	// Do something with a successfully built report.
}
else
{
	// Do something with a report containing a template syntax error.
}
{{< /highlight >}}

**Note** – When `ReportBuildOptions.INLINE_ERROR_MESSAGES` is not applied, `ReportingEngine.buildReport` overloads return `true` if there were no template syntax errors encountered or throw an exception otherwise.

------ 

## FAQ

1. **Q:** How do I enable inline syntax error messages for a report?  
   **A:** Create a `ReportingEngine` instance and set its options to `ReportBuildOptions.INLINE_ERROR_MESSAGES` before calling `buildReport`. This tells the engine to embed syntax error messages directly into the generated document instead of throwing an exception.

2. **Q:** What does the boolean result of `buildReport` indicate when inline error messages are enabled?  
   **A:** The method returns `true` if the report was built without any template‑syntax errors. It returns `false` when a syntax error was detected and inlined into the document, allowing you to handle the two cases separately.

3. **Q:** Are runtime evaluation errors (e.g., division by zero) also inlined with this option?  
   **A:** No. Only syntax‑related errors are inlined. Errors that occur while evaluating expressions are still thrown as exceptions because they cannot be represented as inline messages.

4. **Q:** Can I change the appearance (font, color) of the inlined error messages?  
   **A:** The engine writes error messages using a bold font by default. Custom styling is not configurable through the API; you would need to post‑process the document to modify the formatting after the report is generated.

5. **Q:** Does enabling `INLINE_ERROR_MESSAGES` suppress all exceptions from the reporting engine?  
   **A:** It suppresses exceptions that are caused by template syntax errors only. Other exceptions (e.g., I/O errors, missing data sources) are still thrown and must be handled in the usual way.