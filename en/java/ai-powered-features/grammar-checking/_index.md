---
title: AI Grammar Checking
second_title: Aspose.Words for Java
articleTitle: Grammar Checking
linktitle: Grammar Checking
type: docs
weight: 40
description: "Check a document grammar. Aspose.Words for Java allows users to check grammar and detect errors in documents using OpenAI, Google, and Claude models."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Checking grammar in documents is important to ensure clarity, professionalism, and accuracy. Well-written documents leave a positive impression and avoid misunderstandings. Grammar checks help identify and correct errors quickly, saving time and improving quality.

Aspose.Words allows users to check grammar and detect errors in documents using the OpenAI, Google, and Claude models' families listed in the [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/) enumeration. Use the [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) method to analyze the text in a document and highlights grammatical problems.

The following code example shows how to use the GPT-4o mini model in Aspose.Words to check grammar:

{{< highlight java >}}
 Document doc = new Document("Big document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI generative language models.
 IAiModelText model = (OpenAiModel)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
 grammarOptions.setImproveStylistics(true);

 Document proofedDoc = model.checkGrammar(doc, grammarOptions);
 proofedDoc.save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Checking grammar with Aspose.Words improves the quality of your work and makes it easy to integrate proofreading into your projects. For more information, check the [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}