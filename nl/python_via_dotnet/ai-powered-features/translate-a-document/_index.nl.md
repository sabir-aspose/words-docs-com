---
title: Een Document vertalen
second_title: Aspose.Words voor Python via .NET
articleTitle: Een Document vertalen
linktitle: Een Document vertalen
type: docs
weight: 30
description: "Vertaal een document. Aspose.Words voor Python vereenvoudigt documentvertaling met behulp van Google AI - modellen, zodat u de doeltaal kunt opgeven."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nl/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Documentvertaling is een veelgebruikte optie in het tijdperk van hoge digitalisering. Aspose.Words ondersteunt documentvertaling met behulp van *Google* generatieve taalmodellen, waarmee ontwikkelaars teksten in meer dan 300 talen kunnen vertalen.

Gebruik de methode [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) om uw documenten te vertalen naar elke taal die wordt weergegeven in de [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) - opsomming. Merk op dat als het brondocument meerdere talen bevat, het op Google AI gebaseerde model alle ondersteunde talen kan vertalen. Als het model de taal in sommige tekstfragmenten niet kan herkennen, krijgt u een document terug met deze niet-vertaalde fragmenten en met de rest van de tekst vertaald.

Het volgende codevoorbeeld laat zien hoe u het *Gemini 1.5 Flash* - model in Aspose.Words gebruikt om een document naar het Arabisch te vertalen:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Het vertalen van documenten met Aspose.Words bespaart tijd en maakt het eenvoudig om vertaalfunctionaliteit in uw projecten te integreren. Raadpleeg de [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API documentatie voor meer informatie.

{{% /alert %}}