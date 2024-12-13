---
title: Dokument übersetzen
second_title: Aspose.Words für .NET
articleTitle: Dokument übersetzen
linktitle: Dokument übersetzen
type: docs
weight: 30
description: "Dokument übersetzen. Aspose.Words für .NET vereinfacht die Dokumentübersetzung mithilfe von Google AI-Modellen und ermöglicht Ihnen, die Zielsprache anzugeben."
url: /de/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Dokumentenübersetzung ist im Zeitalter der Hochdigitalisierung eine häufig benötigte Option. Aspose.Words unterstützt die Dokumentübersetzung mithilfe von *Google*-generativen Sprachmodellen, wodurch Entwickler Textinhalte in mehr als 300 Sprachen übersetzen können.

Verwenden Sie die Methode [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/), um Ihre Dokumente in jede Sprache zu übersetzen, die in der Aufzählung [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) dargestellt ist. Beachten Sie, dass das auf Google AI basierende Modell alle unterstützten Sprachen übersetzen kann, wenn das Quelldokument mehrere Sprachen enthält. Wenn das Modell die Sprache in einigen Textfragmenten nicht erkennen kann, wird Ihnen ein Dokument mit diesen nicht übersetzten Fragmenten und dem übersetzten Rest des Textes zurückgegeben.

Das folgende Codebeispiel zeigt, wie Sie das Modell *Gemini 1.5 Flash* in Aspose.Words verwenden, um ein Dokument ins Arabische zu übersetzen:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Das Übersetzen von Dokumenten mit Aspose.Words spart Zeit und erleichtert die Integration von Übersetzungsfunktionen in Ihre Projekte. Weitere Informationen finden Sie in der [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API-Dokumentation.

{{% /alert %}}