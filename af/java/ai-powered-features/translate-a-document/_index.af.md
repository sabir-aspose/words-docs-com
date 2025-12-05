---
title: Vertaal'n Dokument
second_title: Aspose.Words vir Java
articleTitle: Vertaal'n Dokument
linktitle: Vertaal'n Dokument
type: docs
weight: 30
description: "Vertaal'n dokument. Aspose.Words vir Java vereenvoudig dokumentvertaling met Behulp Van Google AI modelle, sodat jy die teikentaal kan spesifiseer."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /af/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Dokumentvertaling is'n dikwels benodigde opsie in die era van hoë digitalisering. Aspose.Words ondersteun dokumentvertaling met behulp van *Google* generatiewe taalmodelle, wat ontwikkelaars toelaat om teksinhoud in meer as 300 tale te vertaal.

Gebruik die [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) metode om jou dokumente te vertaal in enige taal wat in die [Language](https://reference.aspose.com/words/java/com.aspose.words/language/) opsomming verteenwoordig word. Let daarop dat as die brondokument verskeie tale bevat, Die Google AI-gebaseerde model alle ondersteunde tale kan vertaal. As die model nie die taal in sommige teksfragmente kan herken nie, sal u'n dokument met hierdie ongetranslateerde fragmente en met die res van die teks vertaal word.

Die volgende kode voorbeeld toon hoe om die *Gemini 1.5 Flash* model in Aspose.Words te gebruik om'n dokument in arabies te vertaal:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Die vertaling van dokumente met Aspose.Words bespaar tyd en maak dit maklik om vertaalfunksionaliteit in u projekte te integreer. Vir meer inligting, kyk na die [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}