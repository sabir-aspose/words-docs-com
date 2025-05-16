---
title: Přeložit dokument
second_title: Aspose.Words pro Python via .NET
articleTitle: Přeložit dokument
linktitle: Přeložit dokument
type: docs
weight: 30
description: "Přeložit dokument. Aspose.Words pro Python zjednodušuje překlad dokumentů pomocí modelů Google AI, což vám umožňuje určit cílový jazyk."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Překlad dokumentů je v době vysoké digitalizace často potřebnou možností. Aspose.Words podporuje překlad dokumentů pomocí *Google* generativních jazykových modelů, což vývojářům umožňuje překládat obsah textů do více než 300 jazyků.

Pomocí metody [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) přeložte své dokumenty do libovolného jazyka zastoupeného ve výčtu [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). Všimněte si, že pokud zdrojový dokument obsahuje několik jazyků, bude model založený na Google AI schopen přeložit všechny podporované jazyky. Pokud model nedokáže rozpoznat jazyk v některých fragmentech textu, bude vám vrácen dokument s těmito nepřekládanými fragmenty a se zbytkem přeloženého textu.

Následující příklad kódu ukazuje, jak použít model *Gemini 1.5 Flash* v Aspose.Words k překladu dokumentu do arabštiny:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Překlad dokumentů pomocí Aspose.Words šetří čas a usnadňuje integraci překladových funkcí do vašich projektů. Další informace najdete v dokumentaci [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}