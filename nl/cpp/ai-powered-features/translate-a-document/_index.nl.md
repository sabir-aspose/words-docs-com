---
title: Een Document vertalen
second_title: Aspose.Words voor C++
articleTitle: Een Document vertalen
linktitle: Een Document vertalen
type: docs
weight: 30
description: "Vertaal een document. Aspose.Words voor C++ vereenvoudigt documentvertaling met behulp van Google AI - modellen, zodat u de doeltaal kunt opgeven."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nl/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Documentvertaling is een veelgebruikte optie in het tijdperk van hoge digitalisering. Aspose.Words ondersteunt documentvertaling met behulp van *Google* generatieve taalmodellen, waarmee ontwikkelaars teksten in meer dan 300 talen kunnen vertalen.

Gebruik de methode [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) om uw documenten te vertalen naar elke taal die wordt weergegeven in de [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) - opsomming. Merk op dat als het brondocument meerdere talen bevat, het op Google AI gebaseerde model alle ondersteunde talen kan vertalen. Als het model de taal in sommige tekstfragmenten niet kan herkennen, krijgt u een document terug met deze niet-vertaalde fragmenten en met de rest van de tekst vertaald.

Het volgende codevoorbeeld laat zien hoe u het *Gemini 1.5 Flash* - model in Aspose.Words gebruikt om een document naar het Arabisch te vertalen:

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

Het vertalen van documenten met Aspose.Words bespaart tijd en maakt het eenvoudig om vertaalfunctionaliteit in uw projecten te integreren. Raadpleeg de [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API documentatie voor meer informatie.

{{% /alert %}}