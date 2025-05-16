---
title: AI Verificarea Gramaticii
second_title: Aspose.Words pentru Java
articleTitle: Verificarea Gramaticii
linktitle: Verificarea Gramaticii
type: docs
weight: 40
description: "Verificați gramatica unui document. Aspose.Words Pentru Java permite utilizatorilor să verifice gramatica și să detecteze erorile din documente folosind modelele OpenAI, Google și Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ro/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Verificarea gramaticii în documente este importantă pentru a asigura claritate, profesionalism și acuratețe. Documentele bine scrise lasă o impresie pozitivă și evită neînțelegerile. Verificările gramaticale ajută la identificarea și corectarea rapidă a erorilor, economisind timp și îmbunătățind calitatea.

Aspose.Words permite utilizatorilor să verifice gramatica și să detecteze erorile din documente folosind familiile modelelor OpenAI, Google și Claude enumerate în enumerarea [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). Utilizați metoda [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) pentru a analiza textul dintr-un document și pentru a evidenția problemele gramaticale.

Următorul exemplu de cod arată cum să utilizați modelul GPT-4o mini în Aspose.Words pentru a verifica gramatica:

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

Verificarea gramaticii cu Aspose.Words îmbunătățește calitatea muncii dvs. și facilitează integrarea corecturii în proiectele dvs. Pentru mai multe informații, verificați [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}