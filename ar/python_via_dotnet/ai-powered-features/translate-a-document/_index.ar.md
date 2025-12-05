---
title: ترجمة وثيقة
second_title: Aspose.Words ل Python via .NET
articleTitle: ترجمة وثيقة
linktitle: ترجمة وثيقة
type: docs
weight: 30
description: "ترجمة وثيقة. Aspose.Words ل Python يبسط ترجمة المستندات باستخدام نماذج جوجل AI، مما يسمح لك بتحديد اللغة الهدف."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ar/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

تعد ترجمة المستندات خيارا مطلوبا بشكل متكرر في عصر الرقمنة العالية. Aspose.Words يدعم ترجمة المستندات باستخدام *Google* نماذج اللغة التوليدية، والتي تسمح للمطورين بترجمة محتوى النصوص إلى أكثر من 300 لغة.

استخدم طريقة [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) لترجمة مستنداتك إلى أي لغة ممثلة في تعداد [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). لاحظ أنه إذا كان المستند المصدر يحتوي على عدة لغات، فسيكون النموذج المستند إلى جوجل AI قادرا على ترجمة جميع اللغات المدعومة. إذا لم يتمكن النموذج من التعرف على اللغة في بعض أجزاء النص، فسيتم إرجاع مستند به هذه الأجزاء غير المترجمة ومع ترجمة بقية النص.

يوضح مثال الكود التالي كيفية استخدام نموذج *Gemini 1.5 Flash* في Aspose.Words لترجمة مستند إلى اللغة العربية:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

توفر ترجمة المستندات باستخدام Aspose.Words الوقت وتجعل من السهل دمج وظائف الترجمة في مشاريعك. لمزيد من المعلومات، راجع وثائق [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}