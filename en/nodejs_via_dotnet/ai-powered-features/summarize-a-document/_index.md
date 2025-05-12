---
title: Summarize a Document
second_title: Aspose.Words for Node.js via .NET
articleTitle: Summarize a Document
linktitle: Summarize a Document
type: docs
weight: 20
description: "Summarize a document. Aspose.Words for Node.js simplifies document summarization using OpenAI, Google and Anthropic AI models by allowing you to specify the summary length."
url: /nodejs-net/summarize-a-document/
timestamp: 2025-05-12-12-00-00
---

Summarizing documents is a valuable tool for content review, quick insights, or preparing abstracts. Aspose.Words supports document summarization using AI-powered models, making it easier to process long text. This feature, available in the [aspose.words.ai](https://reference.aspose.com/words/nodejs-net/aspose.words.ai/) module, integrates advanced generative language models from *OpenAI*, *Google* and *Anthropic*. 

You can specify various options for summarizing document content. Use the [summarize](https://reference.aspose.com/words/nodejs-net/aspose.words.ai/iaimodeltext/summarize/) method to generate a summary of your document. You can also set summary length using the [summary_length](https://reference.aspose.com/words/nodejs-net/aspose.words.ai/summarizeoptions/summarylength/) property.

With Aspose.Words, implementing document summarization is straightforward. The following code example shows hot to summirize a documet using GPT-4o model:

{{< highlight js >}}
let firstDoc = new aw.Document("Big document.docx");
let secondDoc = new aw.Document("Document.docx");
const apiKey = process.env.API_KEY;
// Use OpenAI or Google generative language models.
let model = aw.AI.AiModel.createGpt4OMini();
model.setApiKey(apiKey);
model.setOrganization("Organization");
model.setProject("Project");
let options = new aw.AI.SummarizeOptions();
options.summaryLength = aw.AI.SummaryLength.Short;
let oneDocumentSummary = model.summarize(firstDoc, options);
oneDocumentSummary.save("AI.AiSummarize.one.docx");
options.summaryLength = aw.AI.SummaryLength.Long;
let multiDocumentSummary = model.summarize([firstDoc, secondDoc], options);
multiDocumentSummary.save("AI.AiSummarize.multi.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Summarizing documents with Aspose.Words saves time and helps you focus on essential information. For more information, check the [aspose.words.ai](https://reference.aspose.com/words/nodejs-net/aspose.words.ai/) API documentation.

{{% /alert %}}