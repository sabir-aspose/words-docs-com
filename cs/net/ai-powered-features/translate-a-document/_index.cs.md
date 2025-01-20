---
title: Přeložit dokument
second_title: Aspose.Words pro .NET
articleTitle: Přeložit dokument
linktitle: Přeložit dokument
type: docs
weight: 30
description: "Přeložit dokument. Aspose.Words pro .NET zjednodušuje překlad dokumentů pomocí modelů Google AI, což vám umožňuje určit cílový jazyk."
url: /cs/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Překlad dokumentů je v době vysoké digitalizace často potřebnou možností. Aspose.Words podporuje překlad dokumentů pomocí *Google* generativních jazykových modelů, což vývojářům umožňuje překládat obsah textů do více než 300 jazyků.

Pomocí metody [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) přeložte své dokumenty do libovolného jazyka zastoupeného ve výčtu [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Všimněte si, že pokud zdrojový dokument obsahuje několik jazyků, bude model založený na Google AI schopen přeložit všechny podporované jazyky. Pokud model nedokáže rozpoznat jazyk v některých fragmentech textu, bude vám vrácen dokument s těmito nepřekládanými fragmenty a se zbytkem přeloženého textu.

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

Překlad dokumentů pomocí Aspose.Words šetří čas a usnadňuje integraci překladových funkcí do vašich projektů. Další informace najdete v dokumentaci [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}