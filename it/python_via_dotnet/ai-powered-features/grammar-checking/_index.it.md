---
title: AI Controllo grammaticale
second_title: Aspose.Words per Python via .NET
articleTitle: Controllo grammaticale
linktitle: Controllo grammaticale
type: docs
weight: 40
description: "Controllare la grammatica di un documento. Aspose.Wordsper Python consente agli utenti di controllare la grammatica e rilevare errori nei documenti utilizzando i modelli OpenAI."
url: /it/python-net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Controllare la grammatica nei documenti è importante per garantire chiarezza, professionalità e accuratezza. I documenti ben scritti lasciano un'impressione positiva ed evitano malintesi. I controlli grammaticali aiutano a identificare e correggere rapidamente gli errori, risparmiando tempo e migliorando la qualità.

Aspose.Words consente agli utenti di controllare la grammatica e rilevare errori nei documenti utilizzando modelli generativi **OpenAI**. Utilizzare il metodo [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), disponibile nello spazio dei nomi [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** analizza il testo di un documento ed evidenzia i problemi grammaticali.

Il seguente esempio di codice mostra come utilizzare il modello GPT-4o mini in Aspose.Words per controllare la grammatica:

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

Il controllo della grammatica con Aspose.Words migliora la qualità del tuo lavoro e semplifica l'integrazione della correzione di bozze nei tuoi progetti. Per ulteriori informazioni, controllare la documentazione [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}