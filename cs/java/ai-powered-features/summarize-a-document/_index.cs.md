---
title: Shrňte dokument
second_title: Aspose.Words pro Java
articleTitle: Shrňte dokument
linktitle: Shrňte dokument
type: docs
weight: 20
description: "Shrňte dokument. Aspose.Words pro Java zjednodušuje sumarizaci dokumentů pomocí modelů OpenAI a Google AI tím, že umožňuje určit délku souhrnu."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/java/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Shrnutí dokumentů je cenným nástrojem pro kontrolu obsahu, rychlé postřehy nebo přípravu abstraktů. Aspose.Words podporuje sumarizaci dokumentů pomocí modelů poháněných AI, což usnadňuje zpracování dlouhého textu. Tato funkce, která je k dispozici ve funkci AI založené na Aspose.Words, integruje pokročilé generativní jazykové modely z *OpenAI* a *Google* a také *Claude's* antropické generativní jazykové modely. Seznam podporovaných modelů je k dispozici ve výčtu [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/).

Můžete zadat různé možnosti pro shrnutí obsahu dokumentu. Pomocí metody [Summarize](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#summarize-com.aspose.words.Document-com.aspose.words.SummarizeOptions) Vygenerujte souhrn dokumentu. Můžete také nastavit délku souhrnu pomocí vlastnosti [SummaryLength](https://reference.aspose.com/words/java/com.aspose.words/summarizeoptions/#getSummaryLength).

S Aspose.Words je shrnutí implementačního dokumentu jednoduché. Následující příklad kódu ukazuje, jak shrnout dokument pomocí modelu GPT-4o:

{{< highlight java >}}
Document firstDoc = new Document(getMyDir() + "Big document.docx");
 Document secondDoc = new Document(getMyDir() + "Document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI or Google generative language models.
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 Document oneDocumentSummary = model.summarize(firstDoc, new SummarizeOptions(); { oneDocumentSummary.setSummaryLength(SummaryLength.SHORT); });
 oneDocumentSummary.save(getArtifactsDir() + "AI.AiSummarize.One.docx");

 Document multiDocumentSummary = model.summarize(new Document[] { firstDoc, secondDoc }, new SummarizeOptions(); { multiDocumentSummary.setSummaryLength(SummaryLength.LONG); });
 multiDocumentSummary.save(getArtifactsDir() + "AI.AiSummarize.Multi.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Shrnutí dokumentů pomocí Aspose.Words šetří čas a pomáhá vám soustředit se na základní informace. Pro více informací zkontrolujte [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}