---
title: AI Sprawdzanie Gramatyki
second_title: Aspose.Words dla Java
articleTitle: Sprawdzanie Gramatyki
linktitle: Sprawdzanie Gramatyki
type: docs
weight: 40
description: "Sprawdź gramatykę dokumentu. Aspose.Words dla Java umożliwia użytkownikom sprawdzanie gramatyki i wykrywanie błędów w dokumentach za pomocą modeli OpenAI, Google i Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pl/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Sprawdzanie gramatyki w dokumentach jest ważne, aby zapewnić jasność, profesjonalizm i dokładność. Dobrze napisane dokumenty pozostawiają pozytywne wrażenie i unikają nieporozumień. Sprawdzanie gramatyki pomaga szybko identyfikować i poprawiać błędy, oszczędzając czas i poprawiając jakość.

Aspose.Words umożliwia użytkownikom sprawdzanie gramatyki i wykrywanie błędów w dokumentach przy użyciu rodzin modeli OpenAI, Google i Claude wymienionych w wyliczeniu [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). Użyj metody [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions), aby przeanalizować tekst w dokumencie i podkreślić problemy gramatyczne.

Poniższy przykład kodu pokazuje, jak używać modelu GPT-4o mini w Aspose.Words do sprawdzania gramatyki:

{{< highlight java >}}
 Document doc = new Document("Big document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI generative language models.
 IAiModelText model = (OpenAiModel)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
 grammarOptions.setImproveStylistics(true);

 Document proofedDoc = model.checkGrammar(doc, grammarOptions);
 proofedDoc.save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Sprawdzanie gramatyki za pomocą Aspose.Words poprawia jakość pracy i ułatwia integrację korekty z projektami. Aby uzyskać więcej informacji, sprawdź [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}