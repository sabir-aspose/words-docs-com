---
title: AI بررسی گرامر
second_title: Aspose.Words برای .NET
articleTitle: بررسی دستور زبان
linktitle: بررسی دستور زبان
type: docs
weight: 40
description: "یک دستور زبان سند را بررسی کنید. Aspose.Words برای .NET به کاربران اجازه می دهد تا گرامر را بررسی کنند و خطاهای اسناد را با استفاده از مدل های OpenAI تشخیص دهند."
url: /fa/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

بررسی دستور زبان در اسناد برای اطمینان از وضوح، حرفه ای بودن و دقت مهم است. اسناد خوب نوشته شده تأثیر مثبتی بر جای می گذارند و از سوء تفاهم جلوگیری می کنند. بررسی گرامر به شناسایی و اصلاح سریع خطاها، صرفه جویی در زمان و بهبود کیفیت کمک می کند.

Aspose.Words به کاربران اجازه می دهد تا گرامر را بررسی کنند و خطاهای اسناد را با استفاده از مدل های مولد **OpenAI** تشخیص دهند. از روش [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/) استفاده کنید که در فضای نام [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) موجود است. **CheckGrammar** متن را در یک سند تجزیه و تحلیل می کند و مشکلات گرامری را برجسته می کند.

مثال کد زیر نشان می دهد که چگونه از مدل GPT-4o mini در Aspose.Words برای بررسی گرامر استفاده کنید:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Big document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use OpenAI generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gpt4OMini).WithApiKey(apiKey);

CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
grammarOptions.ImproveStylistics = true;

Document proofedDoc = model.CheckGrammar(doc, grammarOptions);
proofedDoc.Save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

بررسی گرامر با Aspose.Words کیفیت کار شما را بهبود می بخشد و ادغام تصحیح را در پروژه های شما آسان می کند. برای اطلاعات بیشتر، اسناد [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API را بررسی کنید.

{{% /alert %}}