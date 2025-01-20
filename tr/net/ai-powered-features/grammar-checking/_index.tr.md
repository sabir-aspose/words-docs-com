---
title: AI Dilbilgisi Denetimi
second_title: Aspose.Words için .NET
articleTitle: Dilbilgisi Denetimi
linktitle: Dilbilgisi Denetimi
type: docs
weight: 40
description: "Bir belge dilbilgisini kontrol edin. Aspose.Words için .NET kullanıcıların OpenAI modellerini kullanarak dilbilgisini kontrol etmelerine ve belgelerdeki hataları tespit etmelerine olanak tanır."
url: /tr/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

Belgelerdeki dilbilgisini kontrol etmek netlik, profesyonellik ve doğruluk sağlamak için önemlidir. İyi yazılmış belgeler olumlu bir izlenim bırakır ve yanlış anlaşılmalardan kaçınır. Dilbilgisi denetimleri, hataları hızlı bir şekilde tanımlamaya ve düzeltmeye yardımcı olarak zamandan tasarruf sağlar ve kaliteyi artırır.

Aspose.Words kullanıcıların **OpenAI** üretici modelleri kullanarak dilbilgisini kontrol etmelerine ve belgelerdeki hataları tespit etmelerine olanak tanır. [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) ad alanında bulunan [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/) yöntemini kullanın. **CheckGrammar** bir belgedeki metni analiz eder ve dilbilgisi sorunlarını vurgular.

Aşağıdaki kod örneği, dilbilgisini denetlemek için Aspose.Words içindeki GPT-4o mini modelinin nasıl kullanılacağını gösterir:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Big document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use OpenAI generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gpt4OMini).WithApiKey(apiKey);

CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
grammarOptions.ImproveStylistics = true;

Document proofedDoc = model.CheckGrammar(doc, grammarOptions);
proofedDoc.Save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Dilbilgisini Aspose.Words ile kontrol etmek, çalışmanızın kalitesini artırır ve redaksiyonu projelerinize entegre etmeyi kolaylaştırır. Daha fazla bilgi için [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API belgelerine bakın.

{{% /alert %}}