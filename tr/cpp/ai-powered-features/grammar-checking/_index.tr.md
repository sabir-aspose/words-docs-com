---
title: AI Dilbilgisi Denetimi
second_title: Aspose.Words için C++
articleTitle: Dilbilgisi Denetimi
linktitle: Dilbilgisi Denetimi
type: docs
weight: 40
description: "Bir belge dilbilgisini kontrol edin. Aspose.Words için C++ kullanıcıların OpenAI, Google ve Claude modellerini kullanarak dilbilgisini kontrol etmelerine ve belgelerdeki hataları tespit etmelerine olanak tanır."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /tr/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Belgelerdeki dilbilgisini kontrol etmek netlik, profesyonellik ve doğruluk sağlamak için önemlidir. İyi yazılmış belgeler olumlu bir izlenim bırakır ve yanlış anlaşılmalardan kaçınır. Dilbilgisi denetimleri, hataları hızlı bir şekilde tanımlamaya ve düzeltmeye yardımcı olarak zamandan tasarruf sağlar ve kaliteyi artırır.

Aspose.Words, kullanıcıların [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/) numaralandırmasında listelenen OpenAI, Google ve Claude modellerinin ailelerini kullanarak dilbilgisini kontrol etmelerine ve belgelerdeki hataları tespit etmelerine olanak tanır. [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) ad alanında bulunan [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/) yöntemini kullanın. **CheckGrammar** bir belgedeki metni analiz eder ve dilbilgisi sorunlarını vurgular.

Aşağıdaki kod örneği, dilbilgisini denetlemek için Aspose.Words içindeki GPT-4o mini modelinin nasıl kullanılacağını gösterir:

{{< highlight cpp >}}
void AiGrammar()
{
    auto doc = MakeObject<Document>(MyDir + u"Big document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto grammarOptions = MakeObject<CheckGrammarOptions>();
    grammarOptions->set_ImproveStylistics(true);

    auto proofedDoc = model->CheckGrammar(doc, grammarOptions);
    proofedDoc->Save(ArtifactsDir + u"AI.AiGrammar.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Dilbilgisini Aspose.Words ile kontrol etmek, çalışmanızın kalitesini artırır ve redaksiyonu projelerinize entegre etmeyi kolaylaştırır. Daha fazla bilgi için [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API belgelerine bakın.

{{% /alert %}}