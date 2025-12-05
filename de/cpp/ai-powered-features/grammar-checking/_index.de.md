---
title: AI Grammatikprüfung
second_title: Aspose.Words für C++
articleTitle: Grammatikprüfung
linktitle: Grammatikprüfung
type: docs
weight: 40
description: "Überprüfen Sie die Grammatik eines Dokuments. Aspose.Words für C++ ermöglicht Benutzern das Überprüfen der Grammatik und das Erkennen von Fehlern in Dokumenten mithilfe der Modelle OpenAI, Google und Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /de/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Die Überprüfung der Grammatik in Dokumenten ist wichtig, um Klarheit, Professionalität und Genauigkeit zu gewährleisten. Gut geschriebene Dokumente hinterlassen einen positiven Eindruck und vermeiden Missverständnisse. Grammatikprüfungen helfen, Fehler schnell zu erkennen und zu korrigieren, was Zeit spart und die Qualität verbessert.

Aspose.Words ermöglicht es Benutzern, die Grammatik zu überprüfen und Fehler in Dokumenten mithilfe der in der [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/)-Aufzählung aufgeführten Modellfamilien OpenAI, Google und Claude zu erkennen. Verwenden Sie die Methode [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), die im Namespace [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) verfügbar ist. **CheckGrammar** analysiert den Text in einem Dokument und hebt grammatikalische Probleme hervor.

Das folgende Codebeispiel zeigt, wie Sie das GPT-4o mini -Modell in Aspose.Words verwenden, um die Grammatik zu überprüfen:

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

Die Grammatikprüfung mit Aspose.Words verbessert die Qualität Ihrer Arbeit und erleichtert die Integration von Korrekturlesen in Ihre Projekte. Weitere Informationen finden Sie in der Dokumentation zu [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}