---
title: AI Revisión gramatical
second_title: Aspose.Words por C++
articleTitle: Revisión Gramatical
linktitle: Revisión Gramatical
type: docs
weight: 40
description: "Revisa la gramática de un documento. Aspose.Words por C++ permite a los usuarios verificar la gramática y detectar errores en los documentos utilizando los modelos OpenAI, Google y Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /es/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Revisar la gramática en los documentos es importante para garantizar claridad, profesionalismo y precisión. Los documentos bien escritos dejan una impresión positiva y evitan malentendidos. Las revisiones gramaticales ayudan a identificar y corregir errores rápidamente, ahorrando tiempo y mejorando la calidad.

Aspose.Words permite a los usuarios verificar la gramática y detectar errores en los documentos utilizando las familias de modelos OpenAI, Google y Claude enumeradas en la enumeración [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). Utilice el método [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), disponible en el espacio de nombres [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** analiza el texto de un documento y resalta los problemas gramaticales.

El siguiente ejemplo de código muestra cómo usar el modelo GPT-4o mini en Aspose.Words para verificar la gramática:

{{< highlight cpp >}}
void AiGrammar()
{
    auto doc = MakeObject<Document>(MyDir + u"Big document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto grammarOptions = MakeObject<CheckGrammarOptions>();
    grammarOptions->set_ImproveStylistics(true);

    auto proofedDoc = model->CheckGrammar(doc, grammarOptions);
    proofedDoc->Save(ArtifactsDir + u"AI.AiGrammar.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Revisar la gramática con Aspose.Words mejora la calidad de su trabajo y facilita la integración de la corrección de pruebas en sus proyectos. Para obtener más información, consulte la documentación de [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}