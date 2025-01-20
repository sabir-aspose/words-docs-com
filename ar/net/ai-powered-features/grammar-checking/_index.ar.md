---
title: AI التدقيق النحوي
second_title: Aspose.Words ل .NET
articleTitle: التدقيق النحوي
linktitle: التدقيق النحوي
type: docs
weight: 40
description: "تحقق من قواعد المستند. Aspose.Words ل .NET يسمح للمستخدمين بالتحقق من القواعد واكتشاف الأخطاء في المستندات باستخدام نماذج OpenAI."
url: /ar/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

يعد التحقق من القواعد في المستندات أمرا مهما لضمان الوضوح والاحتراف والدقة. تترك المستندات المكتوبة جيدا انطباعا إيجابيا وتتجنب سوء الفهم. تساعد عمليات التدقيق النحوي في تحديد الأخطاء وتصحيحها بسرعة، مما يوفر الوقت ويحسن الجودة.

Aspose.Words يسمح للمستخدمين بالتحقق من القواعد واكتشاف الأخطاء في المستندات باستخدام **OpenAI** النماذج التوليدية. استخدم طريقة [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/) المتوفرة في [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) مساحة الاسم. **CheckGrammar** يحلل النص في وثيقة ويسلط الضوء على المشاكل النحوية.

يوضح مثال الكود التالي كيفية استخدام نموذج GPT-4o mini في Aspose.Words للتحقق من القواعد:

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

يؤدي التحقق من القواعد باستخدام Aspose.Words إلى تحسين جودة عملك ويجعل من السهل دمج التدقيق اللغوي في مشاريعك. لمزيد من المعلومات، راجع وثائق [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}