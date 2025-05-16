---
title: AI Kontrola Gramatiky
second_title: Aspose.Words pro Python via .NET
articleTitle: Gramatik
linktitle: Gramatik
type: docs
weight: 40
description: "Zkontrolujte gramatiku dokumentu. Aspose.Words pro Python umožňuje uživatelům kontrolovat gramatiku a detekovat chyby v dokumentech pomocí modelů OpenAI, Google a Claude."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/python-net/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Kontrola gramatiky v dokumentech je důležitá pro zajištění jasnosti, profesionality a přesnosti. Dobře napsané dokumenty zanechávají pozitivní dojem a vyhýbají se nedorozuměním. Gramatické kontroly pomáhají rychle identifikovat a opravit chyby, šetří čas a zlepšují kvalitu.

Aspose.Words umožňuje uživatelům kontrolovat gramatiku a detekovat chyby v dokumentech pomocí rodin modelů OpenAI, Google a Claude uvedených ve výčtu [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). Použijte metodu [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), která je k dispozici v oboru názvů [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** analyzuje text v dokumentu a zdůrazňuje gramatické problémy.

Následující příklad kódu ukazuje, jak použít model GPT-4o mini v Aspose.Words ke kontrole gramatiky:

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

Kontrola gramatiky pomocí Aspose.Words zlepšuje kvalitu vaší práce a usnadňuje integraci korektur do vašich projektů. Další informace najdete v dokumentaci [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}