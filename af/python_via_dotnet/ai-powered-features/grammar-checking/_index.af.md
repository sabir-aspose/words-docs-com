---
title: AI Grammatika-Kontrole
second_title: Aspose.Words vir Python via .NET
articleTitle: Grammatika-Kontrole
linktitle: Grammatika-Kontrole
type: docs
weight: 40
description: "Gaan'n dokumentgrammatika na. Aspose.Words vir Python laat gebruikers toe om grammatika te kontroleer en foute in dokumente op te spoor met behulp van OpenAI, Google en Claude modelle."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /af/python-net/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Dit is belangrik om grammatika in dokumente te kontroleer om duidelikheid, professionaliteit en akkuraatheid te verseker. Goedgeskrewe dokumente laat'n positiewe indruk en vermy misverstande. Grammatika-kontroles help om foute vinnig te identifiseer en reg te stel, wat tyd bespaar en kwaliteit verbeter.

Aspose.Words laat gebruikers toe om grammatika te kontroleer en foute in dokumente op te spoor deur die OpenAI, Google en Claude modelle se families te gebruik wat in die [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/) opsomming gelys word. Gebruik die [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions) metode, beskikbaar in die [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) naamruimte. **CheckGrammar** ontleed die teks in'n dokument en beklemtoon grammatikale probleme.

Die volgende kode voorbeeld toon hoe om die GPT-4o mini model in Aspose.Words te gebruik om grammatika te kontroleer:

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

Die nagaan van grammatika met Aspose.Words verbeter die kwaliteit van u werk en maak dit maklik om proeflees in u projekte te integreer. Vir meer inligting, kyk na die [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API dokumentasie.

{{% /alert %}}