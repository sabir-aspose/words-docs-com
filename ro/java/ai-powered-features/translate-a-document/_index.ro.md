---
title: Traduceți un Document
second_title: Aspose.Words pentru Java
articleTitle: Traduceți un Document
linktitle: Traduceți un Document
type: docs
weight: 30
description: "Traduceți un document. Aspose.Words pentru Java simplifică traducerea documentelor folosind modelele Google AI, permițându-vă să specificați limba țintă."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ro/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Traducerea documentelor este o opțiune frecvent necesară în era digitalizării ridicate. Aspose.Words acceptă traducerea documentelor folosind *Google* modele de limbaj generativ, care permite dezvoltatorilor să traducă conținutul textelor în mai mult de 300 de limbi.

Utilizați metoda [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) pentru a traduce documentele în orice limbă reprezentată în enumerarea [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). Rețineți că, dacă documentul sursă conține mai multe limbi, modelul bazat pe Google AI va putea traduce toate limbile acceptate. Dacă modelul nu poate recunoaște limba în unele fragmente de text, atunci vi se va returna un document cu aceste fragmente netraduse și cu restul textului tradus.

Următorul exemplu de cod arată cum să utilizați modelul *Gemini 1.5 Flash* în Aspose.Words pentru a traduce un document în arabă:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Traducerea documentelor cu Aspose.Words economisește timp și facilitează integrarea funcționalității de traducere în proiectele dvs. Pentru mai multe informații, verificați [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}