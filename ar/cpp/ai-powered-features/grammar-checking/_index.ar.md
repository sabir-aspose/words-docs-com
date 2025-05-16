---
title: AI التدقيق النحوي
second_title: Aspose.Words ل C++
articleTitle: التدقيق النحوي
linktitle: التدقيق النحوي
type: docs
weight: 40
description: "تحقق من قواعد المستند. Aspose.Words ل C++ يسمح للمستخدمين بالتحقق من القواعد واكتشاف الأخطاء في المستندات باستخدام نماذج OpenAI وجوجل و Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ar/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

يعد التحقق من القواعد في المستندات أمرا مهما لضمان الوضوح والاحتراف والدقة. تترك المستندات المكتوبة جيدا انطباعا إيجابيا وتتجنب سوء الفهم. تساعد عمليات التدقيق النحوي في تحديد الأخطاء وتصحيحها بسرعة، مما يوفر الوقت ويحسن الجودة.

Aspose.Words يسمح للمستخدمين بالتحقق من القواعد واكتشاف الأخطاء في المستندات باستخدام عائلات النماذج OpenAI وجوجل و Claude المدرجة في تعداد [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). استخدم طريقة [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/)، المتوفرة في مساحة الاسم [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** يحلل النص في وثيقة ويسلط الضوء على المشاكل النحوية.

يوضح مثال الكود التالي كيفية استخدام نموذج GPT-4o mini في Aspose.Words للتحقق من القواعد:

{{< highlight cpp >}}
void AiGrammar()
{
    auto doc = MakeObject<Document>(MyDir + u"Big document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto grammarOptions = MakeObject<CheckGrammarOptions>();
    grammarOptions->set_ImproveStylistics(true);

    auto proofedDoc = model->CheckGrammar(doc, grammarOptions);
    proofedDoc->Save(ArtifactsDir + u"AI.AiGrammar.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

يؤدي التحقق من القواعد باستخدام Aspose.Words إلى تحسين جودة عملك ويجعل من السهل دمج التدقيق اللغوي في مشاريعك. لمزيد من المعلومات، راجع وثائق [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}