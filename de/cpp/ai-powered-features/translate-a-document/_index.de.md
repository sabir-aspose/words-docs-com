---
title: Ein Dokument übersetzen
second_title: Aspose.Words für C++
articleTitle: Ein Dokument übersetzen
linktitle: Ein Dokument übersetzen
type: docs
weight: 30
description: "Übersetzen Sie ein Dokument. Aspose.Words für C++ vereinfacht die Übersetzung von Dokumenten mithilfe von Google AI -Modellen, sodass Sie die Zielsprache angeben können."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /de/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Die Übersetzung von Dokumenten ist eine häufig benötigte Option im Zeitalter der hohen Digitalisierung. Aspose.Words unterstützt die Übersetzung von Dokumenten mithilfe von *Google* generativen Sprachmodellen, mit denen Entwickler Textinhalte in mehr als 300 Sprachen übersetzen können.

Verwenden Sie die [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/)-Methode, um Ihre Dokumente in eine beliebige Sprache zu übersetzen, die in der [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/)-Aufzählung dargestellt wird. Beachten Sie, dass das Google AI-basierte Modell alle unterstützten Sprachen übersetzen kann, wenn das Quelldokument mehrere Sprachen enthält. Wenn das Modell die Sprache in einigen Textfragmenten nicht erkennen kann, erhalten Sie ein Dokument mit diesen nicht übersetzten Fragmenten und dem Rest des übersetzten Textes zurück.

Das folgende Codebeispiel zeigt, wie Sie das *Gemini 1.5 Flash* -Modell in Aspose.Words verwenden, um ein Dokument ins Arabische zu übersetzen:

{{< highlight cpp >}}
void AiTranslate()
{
    auto doc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<GoogleAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto translatedDoc = model->Translate(doc, Language::Arabic);
    translatedDoc->Save(ArtifactsDir + u"AI.AiTranslate.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Das Übersetzen von Dokumenten mit Aspose.Words spart Zeit und erleichtert die Integration von Übersetzungsfunktionen in Ihre Projekte. Weitere Informationen finden Sie in der Dokumentation zu [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}