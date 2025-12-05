---
title: تلخيص وثيقة
second_title: Aspose.Words ل C++
articleTitle: تلخيص وثيقة
linktitle: تلخيص وثيقة
type: docs
weight: 20
description: "تلخيص وثيقة. Aspose.Words ل C++ يبسط تلخيص المستند باستخدام نماذج OpenAI وجوجل AI من خلال السماح لك بتحديد طول الملخص."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ar/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

يعد تلخيص المستندات أداة قيمة لمراجعة المحتوى أو الرؤى السريعة أو إعداد الملخصات. Aspose.Words يدعم تلخيص المستندات باستخدام نماذج تعمل بالطاقة AI، مما يسهل معالجة النص الطويل. هذه الميزة، المتوفرة في [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) مساحة الاسم، تدمج نماذج اللغة التوليدية المتقدمة من *OpenAI* و *Google*، وكذلك *Claude's* نماذج اللغة التوليدية البشرية. تتوفر قائمة النماذج المدعومة في [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/) تعداد.

يمكنك تحديد خيارات مختلفة لتلخيص محتوى المستند. استخدم طريقة [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) لإنشاء ملخص للمستند الخاص بك. يمكنك أيضا تعيين طول الملخص باستخدام خاصية [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/).

باستخدام Aspose.Words، يكون تنفيذ تلخيص المستندات أمرا بسيطا. يوضح مثال الكود التالي كيفية تلخيص مستند باستخدام نموذج GPT-4o:

{{< highlight cpp >}}
void AiSummarize()
{
    auto firstDoc = MakeObject<Document>(MyDir + u"Big document.docx");
    auto secondDoc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"))->WithOrganization(u"Organization")->WithProject(u"Project");

    auto options = MakeObject<SummarizeOptions>();

    options->set_SummaryLength(SummaryLength::Short);
    auto firstDocumentSummary = model->Summarize(firstDoc, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.One.docx");

    System::ArrayPtr<System::SharedPtr<Document>> documents = System::MakeArray<System::SharedPtr<Document>>(2);
    documents[0] = firstDoc;
    documents[1] = secondDoc;

    options->set_SummaryLength(SummaryLength::Long);
    auto multiDocumentSummary = model->Summarize(documents, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.Multi.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

تلخيص الوثائق مع Aspose.Words يوفر الوقت ويساعدك على التركيز على المعلومات الأساسية. لمزيد من المعلومات، راجع وثائق [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}
