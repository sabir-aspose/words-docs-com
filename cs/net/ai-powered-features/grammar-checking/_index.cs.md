---
title: AI Kontrola Gramatiky
second_title: Aspose.Words pro .NET
articleTitle: Gramatik
linktitle: Gramatik
type: docs
weight: 40
description: "Zkontrolujte gramatiku dokumentu. Aspose.Words pro .NET umožňuje uživatelům kontrolovat gramatiku a detekovat chyby v dokumentech pomocí modelů OpenAI."
url: /cs/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Kontrola gramatiky v dokumentech je důležitá pro zajištění jasnosti, profesionality a přesnosti. Dobře napsané dokumenty zanechávají pozitivní dojem a vyhýbají se nedorozuměním. Gramatické kontroly pomáhají rychle identifikovat a opravit chyby, šetří čas a zlepšují kvalitu.

Aspose.Words umožňuje uživatelům kontrolovat gramatiku a detekovat chyby v dokumentech pomocí **OpenAI** generativních modelů. Použijte metodu [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), která je k dispozici v oboru názvů [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/). **CheckGrammar** analyzuje text v dokumentu a zdůrazňuje gramatické problémy.

Následující příklad kódu ukazuje, jak použít model GPT-4o mini v Aspose.Words ke kontrole gramatiky:

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

Kontrola gramatiky pomocí Aspose.Words zlepšuje kvalitu vaší práce a usnadňuje integraci korektur do vašich projektů. Další informace najdete v dokumentaci [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}