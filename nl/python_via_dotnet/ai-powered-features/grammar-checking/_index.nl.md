---
title: AI Grammaticacontrole
second_title: Aspose.Words voor Python via .NET
articleTitle: Grammaticacontrole
linktitle: Grammaticacontrole
type: docs
weight: 40
description: "Controleer de grammatica van een document. Aspose.Words voor Python hiermee kunnen gebruikers grammatica controleren en fouten in documenten detecteren met behulp van OpenAI - modellen."
url: /nl/python-net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Het controleren van grammatica in documenten is belangrijk om duidelijkheid, professionaliteit en nauwkeurigheid te garanderen. Goed geschreven documenten laten een positieve indruk achter en voorkomen misverstanden. Grammaticacontroles helpen fouten snel te identificeren en te corrigeren, waardoor tijd wordt bespaard en de kwaliteit wordt verbeterd.

Aspose.Words stelt gebruikers in staat om grammatica te controleren en fouten in documenten te detecteren met behulp van **OpenAI** generatieve modellen. Gebruik de methode [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), Beschikbaar in de [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) naamruimte. **CheckGrammar** analyseert de tekst in een document en wijst op grammaticale problemen.

Het volgende codevoorbeeld laat zien hoe u het GPT-4o mini model in Aspose.Words gebruikt om grammatica te controleren:

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

Het controleren van grammatica met Aspose.Words verbetert de kwaliteit van uw werk en maakt het gemakkelijk om proeflezen in uw projecten te integreren. Raadpleeg de [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API documentatie voor meer informatie.

{{% /alert %}}