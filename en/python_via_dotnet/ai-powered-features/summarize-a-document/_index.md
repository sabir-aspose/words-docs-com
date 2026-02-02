---
title: Summarize a Document
second_title: Aspose.Words for Python via .NET
articleTitle: Summarize a Document
linktitle: Summarize a Document
type: docs
weight: 20
description: "Summarize a document. Aspose.Words for Python simplifies document summarization using OpenAI and Google AI models by allowing you to specify the summary length."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

{{% alert color="grey" %}}
*Purpose Summary. What is this page about?*

This page demonstrates how to use Aspose.Words for Python via .NET's AI capabilities to generate summaries of single or multiple documents, including selecting AI models and configuring summary length.
{{% /alert %}}

Summarizing documents is a valuable tool for content review, quick insights, or preparing abstracts. Aspose.Words supports document summarization using AI-powered models, making it easier to process long text. This feature, available in the [aspose.words.ai](https://reference.aspose.com/words/python-net/aspose.words.ai/) module, integrates advanced generative language models from *OpenAI* and *Google*, as well as *Claude's* anthropic generative language models. The list of supported models is available in the [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/) enumeration.

You can specify various options for summarizing document content. Use the [summarize](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodel/summarize/) method to generate a summary of your document. You can also set summary length using the [summary_length](https://reference.aspose.com/words/python-net/aspose.words.ai/summarizeoptions/summary_length/) property.

With Aspose.Words, implementing document summarization is straightforward. The following code example shows how to summarize a document using GPT-4o model:

{{< highlight python >}}
first_doc = aw.Document(MyDir + "Big document.docx")
second_doc = aw.Document(MyDir + "Document.docx")
api_key = os.getenv("API_KEY")
# Use OpenAI or Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GPT_4O_MINI).with_api_key(api_key).as_open_ai_model()
options = aw.ai.SummarizeOptions()
options.summary_length = aw.ai.SummaryLength.SHORT
one_document_summary = model.summarize(first_doc, options)
oneDocumentSummary.save(ArtifactsDir + "AI.AiSummarize.One.docx")
options.summary_length = aw.ai.SummaryLength.LONG
multi_document_summary = model.summarize([first_doc, second_doc], options)
multiDocumentSummary.save(ArtifactsDir + "AI.AiSummarize.Multi.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Summarizing documents with Aspose.Words saves time and helps you focus on essential information. For more information, check the [aspose.words.ai](https://reference.aspose.com/words/python-net/aspose.words.ai/) API documentation.

{{% /alert %}}

------ 

## FAQ

1. **Q:** Which AI models can I use for document summarization?  
   **A:** Aspose.Words for Python via .NET supports OpenAI models (e.g., GPT‑4o, GPT‑4o‑mini), Google Gemini models, and Anthropic Claude models. The full list is defined in the `aw.ai.AiModelType` enumeration.

2. **Q:** How do I control the length of the generated summary?  
   **A:** Set the `summary_length` property of `aw.ai.SummarizeOptions` to one of the values in `aw.ai.SummaryLength` (e.g., `SHORT`, `MEDIUM`, `LONG`). The chosen value influences how concise or detailed the summary will be.

3. **Q:** Can I summarize more than one document in a single request?  
   **A:** Yes. Pass a list of `aw.Document` objects to the `summarize` method. The model will generate a combined summary for all supplied documents.

4. **Q:** Do I need a separate license for using the AI summarization feature?  
   **A:** No additional license is required beyond a valid Aspose.Words for Python via .NET license. The AI features are included with the standard product license.

5. **Q:** Is the summarization feature available on Linux platforms?  
   **A:** Yes. Aspose.Words for Python via .NET runs on Linux, and the AI summarization APIs work the same way as on Windows, provided the required runtime dependencies are installed.