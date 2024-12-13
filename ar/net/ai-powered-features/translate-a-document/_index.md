---
title: ترجمة مستند
second_title: Aspose.Words for .NET
articleTitle: ترجمة مستند
linktitle: ترجمة مستند
type: docs
weight: 30
description: "ترجمة مستند. يبسط Aspose.Words for .NET ترجمة المستندات باستخدام نماذج Google AI، مما يسمح لك بتحديد اللغة المستهدفة."
url: /ar/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

تعد ترجمة المستندات خيارًا مطلوبًا بشكل متكرر في عصر الرقمنة العالية. يدعم Aspose.Words ترجمة المستندات باستخدام نماذج اللغة التوليدية *Google*، والتي تسمح للمطورين بترجمة محتوى النصوص إلى أكثر من 300 لغة.

استخدم طريقة [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) لترجمة مستنداتك إلى أي لغة ممثلة في تعداد [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). لاحظ أنه إذا كان المستند المصدر يحتوي على عدة لغات، فسيكون نموذج Google AI قادرًا على ترجمة جميع اللغات المدعومة. إذا لم يتمكن النموذج من التعرف على اللغة في بعض أجزاء النص، فسيتم إرجاع مستند إليك يحتوي على هذه الأجزاء غير المترجمة وبقية النص المترجم.

يوضح مثال التعليمات البرمجية التالي كيفية استخدام نموذج *Gemini 1.5 Flash* في Aspose.Words لترجمة مستند إلى اللغة العربية:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

ترجمة المستندات باستخدام Aspose.Words توفر الوقت وتسهل دمج وظيفة الترجمة في مشاريعك. لمزيد من المعلومات، راجع وثائق واجهة برمجة التطبيقات [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

{{% /alert %}}