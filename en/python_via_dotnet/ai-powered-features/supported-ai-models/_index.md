---
title: AI Models Supported by Aspose.Words
second_title: Aspose.Words for Python via .NET
articleTitle: Supported AI Models
linktitle: Supported AI Models
type: docs
weight: 10
description: "Aspose.Words for Python supports OpenAI and Google AI models for summarization and translation documents. Use Aspose.Words with Gpt-4o, Gpt-4o mini, Gpt-4 Turbo, GPT-3.5 Turbo, Gemini 1.5 Flash, Gemini 1.5 Flash-8B, Gemini 1.5 Pro."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/supported-ai-models/
timestamp: 2026-02-03-11-08-55
---

{{% alert color="grey" %}}
*Purpose Summary. What is this page about?*

This page outlines the AI model families supported by Aspose.Words for Python via .NET and explains how to create `AiModel` instances using the `AiModelType` enumeration.
{{% /alert %}}

Aspose.Words now leverages advanced AI models to enhance document processing and analysis. With the Aspose.Words.AI namespace, developers can access AI‑powered features such as document summarization and analysis, document translation, and grammar checking by integrating generative language models from industry leaders.

## Supported Model Types

Aspose.Words library currently supports integration with:

* OpenAI,
* Google,
* and Claude models' families.

These models bring powerful capabilities for working with documents. By enabling seamless interaction with these AI tools, Aspose.Words simplifies complex tasks and enhances productivity for developers.

{{% alert color="primary" %}}

The full list of supported model types is listed in the [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/) enumeration.

{{% /alert %}}

You can create a model instance using the [create](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodel/create/) method of the [AiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodel/) class. 

The following code example shows how to create a new instance of **AiModel** class.

{{< highlight python >}}
def create(self, model_type: aspose.words.ai.AiModelType):
    ...
{{< /highlight >}}

{{% alert color="primary" %}}

For more information, check the [aspose.words.ai](https://reference.aspose.com/words/python-net/aspose.words.ai/) API documentation.

{{% /alert %}}

------ 

## FAQ

1. **Q:** Which AI model families are currently supported by Aspose.Words for Python?  
   **A:** Aspose.Words supports models from OpenAI, Google (Gemini), and Anthropic Claude families. The specific models are exposed through the `AiModelType` enumeration, such as `OpenAI_Gpt4Turbo`, `Google_Gemini1_5Flash`, and `Claude_Instant`.

2. **Q:** How do I create an `AiModel` instance for a particular model type?  
   **A:** Use the static `create` method of the `AiModel` class and pass a value from the `AiModelType` enumeration. Example:  

   ```python
   import aspose.words.ai as ai

   model = ai.AiModel.create(ai.AiModelType.OpenAI_Gpt4Turbo)
   ```

3. **Q:** Can I retrieve the list of all supported model types programmatically?  
   **A:** Yes. The `AiModelType` enumeration provides all supported values. You can iterate over it using Python's `dir` or `Enum` utilities:

   ```python
   import aspose.words.ai as ai
   from enum import Enum

   for model_type in ai.AiModelType:
       print(model_type.name)
   ```

4. **Q:** Is it possible to switch the AI model used for summarization at runtime?  
   **A:** Absolutely. Create a new `AiModel` with the desired `AiModelType` and pass it to the summarization API each time you call it. The previous model instance does not need to be disposed.

5. **Q:** Are the latest OpenAI models such as **GPT‑4o** and **GPT‑4 Turbo** supported?  
   **A:** Yes. They are represented in the enumeration as `OpenAI_Gpt4o` and `OpenAI_Gpt4Turbo`. Use these values when creating the `AiModel` to access the newest capabilities.