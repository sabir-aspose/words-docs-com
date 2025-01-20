---
title: AI Grammatikprüfung
second_title: Aspose.Words für .NET
articleTitle: Grammatikprüfung
linktitle: Grammatikprüfung
type: docs
weight: 40
description: "Überprüfen Sie die Grammatik eines Dokuments. Aspose.Words für .NET ermöglicht Benutzern das Überprüfen der Grammatik und das Erkennen von Fehlern in Dokumenten mithilfe von OpenAI -Modellen."
url: /de/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Die Überprüfung der Grammatik in Dokumenten ist wichtig, um Klarheit, Professionalität und Genauigkeit zu gewährleisten. Gut geschriebene Dokumente hinterlassen einen positiven Eindruck und vermeiden Missverständnisse. Grammatikprüfungen helfen, Fehler schnell zu erkennen und zu korrigieren, was Zeit spart und die Qualität verbessert.

Aspose.Words ermöglicht es Benutzern, Grammatik zu überprüfen und Fehler in Dokumenten mithilfe generativer **OpenAI**-Modelle zu erkennen. Verwenden Sie die Methode [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), die im Namespace [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) verfügbar ist. **CheckGrammar** analysiert den Text in einem Dokument und hebt grammatikalische Probleme hervor.

Das folgende Codebeispiel zeigt, wie Sie das GPT-4o mini -Modell in Aspose.Words verwenden, um die Grammatik zu überprüfen:

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

Die Grammatikprüfung mit Aspose.Words verbessert die Qualität Ihrer Arbeit und erleichtert die Integration von Korrekturlesen in Ihre Projekte. Weitere Informationen finden Sie in der Dokumentation zu [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}