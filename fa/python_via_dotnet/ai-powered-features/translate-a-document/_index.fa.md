---
title: ترجمه یک سند
second_title: Aspose.Words برای Python via .NET
articleTitle: ترجمه یک سند
linktitle: ترجمه یک سند
type: docs
weight: 30
description: "ترجمه یک سند. Aspose.Words برای Python ترجمه سند را با استفاده از مدل های Google AI ساده می کند و به شما امکان می دهد زبان هدف را مشخص کنید."
url: /fa/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

ترجمه اسناد یک گزینه اغلب مورد نیاز در عصر دیجیتال سازی بالا است. Aspose.Words از ترجمه اسناد با استفاده از مدل های زبان مولد *Google* پشتیبانی می کند که به توسعه دهندگان اجازه می دهد محتوای متون را به بیش از 300 زبان ترجمه کنند.

از روش [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) برای ترجمه اسناد خود به هر زبانی که در فهرست [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) نشان داده شده است استفاده کنید. توجه داشته باشید که اگر سند منبع شامل چندین زبان باشد، مدل مبتنی بر Google AI قادر خواهد بود تمام زبان های پشتیبانی شده را ترجمه کند. اگر مدل نتواند زبان را در برخی از قطعات متن تشخیص دهد، یک سند با این قطعات ترجمه نشده و با بقیه متن ترجمه شده به شما بازگردانده می شود.

مثال کد زیر نشان می دهد که چگونه از مدل *Gemini 1.5 Flash* در Aspose.Words برای ترجمه یک سند به عربی استفاده کنیم:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

ترجمه اسناد با Aspose.Words باعث صرفه جویی در زمان می شود و ادغام قابلیت ترجمه در پروژه های شما را آسان می کند. برای اطلاعات بیشتر، اسناد [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API را بررسی کنید.

{{% /alert %}}