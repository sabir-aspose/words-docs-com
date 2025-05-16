---
title: تلخيص وثيقة
second_title: Aspose.Words ل Java
articleTitle: تلخيص وثيقة
linktitle: تلخيص وثيقة
type: docs
weight: 20
description: "تلخيص وثيقة. Aspose.Words ل Java يبسط تلخيص المستند باستخدام نماذج OpenAI وجوجل AI من خلال السماح لك بتحديد طول الملخص."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ar/java/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

يعد تلخيص المستندات أداة قيمة لمراجعة المحتوى أو الرؤى السريعة أو إعداد الملخصات. Aspose.Words يدعم تلخيص المستندات باستخدام نماذج تعمل بالطاقة AI، مما يسهل معالجة النص الطويل. هذه الميزة، المتوفرة في AI-على أساس Aspose.Words وظيفة، يدمج نماذج اللغة التوليدية المتقدمة من *OpenAI* و *Google*، طالما *Claude's* نماذج اللغة التوليدية البشرية. تتوفر قائمة النماذج المدعومة في [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/) تعداد.

يمكنك تحديد خيارات مختلفة لتلخيص محتوى المستند. استخدم طريقة [Summarize](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#summarize-com.aspose.words.Document-com.aspose.words.SummarizeOptions) لإنشاء ملخص للمستند الخاص بك. يمكنك أيضا تعيين طول الملخص باستخدام خاصية [SummaryLength](https://reference.aspose.com/words/java/com.aspose.words/summarizeoptions/#getSummaryLength).

باستخدام Aspose.Words، يكون تنفيذ تلخيص المستندات أمرا بسيطا. يوضح مثال الكود التالي كيفية تلخيص مستند باستخدام نموذج GPT-4o:

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

تلخيص الوثائق مع Aspose.Words يوفر الوقت ويساعدك على التركيز على المعلومات الأساسية. لمزيد من المعلومات، تحقق من [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}