---
title: AI Dilbilgisi Denetimi
second_title: Aspose.Words için Java
articleTitle: Dilbilgisi Denetimi
linktitle: Dilbilgisi Denetimi
type: docs
weight: 40
description: "Bir belge dilbilgisini kontrol edin. Aspose.Words için Java kullanıcıların OpenAI, Google ve Claude modellerini kullanarak dilbilgisini kontrol etmelerine ve belgelerdeki hataları tespit etmelerine olanak tanır."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Belgelerdeki dilbilgisini kontrol etmek netlik, profesyonellik ve doğruluk sağlamak için önemlidir. İyi yazılmış belgeler olumlu bir izlenim bırakır ve yanlış anlaşılmalardan kaçınır. Dilbilgisi denetimleri, hataları hızlı bir şekilde tanımlamaya ve düzeltmeye yardımcı olarak zamandan tasarruf sağlar ve kaliteyi artırır.

Aspose.Words, kullanıcıların [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/) numaralandırmasında listelenen OpenAI, Google ve Claude modellerinin ailelerini kullanarak dilbilgisini kontrol etmelerine ve belgelerdeki hataları tespit etmelerine olanak tanır. Bir belgedeki metni çözümlemek için [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) yöntemini kullanın ve dilbilgisi sorunlarını vurgulayın.

Aşağıdaki kod örneği, dilbilgisini denetlemek için Aspose.Words içindeki GPT-4o mini modelinin nasıl kullanılacağını gösterir:

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

Dilbilgisini Aspose.Words ile kontrol etmek, çalışmanızın kalitesini artırır ve redaksiyonu projelerinize entegre etmeyi kolaylaştırır. Daha fazla bilgi için [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/)'ı kontrol edin.

{{% /alert %}}