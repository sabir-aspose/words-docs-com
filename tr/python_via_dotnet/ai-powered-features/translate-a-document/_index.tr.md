---
title: Bir Belgeyi Çevirme
second_title: Aspose.Words için Python via .NET
articleTitle: Bir Belgeyi Çevirme
linktitle: Bir Belgeyi Çevirme
type: docs
weight: 30
description: "Bir belgeyi çevirin. Aspose.Words için Python Google AI modellerini kullanarak belge çevirisini basitleştirerek hedef dili belirlemenizi sağlar."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /tr/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Belge çevirisi, yüksek dijitalleşme çağında sıkça ihtiyaç duyulan bir seçenektir. Aspose.Words, geliştiricilerin metin içeriğini 300'den fazla dile çevirmesine olanak tanıyan *Google* üretken dil modellerini kullanarak belge çevirisini destekler.

Belgelerinizi [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) numaralandırmasında temsil edilen herhangi bir dile çevirmek için [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) yöntemini kullanın. Kaynak belge birkaç dil içeriyorsa, Google AI tabanlı modelin desteklenen tüm dilleri çevirebileceğini unutmayın. Model, bazı metin parçalarındaki dili tanıyamazsa, bu çevrilmemiş parçaları ve çevrilmiş metnin geri kalanını içeren bir belge size iade edilir.

Aşağıdaki kod örneği, bir belgeyi Arapça'ya çevirmek için Aspose.Words içindeki *Gemini 1.5 Flash* modelinin nasıl kullanılacağını gösterir:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Belgeleri Aspose.Words ile çevirmek zaman kazandırır ve çeviri işlevselliğini projelerinize entegre etmeyi kolaylaştırır. Daha fazla bilgi için [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API belgelerine bakın.

{{% /alert %}}