---
title: Vertaal 'n dokument
second_title: Aspose.Words vir .NET
articleTitle: Vertaal 'n dokument
linktitle: Vertaal 'n dokument
tipe: doks
weight: 30
description: "Vertaal 'n dokument. Aspose.Words for .NET vereenvoudig dokumentvertaling deur gebruik te maak van Google KI-modelle, wat jou toelaat om die teikentaal te spesifiseer."
url: /af/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Dokumentvertaling is 'n gereelde vereiste opsie in die era van hoë digitalisering. Aspose.Words ondersteun dokumentvertaling deur gebruik te maak van *Google* generatiewe taalmodelle, wat ontwikkelaars in staat stel om tekste-inhoud in meer as 300 tale te vertaal.

Gebruik die [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) metode om jou dokumente te vertaal in enige taal wat in die [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) opsomming. Let daarop dat as die brondokument verskeie tale bevat, die Google KI-gebaseerde model alle ondersteunde tale sal kan vertaal. As die model nie die taal in sommige teksfragmente kan herken nie, sal jy 'n dokument met hierdie onvertaalde fragmente teruggestuur word en met die res van die teks vertaal.

Die volgende kodevoorbeeld wys hoe om die *Gemini 1.5 Flash*-model in Aspose.Words te gebruik om 'n dokument in Arabies te vertaal:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Die vertaling van dokumente met Aspose.Words spaar tyd en maak dit maklik om vertaalfunksionaliteit in jou projekte te integreer. Vir meer inligting, gaan na die [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API dokumentasie.

{{% /alert %}}