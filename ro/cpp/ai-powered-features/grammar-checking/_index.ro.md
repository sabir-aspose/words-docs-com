---
title: AI Verificarea Gramaticii
second_title: Aspose.Words pentru C++
articleTitle: Verificarea Gramaticii
linktitle: Verificarea Gramaticii
type: docs
weight: 40
description: "Verificați gramatica unui document. Aspose.Words Pentru C++ permite utilizatorilor să verifice gramatica și să detecteze erorile din documente folosind modelele OpenAI, Google și Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ro/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Verificarea gramaticii în documente este importantă pentru a asigura claritate, profesionalism și acuratețe. Documentele bine scrise lasă o impresie pozitivă și evită neînțelegerile. Verificările gramaticale ajută la identificarea și corectarea rapidă a erorilor, economisind timp și îmbunătățind calitatea.

Aspose.Words permite utilizatorilor să verifice gramatica și să detecteze erorile din documente folosind familiile modelelor OpenAI, Google și Claude enumerate în enumerarea [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). Utilizați metoda [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), disponibilă în spațiul de nume [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** analizează textul dintr-un document și evidențiază problemele gramaticale.

Următorul exemplu de cod arată cum să utilizați modelul GPT-4o mini în Aspose.Words pentru a verifica gramatica:

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

Verificarea gramaticii cu Aspose.Words îmbunătățește calitatea muncii dvs. și facilitează integrarea corecturii în proiectele dvs. Pentru mai multe informații, verificați documentația [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}