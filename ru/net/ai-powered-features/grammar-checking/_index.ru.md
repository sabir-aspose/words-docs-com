---
title: AI Проверка грамматики
second_title: Aspose.Words для .NET
articleTitle: Проверка грамматики
linktitle: Проверка грамматики
type: docs
weight: 40
description: "Проверка грамматики документа. Aspose.Words для .NET позволяет пользователям проверять грамматику и обнаруживать ошибки в документах, используя модели OpenAI."
url: /ru/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Проверка грамматики в документах важна для обеспечения ясности, профессионализма и точности. Грамотно составленные документы оставляют положительное впечатление и позволяют избежать недоразумений. Проверка грамматики помогает быстро выявлять и исправлять ошибки, экономя время и повышая качество.

Aspose.Words позволяет пользователям проверять грамматику и выявлять ошибки в документах, используя **OpenAI** порождающие модели. Используйте метод [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), доступный в пространстве имен [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/). **CheckGrammar** анализирует текст в документе и выявляет грамматические проблемы.

В следующем примере кода показано, как использовать модель GPT-4o mini в Aspose.Words для проверки грамматики:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Big document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use OpenAI generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gpt4OMini).WithApiKey(apiKey);

CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
grammarOptions.ImproveStylistics = true;

Document proofedDoc = model.CheckGrammar(doc, grammarOptions);
proofedDoc.Save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Проверка грамматики с помощью Aspose.Words повышает качество вашей работы и упрощает внедрение корректуры в ваши проекты. Для получения дополнительной информации ознакомьтесь с документацией [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}