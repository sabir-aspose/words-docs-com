---
title: AI Проверка На Граматиката
second_title: Aspose.Words за .NET
articleTitle: Проверка На Граматиката
linktitle: Проверка На Граматиката
type: docs
weight: 40
description: "Проверете граматиката на документа. Aspose.Words за .NET позволява на потребителите да проверяват граматиката и да откриват грешки в документите, използвайки OpenAI модели."
url: /bg/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Проверката на граматиката в документите е важна, за да се гарантира яснота, професионализъм и точност. Добре написаните документи оставят положително впечатление и избягват недоразумения. Проверките на граматиката помагат бързо да се идентифицират и коригират грешките, спестявайки време и подобрявайки качеството.

Aspose.Words позволява на потребителите да проверяват граматиката и да откриват грешки в документите, използвайки **OpenAI** генеративни модели. Използвайте метода [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), Наличен в пространство от имена [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/). **CheckGrammar** анализира текста в документ и подчертава граматическите проблеми.

Следващият пример за код показва как да използвате модела GPT-4o mini в Aspose.Words, за да проверите граматиката:

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

Проверката на граматиката с Aspose.Words подобрява качеството на работата ви и улеснява интегрирането на корекцията във вашите проекти. За повече информация вижте документацията [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}