---
title: Traduceți un Document
second_title: Aspose.Words pentru Python via .NET
articleTitle: Traduceți un Document
linktitle: Traduceți un Document
type: docs
weight: 30
description: "Traduceți un document. Aspose.Words pentru Python simplifică traducerea documentelor folosind modelele Google AI, permițându-vă să specificați limba țintă."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ro/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Traducerea documentelor este o opțiune frecvent necesară în era digitalizării ridicate. Aspose.Words acceptă traducerea documentelor folosind *Google* modele de limbaj generativ, care permite dezvoltatorilor să traducă conținutul textelor în mai mult de 300 de limbi.

Utilizați metoda [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) pentru a traduce documentele în orice limbă reprezentată în enumerarea [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). Rețineți că, dacă documentul sursă conține mai multe limbi, modelul bazat pe Google AI va putea traduce toate limbile acceptate. Dacă modelul nu poate recunoaște limba în unele fragmente de text, atunci vi se va returna un document cu aceste fragmente netraduse și cu restul textului tradus.

Următorul exemplu de cod arată cum să utilizați modelul *Gemini 1.5 Flash* în Aspose.Words pentru a traduce un document în arabă:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Traducerea documentelor cu Aspose.Words economisește timp și facilitează integrarea funcționalității de traducere în proiectele dvs. Pentru mai multe informații, verificați documentația [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}