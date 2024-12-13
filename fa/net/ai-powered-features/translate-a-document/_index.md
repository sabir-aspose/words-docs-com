---
title: ترجمه یک سند
second_title: Aspose.Words برای دات نت
articleTitle: ترجمه یک سند
linktitle: ترجمه یک سند
type: docs
weight: 30
description: "یک سند را ترجمه کنید Aspose.Words for .NET ترجمه سند را با استفاده از مدل های هوش مصنوعی گوگل ساده می کند و به شما امکان می دهد زبان مقصد را مشخص کنید."
url: /fa/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

ترجمه سند در عصر دیجیتالی شدن بالا گزینه ای است که اغلب مورد نیاز است. Aspose.Words از ترجمه سند با استفاده از مدل‌های زبانی *Google* پشتیبانی می‌کند، که به توسعه‌دهندگان اجازه می‌دهد محتوای متون را به بیش از 300 زبان ترجمه کنند.

از روش [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) برای ترجمه اسناد خود به هر زبانی که در [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) ارائه شده است استفاده کنید  شمارش. توجه داشته باشید که اگر سند منبع حاوی چندین زبان باشد، مدل مبتنی بر هوش مصنوعی گوگل می‌تواند تمام زبان‌های پشتیبانی شده را ترجمه کند. اگر مدل نتواند زبان را در برخی از قطعات متن تشخیص دهد، سندی با این قطعات ترجمه نشده و با بقیه متن ترجمه شده به شما برگردانده می شود.

مثال کد زیر نحوه استفاده از مدل *Gemini 1.5 Flash* را در Aspose.Words برای ترجمه یک سند به عربی نشان می دهد:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

 Aspose.Words در زمان صرفه جویی می کند و ادغام قابلیت ترجمه در پروژه های شما را آسان می کند. برای اطلاعات بیشتر، اسناد API [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) را بررسی کنید.

{{% /alert %}}