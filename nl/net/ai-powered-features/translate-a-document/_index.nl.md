---
title: Een Document vertalen
second_title: Aspose.Words voor .NET
articleTitle: Een Document vertalen
linktitle: Een Document vertalen
type: docs
weight: 30
description: "Vertaal een document. Aspose.Words voor .NET vereenvoudigt documentvertaling met behulp van Google AI - modellen, zodat u de doeltaal kunt opgeven."
url: /nl/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Documentvertaling is een veelgebruikte optie in het tijdperk van hoge digitalisering. Aspose.Words ondersteunt documentvertaling met behulp van *Google* generatieve taalmodellen, waarmee ontwikkelaars teksten in meer dan 300 talen kunnen vertalen.

Gebruik de methode [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) om uw documenten te vertalen naar elke taal die wordt weergegeven in de [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) - opsomming. Merk op dat als het brondocument meerdere talen bevat, het op Google AI gebaseerde model alle ondersteunde talen kan vertalen. Als het model de taal in sommige tekstfragmenten niet kan herkennen, krijgt u een document terug met deze niet-vertaalde fragmenten en met de rest van de tekst vertaald.

Het volgende codevoorbeeld laat zien hoe u het *Gemini 1.5 Flash* - model in Aspose.Words gebruikt om een document naar het Arabisch te vertalen:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Het vertalen van documenten met Aspose.Words bespaart tijd en maakt het eenvoudig om vertaalfunctionaliteit in uw projecten te integreren. Raadpleeg de [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API documentatie voor meer informatie.

{{% /alert %}}