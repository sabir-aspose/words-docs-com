---
title: تلخيص وثيقة
second_title: Aspose.Words ل Python via .NET
articleTitle: تلخيص وثيقة
linktitle: تلخيص وثيقة
type: docs
weight: 20
description: "تلخيص وثيقة. Aspose.Words ل Python يبسط تلخيص المستند باستخدام نماذج OpenAI وجوجل AI من خلال السماح لك بتحديد طول الملخص."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ar/python-net/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

يعد تلخيص المستندات أداة قيمة لمراجعة المحتوى أو الرؤى السريعة أو إعداد الملخصات. Aspose.Words يدعم تلخيص المستندات باستخدام نماذج تعمل بالطاقة AI، مما يسهل معالجة النص الطويل. هذه الميزة، المتوفرة في وحدة [aspose.words.ai](https://reference.aspose.com/words/python-net/aspose.words.ai/)، تدمج نماذج اللغة التوليدية المتقدمة من *OpenAI* و *Google*، وكذلك *Claude's* نماذج اللغة التوليدية البشرية. تتوفر قائمة النماذج المدعومة في [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/) تعداد.

يمكنك تحديد خيارات مختلفة لتلخيص محتوى المستند. استخدم طريقة [summarize](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/summarize/) لإنشاء ملخص للمستند الخاص بك. يمكنك أيضا تعيين طول الملخص باستخدام خاصية [summary_length](https://reference.aspose.com/words/python-net/aspose.words.ai/summarizeoptions/summary_length/).

باستخدام Aspose.Words، يكون تنفيذ تلخيص المستندات أمرا بسيطا. يوضح مثال الكود التالي كيفية تلخيص مستند باستخدام نموذج GPT-4o:

{{< highlight python >}}
first_doc = aw.Document(MyDir + "Big document.docx")
second_doc = aw.Document(MyDir + "Document.docx")
api_key = os.getenv("API_KEY")
# Use OpenAI or Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GPT_4O_MINI).with_api_key(api_key).as_open_ai_model()
options = aw.ai.SummarizeOptions()
options.summary_length = aw.ai.SummaryLength.SHORT
one_document_summary = model.summarize(first_doc, options)
oneDocumentSummary.save(ArtifactsDir + "AI.AiSummarize.One.docx")
options.summary_length = aw.ai.SummaryLength.LONG
multi_document_summary = model.summarize([first_doc, second_doc], options)
multiDocumentSummary.save(ArtifactsDir + "AI.AiSummarize.Multi.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

تلخيص الوثائق مع Aspose.Words يوفر الوقت ويساعدك على التركيز على المعلومات الأساسية. لمزيد من المعلومات، راجع وثائق [aspose.words.ai](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}