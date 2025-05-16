---
title: AI بررسی گرامر
second_title: Aspose.Words برای Python via .NET
articleTitle: بررسی دستور زبان
linktitle: بررسی دستور زبان
type: docs
weight: 40
description: "یک دستور زبان سند را بررسی کنید. Aspose.Words برای Python به کاربران اجازه می دهد تا گرامر را بررسی کنند و خطاهای اسناد را با استفاده از مدل های OpenAI، گوگل و Claude تشخیص دهند."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /fa/python-net/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

بررسی دستور زبان در اسناد برای اطمینان از وضوح، حرفه ای بودن و دقت مهم است. اسناد خوب نوشته شده تأثیر مثبتی بر جای می گذارند و از سوء تفاهم جلوگیری می کنند. بررسی گرامر به شناسایی و اصلاح سریع خطاها، صرفه جویی در زمان و بهبود کیفیت کمک می کند.

Aspose.Words به کاربران اجازه می دهد تا گرامر را بررسی کنند و خطاهای اسناد را با استفاده از خانواده های مدل های OpenAI، گوگل و Claude که در فهرست [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/) ذکر شده است، تشخیص دهند. از روش [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions) استفاده کنید که در فضای نام [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) موجود است. **CheckGrammar** متن را در یک سند تجزیه و تحلیل می کند و مشکلات گرامری را برجسته می کند.

مثال کد زیر نشان می دهد که چگونه از مدل GPT-4o mini در Aspose.Words برای بررسی گرامر استفاده کنید:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + 'Big document.docx')

api_key = system_helper.environment.Environment.get_environment_variable('API_KEY')
# Use OpenAI generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GPT_4O_MINI).with_api_key(api_key).as_open_ai_model()

grammar_options = aw.ai.CheckGrammarOptions()
grammar_options.improve_stylistics = True

proofed_doc = model.check_grammar(doc, grammar_options)
proofed_doc.save(file_name='AI.AiGrammar.docx')
{{< /highlight >}}

{{% alert color="primary" %}}

بررسی گرامر با Aspose.Words کیفیت کار شما را بهبود می بخشد و ادغام تصحیح را در پروژه های شما آسان می کند. برای اطلاعات بیشتر، اسناد [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API را بررسی کنید.

{{% /alert %}}