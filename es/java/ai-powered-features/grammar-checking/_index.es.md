---
title: AI Revisión gramatical
second_title: Aspose.Words por Java
articleTitle: Revisión Gramatical
linktitle: Revisión Gramatical
type: docs
weight: 40
description: "Revisa la gramática de un documento. Aspose.Words por Java permite a los usuarios verificar la gramática y detectar errores en los documentos utilizando los modelos OpenAI, Google y Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /es/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Revisar la gramática en los documentos es importante para garantizar claridad, profesionalismo y precisión. Los documentos bien escritos dejan una impresión positiva y evitan malentendidos. Las revisiones gramaticales ayudan a identificar y corregir errores rápidamente, ahorrando tiempo y mejorando la calidad.

Aspose.Words permite a los usuarios verificar la gramática y detectar errores en los documentos utilizando las familias de modelos OpenAI, Google y Claude enumeradas en la enumeración [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). Utilice el método [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) para analizar el texto de un documento y resaltar problemas gramaticales.

El siguiente ejemplo de código muestra cómo usar el modelo GPT-4o mini en Aspose.Words para verificar la gramática:

{{< highlight java >}}
 Document doc = new Document("Big document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI generative language models.
 IAiModelText model = (OpenAiModel)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
 grammarOptions.setImproveStylistics(true);

 Document proofedDoc = model.checkGrammar(doc, grammarOptions);
 proofedDoc.save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Revisar la gramática con Aspose.Words mejora la calidad de su trabajo y facilita la integración de la corrección de pruebas en sus proyectos. Para obtener más información, marque [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}