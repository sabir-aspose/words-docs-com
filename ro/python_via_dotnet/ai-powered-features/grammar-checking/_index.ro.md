---
title: AI Verificarea Gramaticii
second_title: Aspose.Words pentru Python via .NET
articleTitle: Verificarea Gramaticii
linktitle: Verificarea Gramaticii
type: docs
weight: 40
description: "Verificați gramatica unui document. Aspose.Words pentru Python permite utilizatorilor să verifice gramatica și să detecteze erorile din documente folosind OpenAI modele."
url: /ro/python-net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Verificarea gramaticii în documente este importantă pentru a asigura claritate, profesionalism și acuratețe. Documentele bine scrise lasă o impresie pozitivă și evită neînțelegerile. Verificările gramaticale ajută la identificarea și corectarea rapidă a erorilor, economisind timp și îmbunătățind calitatea.

Aspose.Words permite utilizatorilor să verifice gramatica și să detecteze erorile din documente folosind **OpenAI** modele generative. Utilizați metoda [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), disponibilă în spațiul de nume [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** analizează textul dintr-un document și evidențiază problemele gramaticale.

Următorul exemplu de cod arată cum să utilizați modelul GPT-4o mini în Aspose.Words pentru a verifica gramatica:

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

Verificarea gramaticii cu Aspose.Words îmbunătățește calitatea muncii dvs. și facilitează integrarea corecturii în proiectele dvs. Pentru mai multe informații, verificați documentația [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}