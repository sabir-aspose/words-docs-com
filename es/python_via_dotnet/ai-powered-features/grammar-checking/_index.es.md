---
title: AI Revisión gramatical
second_title: Aspose.Words por Python via .NET
articleTitle: Revisión Gramatical
linktitle: Revisión Gramatical
type: docs
weight: 40
description: "Revisa la gramática de un documento. Aspose.Words por Python permite a los usuarios verificar la gramática y detectar errores en los documentos utilizando los modelos OpenAI, Google y Claude."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /es/python-net/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Revisar la gramática en los documentos es importante para garantizar claridad, profesionalismo y precisión. Los documentos bien escritos dejan una impresión positiva y evitan malentendidos. Las revisiones gramaticales ayudan a identificar y corregir errores rápidamente, ahorrando tiempo y mejorando la calidad.

Aspose.Words permite a los usuarios verificar la gramática y detectar errores en los documentos utilizando las familias de modelos OpenAI, Google y Claude enumeradas en la enumeración [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). Utilice el método [CheckGrammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/#document_checkgrammaroptions), disponible en el espacio de nombres [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/). **CheckGrammar** analiza el texto de un documento y resalta los problemas gramaticales.

El siguiente ejemplo de código muestra cómo usar el modelo GPT-4o mini en Aspose.Words para verificar la gramática:

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

Revisar la gramática con Aspose.Words mejora la calidad de su trabajo y facilita la integración de la corrección de pruebas en sus proyectos. Para obtener más información, consulte la documentación de [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}