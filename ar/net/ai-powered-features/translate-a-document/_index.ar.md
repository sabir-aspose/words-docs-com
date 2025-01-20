---
title: ترجمة وثيقة
second_title: Aspose.Words ل .NET
articleTitle: ترجمة وثيقة
linktitle: ترجمة وثيقة
type: docs
weight: 30
description: "ترجمة وثيقة. Aspose.Words ل .NET يبسط ترجمة المستندات باستخدام نماذج جوجل AI، مما يسمح لك بتحديد اللغة الهدف."
url: /ar/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

تعد ترجمة المستندات خيارا مطلوبا بشكل متكرر في عصر الرقمنة العالية. Aspose.Words يدعم ترجمة المستندات باستخدام *Google* نماذج اللغة التوليدية، والتي تسمح للمطورين بترجمة محتوى النصوص إلى أكثر من 300 لغة.

استخدم طريقة [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) لترجمة مستنداتك إلى أي لغة ممثلة في تعداد [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). لاحظ أنه إذا كان المستند المصدر يحتوي على عدة لغات، فسيكون النموذج المستند إلى جوجل AI قادرا على ترجمة جميع اللغات المدعومة. إذا لم يتمكن النموذج من التعرف على اللغة في بعض أجزاء النص، فسيتم إرجاع مستند به هذه الأجزاء غير المترجمة ومع ترجمة بقية النص.

يوضح مثال الكود التالي كيفية استخدام نموذج *Gemini 1.5 Flash* في Aspose.Words لترجمة مستند إلى اللغة العربية:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

توفر ترجمة المستندات باستخدام Aspose.Words الوقت وتجعل من السهل دمج وظائف الترجمة في مشاريعك. لمزيد من المعلومات، راجع وثائق [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}