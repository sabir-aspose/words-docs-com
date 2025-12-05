---
title: AI Grammatikprüfung
second_title: Aspose.Words für Python via .NET
articleTitle: Grammatikprüfung
linktitle: Grammatikprüfung
type: docs
weight: 40
description: "Überprüfen Sie die Grammatik eines Dokuments. Aspose.Words für Python ermöglicht Benutzern das Überprüfen der Grammatik und das Erkennen von Fehlern in Dokumenten mithilfe der Modelle OpenAI, Google und Claude."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /de/python-net/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Die Überprüfung der Grammatik in Dokumenten ist wichtig, um Klarheit, Professionalität und Genauigkeit zu gewährleisten. Gut geschriebene Dokumente hinterlassen einen positiven Eindruck und vermeiden Missverständnisse. Grammatikprüfungen helfen, Fehler schnell zu erkennen und zu korrigieren, was Zeit spart und die Qualität verbessert.

Aspose.Words ermöglicht es Benutzern, die Grammatik zu überprüfen und Fehler in Dokumenten mithilfe der in der [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/)-Aufzählung aufgeführten Modellfamilien OpenAI, Google und Claude zu erkennen. Verwenden Sie die Methode [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), die im Namespace [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) verfügbar ist. **CheckGrammar** analysiert den Text in einem Dokument und hebt grammatikalische Probleme hervor.

Das folgende Codebeispiel zeigt, wie Sie das GPT-4o mini -Modell in Aspose.Words verwenden, um die Grammatik zu überprüfen:

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

Die Grammatikprüfung mit Aspose.Words verbessert die Qualität Ihrer Arbeit und erleichtert die Integration von Korrekturlesen in Ihre Projekte. Weitere Informationen finden Sie in der Dokumentation zu [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}