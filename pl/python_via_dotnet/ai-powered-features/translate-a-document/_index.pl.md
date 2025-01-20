---
title: Przetłumacz dokument
second_title: Aspose.Words dla Python via .NET
articleTitle: Przetłumacz dokument
linktitle: Przetłumacz dokument
type: docs
weight: 30
description: "Przetłumacz dokument. Aspose.Words dla Python upraszcza tłumaczenie dokumentów za pomocą modeli Google AI, umożliwiając określenie języka docelowego."
url: /pl/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Tłumaczenie dokumentów jest często potrzebną opcją w dobie wysokiej cyfryzacji. Aspose.Words obsługuje tłumaczenie dokumentów przy użyciu *Google* generatywnych modeli językowych, co pozwala programistom tłumaczyć treści tekstów na ponad 300 języków.

Użyj metody [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language), aby przetłumaczyć dokumenty na dowolny język reprezentowany w wyliczeniu [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). Pamiętaj, że jeśli dokument źródłowy zawiera kilka języków, model oparty na Google AI będzie mógł przetłumaczyć wszystkie obsługiwane języki. Jeśli model nie może rozpoznać języka w niektórych fragmentach tekstu, zostanie zwrócony dokument z tymi nieprzetłumaczonymi fragmentami i przetłumaczoną resztą tekstu.

Poniższy przykład kodu pokazuje, jak użyć modelu *Gemini 1.5 Flash* w Aspose.Words do przetłumaczenia dokumentu na język arabski:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Tłumaczenie dokumentów za pomocą Aspose.Words oszczędza czas i ułatwia integrację funkcji tłumaczenia z projektami. Aby uzyskać więcej informacji, sprawdź dokumentację [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}