---
title: Bir Belgeyi Çevirme
second_title: Aspose.Words için .NET
articleTitle: Bir Belgeyi Çevirme
linktitle: Bir Belgeyi Çevirme
type: docs
weight: 30
description: "Bir belgeyi çevirin. Aspose.Words için .NET Google AI modellerini kullanarak belge çevirisini basitleştirerek hedef dili belirlemenizi sağlar."
url: /tr/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Belge çevirisi, yüksek dijitalleşme çağında sıkça ihtiyaç duyulan bir seçenektir. Aspose.Words, geliştiricilerin metin içeriğini 300'den fazla dile çevirmesine olanak tanıyan *Google* üretken dil modellerini kullanarak belge çevirisini destekler.

Belgelerinizi [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) numaralandırmasında temsil edilen herhangi bir dile çevirmek için [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) yöntemini kullanın. Kaynak belge birkaç dil içeriyorsa, Google AI tabanlı modelin desteklenen tüm dilleri çevirebileceğini unutmayın. Model, bazı metin parçalarındaki dili tanıyamazsa, bu çevrilmemiş parçaları ve çevrilmiş metnin geri kalanını içeren bir belge size iade edilir.

Aşağıdaki kod örneği, bir belgeyi Arapça'ya çevirmek için Aspose.Words içindeki *Gemini 1.5 Flash* modelinin nasıl kullanılacağını gösterir:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Belgeleri Aspose.Words ile çevirmek zaman kazandırır ve çeviri işlevselliğini projelerinize entegre etmeyi kolaylaştırır. Daha fazla bilgi için [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API belgelerine bakın.

{{% /alert %}}