---
title: ترجمه یک سند
second_title: Aspose.Words برای C++
articleTitle: ترجمه یک سند
linktitle: ترجمه یک سند
type: docs
weight: 30
description: "ترجمه یک سند. Aspose.Words برای C++ ترجمه سند را با استفاده از مدل های Google AI ساده می کند و به شما امکان می دهد زبان هدف را مشخص کنید."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fa/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

ترجمه اسناد یک گزینه اغلب مورد نیاز در عصر دیجیتال سازی بالا است. Aspose.Words از ترجمه اسناد با استفاده از مدل های زبان مولد *Google* پشتیبانی می کند که به توسعه دهندگان اجازه می دهد محتوای متون را به بیش از 300 زبان ترجمه کنند.

از روش [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) برای ترجمه اسناد خود به هر زبانی که در فهرست [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) نشان داده شده است استفاده کنید. توجه داشته باشید که اگر سند منبع شامل چندین زبان باشد، مدل مبتنی بر Google AI قادر خواهد بود تمام زبان های پشتیبانی شده را ترجمه کند. اگر مدل نتواند زبان را در برخی از قطعات متن تشخیص دهد، یک سند با این قطعات ترجمه نشده و با بقیه متن ترجمه شده به شما بازگردانده می شود.

مثال کد زیر نشان می دهد که چگونه از مدل *Gemini 1.5 Flash* در Aspose.Words برای ترجمه یک سند به عربی استفاده کنیم:

{{< highlight cpp >}}
void AiTranslate()
{
    auto doc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<GoogleAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto translatedDoc = model->Translate(doc, Language::Arabic);
    translatedDoc->Save(ArtifactsDir + u"AI.AiTranslate.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

ترجمه اسناد با Aspose.Words باعث صرفه جویی در زمان می شود و ادغام قابلیت ترجمه در پروژه های شما را آسان می کند. برای اطلاعات بیشتر، اسناد [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API را بررسی کنید.

{{% /alert %}}