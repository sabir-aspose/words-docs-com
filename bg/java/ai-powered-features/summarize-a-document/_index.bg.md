---
title: Обобщаване на документ
second_title: Aspose.Words за Java
articleTitle: Обобщаване на документ
linktitle: Обобщаване на документ
type: docs
weight: 20
description: "Обобщете документ. Aspose.Words за Java опростява обобщаването на документи, използвайки модели OpenAI и Гугъл AI, като ви позволява да зададете дължината на резюмето."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /bg/java/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

Обобщаването на документи е ценен инструмент за преглед на съдържанието, бързи прозрения или изготвяне на резюмета. Aspose.Words поддържа обобщаване на документи, използвайки AI - захранвани модели, което улеснява обработката на дълъг текст. Тази функция, налична в AI-базираната Aspose.Words функционалност, интегрира съвременни генеративни езикови модели от *OpenAI* и *Google*, както и *Claude's* антропни генеративни езикови модели. Списъкът с поддържаните модели е достъпен в списъка [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/).

Можете да зададете различни опции за обобщаване на съдържанието на документа. Използвайте метода [Summarize](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#summarize-com.aspose.words.Document-com.aspose.words.SummarizeOptions), за да генерирате резюме на вашия документ. Можете също да зададете дължина на резюмето, като използвате свойството [SummaryLength](https://reference.aspose.com/words/java/com.aspose.words/summarizeoptions/#getSummaryLength).

При Aspose.Words обобщаването на документа е лесно. Следващият пример за код показва как да обобщите документ, като използвате модел GPT-4o:

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

Обобщаването на документи с Aspose.Words спестява време и Ви помага да се съсредоточите върху основната информация. За повече информация вижте [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}