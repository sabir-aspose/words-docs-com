---
title: AI перевірка граматики
second_title: Aspose.Words для .NET
articleTitle: Перевірка граматики
linktitle: Перевірка граматики
type: docs
weight: 40
description: "Перевірка граматики документа. Aspose.Words для .NET дозволяє користувачам перевіряти граматику та виявляти помилки в документах за допомогою моделей OpenAI."
url: /uk/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Перевірка граматики в документах важлива для забезпечення ясності, професіоналізму та точності. Грамотно складені документи залишають позитивне враження і дозволяють уникнути непорозумінь. Перевірка граматики допомагає швидко виявляти та виправляти помилки, заощаджуючи час та покращуючи якість.

Aspose.Words дозволяє користувачам перевіряти граматику та виявляти помилки в документах, використовуючи **OpenAI** генеруючі моделі. Використовуйте метод [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), доступний у просторі імен [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/). **CheckGrammar** аналізує текст у документі та виявляє граматичні проблеми.

Наступний приклад коду показує, як використовувати модель GPT-4o mini в Aspose.Words для перевірки граматики:

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

Перевірка граматики за допомогою Aspose.Words покращує якість вашої роботи та полегшує впровадження коректури у ваші проекти. Для отримання додаткової інформації перегляньте документацію [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}