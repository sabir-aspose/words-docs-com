---
title: Ein Dokument übersetzen
second_title: Aspose.Words für Python via .NET
articleTitle: Ein Dokument übersetzen
linktitle: Ein Dokument übersetzen
type: docs
weight: 30
description: "Übersetzen Sie ein Dokument. Aspose.Words für Python vereinfacht die Übersetzung von Dokumenten mithilfe von Google AI -Modellen, sodass Sie die Zielsprache angeben können."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /de/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Die Übersetzung von Dokumenten ist eine häufig benötigte Option im Zeitalter der hohen Digitalisierung. Aspose.Words unterstützt die Übersetzung von Dokumenten mithilfe von *Google* generativen Sprachmodellen, mit denen Entwickler Textinhalte in mehr als 300 Sprachen übersetzen können.

Verwenden Sie die [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language)-Methode, um Ihre Dokumente in eine beliebige Sprache zu übersetzen, die in der [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/)-Aufzählung dargestellt wird. Beachten Sie, dass das Google AI-basierte Modell alle unterstützten Sprachen übersetzen kann, wenn das Quelldokument mehrere Sprachen enthält. Wenn das Modell die Sprache in einigen Textfragmenten nicht erkennen kann, erhalten Sie ein Dokument mit diesen nicht übersetzten Fragmenten und dem Rest des übersetzten Textes zurück.

Das folgende Codebeispiel zeigt, wie Sie das *Gemini 1.5 Flash* -Modell in Aspose.Words verwenden, um ein Dokument ins Arabische zu übersetzen:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Das Übersetzen von Dokumenten mit Aspose.Words spart Zeit und erleichtert die Integration von Übersetzungsfunktionen in Ihre Projekte. Weitere Informationen finden Sie in der Dokumentation zu [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}