---
title: Traduceți un Document
second_title: Aspose.Words pentru .NET
articleTitle: Traduceți un Document
linktitle: Traduceți un Document
type: docs
weight: 30
description: "Traduceți un document. Aspose.Words pentru .NET simplifică traducerea documentelor folosind modelele Google AI, permițându-vă să specificați limba țintă."
url: /ro/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Traducerea documentelor este o opțiune frecvent necesară în era digitalizării ridicate. Aspose.Words acceptă traducerea documentelor folosind *Google* modele de limbaj generativ, care permite dezvoltatorilor să traducă conținutul textelor în mai mult de 300 de limbi.

Utilizați metoda [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) pentru a traduce documentele în orice limbă reprezentată în enumerarea [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Rețineți că, dacă documentul sursă conține mai multe limbi, modelul bazat pe Google AI va putea traduce toate limbile acceptate. Dacă modelul nu poate recunoaște limba în unele fragmente de text, atunci vi se va returna un document cu aceste fragmente netraduse și cu restul textului tradus.

Următorul exemplu de cod arată cum să utilizați modelul *Gemini 1.5 Flash* în Aspose.Words pentru a traduce un document în arabă:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Traducerea documentelor cu Aspose.Words economisește timp și facilitează integrarea funcționalității de traducere în proiectele dvs. Pentru mai multe informații, verificați documentația [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}