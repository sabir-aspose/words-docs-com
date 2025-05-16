---
title: AI Sprawdzanie Gramatyki
second_title: Aspose.Words dla Python via .NET
articleTitle: Sprawdzanie Gramatyki
linktitle: Sprawdzanie Gramatyki
type: docs
weight: 40
description: "Sprawdź gramatykę dokumentu. Aspose.Words dla Python umożliwia użytkownikom sprawdzanie gramatyki i wykrywanie błędów w dokumentach za pomocą modeli OpenAI, Google i Claude."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pl/python-net/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Sprawdzanie gramatyki w dokumentach jest ważne, aby zapewnić jasność, profesjonalizm i dokładność. Dobrze napisane dokumenty pozostawiają pozytywne wrażenie i unikają nieporozumień. Sprawdzanie gramatyki pomaga szybko identyfikować i poprawiać błędy, oszczędzając czas i poprawiając jakość.

Aspose.Words umożliwia użytkownikom sprawdzanie gramatyki i wykrywanie błędów w dokumentach przy użyciu rodzin modeli OpenAI, Google i Claude wymienionych w wyliczeniu [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). Użyj metody [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), dostępnej w przestrzeni nazw [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** analizuje tekst w dokumencie i podkreśla problemy gramatyczne.

Poniższy przykład kodu pokazuje, jak używać modelu GPT-4o mini w Aspose.Words do sprawdzania gramatyki:

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

Sprawdzanie gramatyki za pomocą Aspose.Words poprawia jakość pracy i ułatwia integrację korekty z projektami. Aby uzyskać więcej informacji, sprawdź dokumentację [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}