---
title: AI Dilbilgisi Denetimi
second_title: Aspose.Words için Python via .NET
articleTitle: Dilbilgisi Denetimi
linktitle: Dilbilgisi Denetimi
type: docs
weight: 40
description: "Bir belge dilbilgisini kontrol edin. Aspose.Words için Python kullanıcıların OpenAI modellerini kullanarak dilbilgisini kontrol etmelerine ve belgelerdeki hataları tespit etmelerine olanak tanır."
url: /tr/python-net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Belgelerdeki dilbilgisini kontrol etmek netlik, profesyonellik ve doğruluk sağlamak için önemlidir. İyi yazılmış belgeler olumlu bir izlenim bırakır ve yanlış anlaşılmalardan kaçınır. Dilbilgisi denetimleri, hataları hızlı bir şekilde tanımlamaya ve düzeltmeye yardımcı olarak zamandan tasarruf sağlar ve kaliteyi artırır.

Aspose.Words kullanıcıların **OpenAI** üretici modelleri kullanarak dilbilgisini kontrol etmelerine ve belgelerdeki hataları tespit etmelerine olanak tanır. [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) ad alanında bulunan [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions) yöntemini kullanın. **CheckGrammar** bir belgedeki metni analiz eder ve dilbilgisi sorunlarını vurgular.

Aşağıdaki kod örneği, dilbilgisini denetlemek için Aspose.Words içindeki GPT-4o mini modelinin nasıl kullanılacağını gösterir:

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

Dilbilgisini Aspose.Words ile kontrol etmek, çalışmanızın kalitesini artırır ve redaksiyonu projelerinize entegre etmeyi kolaylaştırır. Daha fazla bilgi için [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API belgelerine bakın.

{{% /alert %}}