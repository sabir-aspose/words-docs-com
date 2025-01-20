---
title: AI Revisión gramatical
second_title: Aspose.Words por .NET
articleTitle: Revisión Gramatical
linktitle: Revisión Gramatical
type: docs
weight: 40
description: "Revisa la gramática de un documento. Aspose.Words por .NET permite a los usuarios verificar la gramática y detectar errores en los documentos utilizando modelos OpenAI."
url: /es/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Revisar la gramática en los documentos es importante para garantizar claridad, profesionalismo y precisión. Los documentos bien escritos dejan una impresión positiva y evitan malentendidos. Las revisiones gramaticales ayudan a identificar y corregir errores rápidamente, ahorrando tiempo y mejorando la calidad.

Aspose.Words permite a los usuarios verificar la gramática y detectar errores en los documentos utilizando **OpenAI** modelos generativos. Utilice el método [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), disponible en el espacio de nombres [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/). **CheckGrammar** analiza el texto de un documento y resalta los problemas gramaticales.

El siguiente ejemplo de código muestra cómo usar el modelo GPT-4o mini en Aspose.Words para verificar la gramática:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Big document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use OpenAI generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gpt4OMini).WithApiKey(apiKey);

CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
grammarOptions.ImproveStylistics = true;

Document proofedDoc = model.CheckGrammar(doc, grammarOptions);
proofedDoc.Save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Revisar la gramática con Aspose.Words mejora la calidad de su trabajo y facilita la integración de la corrección de pruebas en sus proyectos. Para obtener más información, consulte la documentación de [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}