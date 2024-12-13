---
title: Bir Belgeyi Çevirin
second_title: .NET için Aspose.Words
articleTitle: Bir Belgeyi Çevirin
linktitle: Bir Belgeyi Çevirin
type: docs
weight: 30
description: "Bir belgeyi çevirin. .NET için Aspose.Words, Google AI modellerini kullanarak belge çevirisini basitleştirir ve hedef dili belirtmenize olanak tanır."
url: /tr/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Belge çevirisi, yüksek dijitalleşme çağında sıklıkla ihtiyaç duyulan bir seçenektir. Aspose.Words, geliştiricilerin metin içeriklerini 300'den fazla dile çevirmesine olanak tanıyan *Google* üretken dil modellerini kullanarak belge çevirisini destekler.

Belgelerinizi [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) numaralandırmasında gösterilen herhangi bir dile çevirmek için [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) yöntemini kullanın. Kaynak belgenin birden fazla dil içermesi durumunda, Google AI tabanlı modelin desteklenen tüm dilleri çevirebileceğini unutmayın. Model bazı metin parçalarındaki dili tanıyamazsa, bu çevrilmemiş parçaları ve metnin geri kalanını çevirmiş bir belge döndürülür.

Aşağıdaki kod örneği, bir belgeyi Arapçaya çevirmek için Aspose.Words'de *Gemini 1.5 Flash* modelinin nasıl kullanılacağını gösterir:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Words ile belgeleri çevirmek zamandan tasarruf sağlar ve çeviri işlevselliğini projelerinize entegre etmeyi kolaylaştırır. Daha fazla bilgi için [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API belgelerine bakın.

{{% /alert %}}