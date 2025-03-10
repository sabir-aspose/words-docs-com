---
title: AI Grammatika-Kontrole
second_title: Aspose.Words vir Python via .NET
articleTitle: Grammatika-Kontrole
linktitle: Grammatika-Kontrole
type: docs
weight: 40
description: "Gaan'n dokumentgrammatika na. Aspose.Words vir Python laat gebruikers toe om grammatika te kontroleer en foute in dokumente op te spoor met behulp van OpenAI modelle."
url: /af/python-net/grammar-checking/
timestamp: 2025-01-15-16-40-05
---

Dit is belangrik om grammatika in dokumente te kontroleer om duidelikheid, professionaliteit en akkuraatheid te verseker. Goedgeskrewe dokumente laat'n positiewe indruk en vermy misverstande. Grammatika-kontroles help om foute vinnig te identifiseer en reg te stel, wat tyd bespaar en kwaliteit verbeter.

Aspose.Words laat gebruikers toe om grammatika te kontroleer en foute in dokumente op te spoor met behulp van **OpenAI** generatiewe modelle. Gebruik die [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions) metode, beskikbaar in die [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) naamruimte. **CheckGrammar** ontleed die teks in'n dokument en beklemtoon grammatikale probleme.

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