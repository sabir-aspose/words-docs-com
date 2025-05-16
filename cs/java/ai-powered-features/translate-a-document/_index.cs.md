---
title: Přeložit dokument
second_title: Aspose.Words pro Java
articleTitle: Přeložit dokument
linktitle: Přeložit dokument
type: docs
weight: 30
description: "Přeložit dokument. Aspose.Words pro Java zjednodušuje překlad dokumentů pomocí modelů Google AI, což vám umožňuje určit cílový jazyk."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Překlad dokumentů je v době vysoké digitalizace často potřebnou možností. Aspose.Words podporuje překlad dokumentů pomocí *Google* generativních jazykových modelů, což vývojářům umožňuje překládat obsah textů do více než 300 jazyků.

Pomocí metody [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) přeložte své dokumenty do libovolného jazyka zastoupeného ve výčtu [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). Všimněte si, že pokud zdrojový dokument obsahuje několik jazyků, bude model založený na Google AI schopen přeložit všechny podporované jazyky. Pokud model nedokáže rozpoznat jazyk v některých fragmentech textu, bude vám vrácen dokument s těmito nepřekládanými fragmenty a se zbytkem přeloženého textu.

Následující příklad kódu ukazuje, jak použít model *Gemini 1.5 Flash* v Aspose.Words k překladu dokumentu do arabštiny:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Překlad dokumentů pomocí Aspose.Words šetří čas a usnadňuje integraci překladových funkcí do vašich projektů. Pro více informací zkontrolujte [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}