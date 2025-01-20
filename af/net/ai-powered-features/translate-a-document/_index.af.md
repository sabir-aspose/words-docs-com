---
title: Vertaal'n Dokument
second_title: Aspose.Words vir .NET
articleTitle: Vertaal'n Dokument
linktitle: Vertaal'n Dokument
type: docs
weight: 30
description: "Vertaal'n dokument. Aspose.Words vir .NET vereenvoudig dokumentvertaling met Behulp Van Google AI modelle, sodat jy die teikentaal kan spesifiseer."
url: /af/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Dokumentvertaling is'n dikwels benodigde opsie in die era van hoë digitalisering. Aspose.Words ondersteun dokumentvertaling met behulp van *Google* generatiewe taalmodelle, wat ontwikkelaars toelaat om teksinhoud in meer as 300 tale te vertaal.

Gebruik die [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) metode om jou dokumente te vertaal in enige taal wat in die [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) opsomming verteenwoordig word. Let daarop dat as die brondokument verskeie tale bevat, Die Google AI-gebaseerde model alle ondersteunde tale kan vertaal. As die model nie die taal in sommige teksfragmente kan herken nie, sal u'n dokument met hierdie ongetranslateerde fragmente en met die res van die teks vertaal word.

Die volgende kode voorbeeld toon hoe om die *Gemini 1.5 Flash* model in Aspose.Words te gebruik om'n dokument in arabies te vertaal:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Die vertaling van dokumente met Aspose.Words bespaar tyd en maak dit maklik om vertaalfunksionaliteit in u projekte te integreer. Vir meer inligting, kyk na die [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API dokumentasie.

{{% /alert %}}