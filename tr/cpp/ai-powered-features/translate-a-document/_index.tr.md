---
title: Bir Belgeyi Çevirme
second_title: Aspose.Words için C++
articleTitle: Bir Belgeyi Çevirme
linktitle: Bir Belgeyi Çevirme
type: docs
weight: 30
description: "Bir belgeyi çevirin. Aspose.Words için C++ Google AI modellerini kullanarak belge çevirisini basitleştirerek hedef dili belirlemenizi sağlar."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Belge çevirisi, yüksek dijitalleşme çağında sıkça ihtiyaç duyulan bir seçenektir. Aspose.Words, geliştiricilerin metin içeriğini 300'den fazla dile çevirmesine olanak tanıyan *Google* üretken dil modellerini kullanarak belge çevirisini destekler.

Belgelerinizi [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) numaralandırmasında temsil edilen herhangi bir dile çevirmek için [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) yöntemini kullanın. Kaynak belge birkaç dil içeriyorsa, Google AI tabanlı modelin desteklenen tüm dilleri çevirebileceğini unutmayın. Model, bazı metin parçalarındaki dili tanıyamazsa, bu çevrilmemiş parçaları ve çevrilmiş metnin geri kalanını içeren bir belge size iade edilir.

Aşağıdaki kod örneği, bir belgeyi Arapça'ya çevirmek için Aspose.Words içindeki *Gemini 1.5 Flash* modelinin nasıl kullanılacağını gösterir:

{{< highlight cpp >}}
void AiTranslate()
{
    auto doc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<GoogleAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"));

    auto translatedDoc = model->Translate(doc, Language::Arabic);
    translatedDoc->Save(ArtifactsDir + u"AI.AiTranslate.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

Belgeleri Aspose.Words ile çevirmek zaman kazandırır ve çeviri işlevselliğini projelerinize entegre etmeyi kolaylaştırır. Daha fazla bilgi için [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API belgelerine bakın.

{{% /alert %}}