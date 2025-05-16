---
title: Vertaal'n Dokument
second_title: Aspose.Words vir Python via .NET
articleTitle: Vertaal'n Dokument
linktitle: Vertaal'n Dokument
type: docs
weight: 30
description: "Vertaal'n dokument. Aspose.Words vir Python vereenvoudig dokumentvertaling met Behulp Van Google AI modelle, sodat jy die teikentaal kan spesifiseer."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /af/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Dokumentvertaling is'n dikwels benodigde opsie in die era van hoë digitalisering. Aspose.Words ondersteun dokumentvertaling met behulp van *Google* generatiewe taalmodelle, wat ontwikkelaars toelaat om teksinhoud in meer as 300 tale te vertaal.

Gebruik die [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) metode om jou dokumente te vertaal in enige taal wat in die [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) opsomming verteenwoordig word. Let daarop dat as die brondokument verskeie tale bevat, Die Google AI-gebaseerde model alle ondersteunde tale kan vertaal. As die model nie die taal in sommige teksfragmente kan herken nie, sal u'n dokument met hierdie ongetranslateerde fragmente en met die res van die teks vertaal word.

Die volgende kode voorbeeld toon hoe om die *Gemini 1.5 Flash* model in Aspose.Words te gebruik om'n dokument in arabies te vertaal:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Die vertaling van dokumente met Aspose.Words bespaar tyd en maak dit maklik om vertaalfunksionaliteit in u projekte te integreer. Vir meer inligting, kyk na die [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API dokumentasie.

{{% /alert %}}