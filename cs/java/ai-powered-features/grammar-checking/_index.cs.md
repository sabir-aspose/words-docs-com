---
title: AI Kontrola Gramatiky
second_title: Aspose.Words pro Java
articleTitle: Gramatik
linktitle: Gramatik
type: docs
weight: 40
description: "Zkontrolujte gramatiku dokumentu. Aspose.Words pro Java umožňuje uživatelům kontrolovat gramatiku a detekovat chyby v dokumentech pomocí modelů OpenAI, Google a Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Kontrola gramatiky v dokumentech je důležitá pro zajištění jasnosti, profesionality a přesnosti. Dobře napsané dokumenty zanechávají pozitivní dojem a vyhýbají se nedorozuměním. Gramatické kontroly pomáhají rychle identifikovat a opravit chyby, šetří čas a zlepšují kvalitu.

Aspose.Words umožňuje uživatelům kontrolovat gramatiku a detekovat chyby v dokumentech pomocí rodin modelů OpenAI, Google a Claude uvedených ve výčtu [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). Pomocí metody [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) analyzujte text v dokumentu a zvýrazněte gramatické problémy.

Následující příklad kódu ukazuje, jak použít model GPT-4o mini v Aspose.Words ke kontrole gramatiky:

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

Kontrola gramatiky pomocí Aspose.Words zlepšuje kvalitu vaší práce a usnadňuje integraci korektur do vašich projektů. Pro více informací zkontrolujte [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}