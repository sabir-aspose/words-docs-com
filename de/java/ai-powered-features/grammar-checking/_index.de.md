---
title: AI Grammatikprüfung
second_title: Aspose.Words für Java
articleTitle: Grammatikprüfung
linktitle: Grammatikprüfung
type: docs
weight: 40
description: "Überprüfen Sie die Grammatik eines Dokuments. Aspose.Words für Java ermöglicht Benutzern das Überprüfen der Grammatik und das Erkennen von Fehlern in Dokumenten mithilfe der Modelle OpenAI, Google und Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /de/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Die Überprüfung der Grammatik in Dokumenten ist wichtig, um Klarheit, Professionalität und Genauigkeit zu gewährleisten. Gut geschriebene Dokumente hinterlassen einen positiven Eindruck und vermeiden Missverständnisse. Grammatikprüfungen helfen, Fehler schnell zu erkennen und zu korrigieren, was Zeit spart und die Qualität verbessert.

Aspose.Words ermöglicht es Benutzern, die Grammatik zu überprüfen und Fehler in Dokumenten mithilfe der in der [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/)-Aufzählung aufgeführten Modellfamilien OpenAI, Google und Claude zu erkennen. Verwenden Sie die [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) -Methode, um den Text in einem Dokument zu analysieren und grammatikalische Probleme hervorzuheben.

Das folgende Codebeispiel zeigt, wie Sie das GPT-4o mini -Modell in Aspose.Words verwenden, um die Grammatik zu überprüfen:

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

Die Grammatikprüfung mit Aspose.Words verbessert die Qualität Ihrer Arbeit und erleichtert die Integration von Korrekturlesen in Ihre Projekte. Für weitere Informationen überprüfen Sie die [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}