---
title: خلاصه یک سند
second_title: Aspose.Words برای Java
articleTitle: خلاصه یک سند
linktitle: خلاصه یک سند
type: docs
weight: 20
description: "یک سند را خلاصه کنید. Aspose.Words برای Java خلاصه سازی اسناد را با استفاده از مدل های OpenAI و Google AI ساده می کند و به شما اجازه می دهد طول خلاصه را مشخص کنید."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fa/java/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

خلاصه کردن اسناد ابزاری ارزشمند برای بررسی محتوا، بینش سریع یا تهیه خلاصه است. Aspose.Words از خلاصه سازی اسناد با استفاده از مدل های AI پشتیبانی می کند و پردازش متن طولانی را آسان تر می کند. این ویژگی که در قابلیت AI مبتنی بر Aspose.Words موجود است، مدل های پیشرفته زبان تولید کننده را از *OpenAI* و *Google* و همچنین مدل های زبان تولید کننده انسان *Claude's* ادغام می کند. لیست مدل های پشتیبانی شده در فهرست [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/) موجود است.

شما می توانید گزینه های مختلفی را برای خلاصه کردن محتوای سند مشخص کنید. از روش [Summarize](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#summarize-com.aspose.words.Document-com.aspose.words.SummarizeOptions) برای ایجاد خلاصه ای از سند خود استفاده کنید. همچنین می توانید طول خلاصه را با استفاده از ویژگی [SummaryLength](https://reference.aspose.com/words/java/com.aspose.words/summarizeoptions/#getSummaryLength) تنظیم کنید.

با Aspose.Words، خلاصه سازی اسناد پیاده سازی ساده است. مثال کد زیر نشان می دهد که چگونه یک سند را با استفاده از مدل GPT-4o خلاصه کنیم:

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

خلاصه کردن اسناد با Aspose.Words زمان را صرفه جویی می کند و به شما کمک می کند تا بر روی اطلاعات ضروری تمرکز کنید. برای اطلاعات بیشتر، [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/) را بررسی کنید.

{{% /alert %}}