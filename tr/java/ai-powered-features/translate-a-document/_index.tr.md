---
title: Bir Belgeyi Çevirme
second_title: Aspose.Words için Java
articleTitle: Bir Belgeyi Çevirme
linktitle: Bir Belgeyi Çevirme
type: docs
weight: 30
description: "Bir belgeyi çevirin. Aspose.Words için Java Google AI modellerini kullanarak belge çevirisini basitleştirerek hedef dili belirlemenizi sağlar."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /tr/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Belge çevirisi, yüksek dijitalleşme çağında sıkça ihtiyaç duyulan bir seçenektir. Aspose.Words, geliştiricilerin metin içeriğini 300'den fazla dile çevirmesine olanak tanıyan *Google* üretken dil modellerini kullanarak belge çevirisini destekler.

Belgelerinizi [Language](https://reference.aspose.com/words/java/com.aspose.words/language/) numaralandırmasında temsil edilen herhangi bir dile çevirmek için [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) yöntemini kullanın. Kaynak belge birkaç dil içeriyorsa, Google AI tabanlı modelin desteklenen tüm dilleri çevirebileceğini unutmayın. Model, bazı metin parçalarındaki dili tanıyamazsa, bu çevrilmemiş parçaları ve çevrilmiş metnin geri kalanını içeren bir belge size iade edilir.

Aşağıdaki kod örneği, bir belgeyi Arapça'ya çevirmek için Aspose.Words içindeki *Gemini 1.5 Flash* modelinin nasıl kullanılacağını gösterir:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Belgeleri Aspose.Words ile çevirmek zaman kazandırır ve çeviri işlevselliğini projelerinize entegre etmeyi kolaylaştırır. Daha fazla bilgi için [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/)'ı kontrol edin.

{{% /alert %}}