---
title: Przetłumacz dokument
second_title: Aspose.Words dla Java
articleTitle: Przetłumacz dokument
linktitle: Przetłumacz dokument
type: docs
weight: 30
description: "Przetłumacz dokument. Aspose.Words dla Java upraszcza tłumaczenie dokumentów za pomocą modeli Google AI, umożliwiając określenie języka docelowego."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pl/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Tłumaczenie dokumentów jest często potrzebną opcją w dobie wysokiej cyfryzacji. Aspose.Words obsługuje tłumaczenie dokumentów przy użyciu *Google* generatywnych modeli językowych, co pozwala programistom tłumaczyć treści tekstów na ponad 300 języków.

Użyj metody [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int), aby przetłumaczyć dokumenty na dowolny język reprezentowany w wyliczeniu [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). Pamiętaj, że jeśli dokument źródłowy zawiera kilka języków, model oparty na Google AI będzie mógł przetłumaczyć wszystkie obsługiwane języki. Jeśli model nie może rozpoznać języka w niektórych fragmentach tekstu, zostanie zwrócony dokument z tymi nieprzetłumaczonymi fragmentami i przetłumaczoną resztą tekstu.

Poniższy przykład kodu pokazuje, jak użyć modelu *Gemini 1.5 Flash* w Aspose.Words do przetłumaczenia dokumentu na język arabski:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Tłumaczenie dokumentów za pomocą Aspose.Words oszczędza czas i ułatwia integrację funkcji tłumaczenia z projektami. Aby uzyskać więcej informacji, sprawdź [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}