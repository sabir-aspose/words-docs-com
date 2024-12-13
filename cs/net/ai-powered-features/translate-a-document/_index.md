---
title: Přeložit dokument
second_title: Aspose.Words pro .NET
articleTitle: Přeložte dokument
linktitle: Přeložit dokument
type: docs
weight: 30
description: "Přeložte dokument. Aspose.Words for .NET zjednodušuje překlad dokumentů pomocí modelů umělé inteligence Google a umožňuje vám určit cílový jazyk."
url: /cs/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Překlad dokumentů je v době vysoké digitalizace často potřebnou možností. Aspose.Words podporuje překlad dokumentů pomocí generativních jazykových modelů *Google*, což umožňuje vývojářům překládat obsah textů do více než 300 jazyků.

Pomocí metody [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) přeložte své dokumenty do jakéhokoli jazyka uvedeného v [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Upozorňujeme, že pokud zdrojový dokument obsahuje několik jazyků, model založený na umělé inteligenci Google bude schopen přeložit všechny podporované jazyky. Pokud model nedokáže rozpoznat jazyk v některých textových fragmentech, pak vám bude vrácen dokument s těmito nepřeloženými fragmenty a s přeloženým zbytkem textu.

Následující příklad kódu ukazuje, jak použít model *Gemini 1.5 Flash* v Aspose.Words k překladu dokumentu do arabštiny:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Překládání dokumentů pomocí Aspose.Words šetří čas a usnadňuje integraci funkcí překladu do vašich projektů. Další informace naleznete v dokumentaci rozhraní API [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

{{% /alert %}}