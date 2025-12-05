---
title: AI Vérification grammaticale
second_title: Aspose.Words pour Python via .NET
articleTitle: Vérification Grammaticale
linktitle: Vérification Grammaticale
type: docs
weight: 40
description: "Vérifiez la grammaire d'un document. Aspose.Words pour Python permet aux utilisateurs de vérifier la grammaire et de détecter les erreurs dans les documents à l'aide des modèles OpenAI, Google et Claude."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/python-net/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

La vérification de la grammaire dans les documents est importante pour assurer la clarté, le professionnalisme et l'exactitude. Des documents bien écrits laissent une impression positive et évitent les malentendus. Les vérifications grammaticales aident à identifier et à corriger rapidement les erreurs, ce qui permet de gagner du temps et d'améliorer la qualité.

Aspose.Words permet aux utilisateurs de vérifier la grammaire et de détecter les erreurs dans les documents en utilisant les familles de modèles OpenAI, Google et Claude répertoriées dans l'énumération [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). Utilisez la méthode [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), disponible dans l'espace de noms [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** analyse le texte d'un document et met en évidence les problèmes grammaticaux.

L'exemple de code suivant montre comment utiliser le modèle GPT-4o mini dans Aspose.Words pour vérifier la grammaire:

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

Vérifier la grammaire avec Aspose.Words améliore la qualité de votre travail et facilite l'intégration de la relecture dans vos projets. Pour plus d'informations, consultez la documentation [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}