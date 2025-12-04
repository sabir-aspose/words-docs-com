---
title: AI Models Supported by Aspose.Words
second_title: Aspose.Words for Java
articleTitle: Supported AI Models
linktitle: Supported AI Models
type: docs
weight: 10
description: "Aspose.Words for Java supports OpenAI and Google AI models for summarization and translation documents. Use Aspose.Words with Gpt-4o, Gpt-4o mini, Gpt-4 Turbo, GPT-3.5 Turbo, Gemini 1.5 Flash, Gemini 1.5 Flash-8B, Gemini 1.5 Pro."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /java/supported-ai-models/
timestamp: 2025-07-29-07-02-49
---

Aspose.Words now leverages advanced AI models to enhance document processing and analysis. With the Aspose.Words.AI namespace, developers can access AI-powered features such as document summarization and analysis, document translation, and grammar checking by integrating generative language models from industry leaders.

## Supported Model Types

Aspose.Words library currently supports integration with:

* OpenAI,
* Google,
* and Claude models' families.

These models bring powerful capabilities for working with documents. By enabling seamless interaction with these AI tools, Aspose.Words simplifies complex tasks and enhances productivity for developers.

{{% alert color="primary" %}}

The full list of supported model types is listed in the [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/) enumeration.

{{% /alert %}}

You can create a model instance using the [Create](https://reference.aspose.com/words/java/com.aspose.words/aimodel/#create-int) method of the [AiModel](https://reference.aspose.com/words/java/com.aspose.words/aimodel/) class.

The following code example shows how to create a new instance of **AiModel** class:

{{< highlight java>}}
public static AiModel create(int modelType)
{{< /highlight >}}

{{% alert color="primary" %}}

For more information, check the [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}

## Using Self-hosted LLM Implementations

With Aspose.Words, developers can also integrate self-hosted LLMs (Large Language Models), providing an alternative to OpenAI/Anthropic/Google's hosted services.

The following code example shows how to create a self-hosted LLM based on OpenAI's generative language model:

{{< highlight java >}}
public void selfHostedModel() throws Exception
{
    Document doc = new Document(getMyDir() + "Big document.docx");

    String apiKey = System.getenv("API_KEY");
    // Use OpenAI generative language models.
    AiModel model = new CustomAiModel().withApiKey(apiKey);

    Document translatedDoc = model.translate(doc, Language.RUSSIAN);
    translatedDoc.save(getArtifactsDir() + "AI.SelfHostedModel.docx");
    }

// Custom self-hosted AI model.
static class CustomAiModel extends OpenAiModel
{
    protected String getUrl()
    {
        return "https://localhost/";
    }

    protected String getName()
    {
        return "my-model-24b";
    }
}
{{< /highlight >}}