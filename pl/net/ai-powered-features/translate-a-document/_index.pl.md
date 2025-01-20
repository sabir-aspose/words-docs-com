---
title: Przetłumacz dokument
second_title: Aspose.Words dla .NET
articleTitle: Przetłumacz dokument
linktitle: Przetłumacz dokument
type: docs
weight: 30
description: "Przetłumacz dokument. Aspose.Words dla .NET upraszcza tłumaczenie dokumentów za pomocą modeli Google AI, umożliwiając określenie języka docelowego."
url: /pl/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Tłumaczenie dokumentów jest często potrzebną opcją w dobie wysokiej cyfryzacji. Aspose.Words obsługuje tłumaczenie dokumentów przy użyciu *Google* generatywnych modeli językowych, co pozwala programistom tłumaczyć treści tekstów na ponad 300 języków.

Użyj metody [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/), aby przetłumaczyć dokumenty na dowolny język reprezentowany w wyliczeniu [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Pamiętaj, że jeśli dokument źródłowy zawiera kilka języków, model oparty na Google AI będzie mógł przetłumaczyć wszystkie obsługiwane języki. Jeśli model nie może rozpoznać języka w niektórych fragmentach tekstu, zostanie zwrócony dokument z tymi nieprzetłumaczonymi fragmentami i przetłumaczoną resztą tekstu.

Poniższy przykład kodu pokazuje, jak użyć modelu *Gemini 1.5 Flash* w Aspose.Words do przetłumaczenia dokumentu na język arabski:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Tłumaczenie dokumentów za pomocą Aspose.Words oszczędza czas i ułatwia integrację funkcji tłumaczenia z projektami. Aby uzyskać więcej informacji, sprawdź dokumentację [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}