---
title: Przetłumacz dokument
second_title: Aspose.Words dla C++
articleTitle: Przetłumacz dokument
linktitle: Przetłumacz dokument
type: docs
weight: 30
description: "Przetłumacz dokument. Aspose.Words dla C++ upraszcza tłumaczenie dokumentów za pomocą modeli Google AI, umożliwiając określenie języka docelowego."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pl/cpp/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Tłumaczenie dokumentów jest często potrzebną opcją w dobie wysokiej cyfryzacji. Aspose.Words obsługuje tłumaczenie dokumentów przy użyciu *Google* generatywnych modeli językowych, co pozwala programistom tłumaczyć treści tekstów na ponad 300 języków.

Użyj metody [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/), aby przetłumaczyć dokumenty na dowolny język reprezentowany w wyliczeniu [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/). Pamiętaj, że jeśli dokument źródłowy zawiera kilka języków, model oparty na Google AI będzie mógł przetłumaczyć wszystkie obsługiwane języki. Jeśli model nie może rozpoznać języka w niektórych fragmentach tekstu, zostanie zwrócony dokument z tymi nieprzetłumaczonymi fragmentami i przetłumaczoną resztą tekstu.

Poniższy przykład kodu pokazuje, jak użyć modelu *Gemini 1.5 Flash* w Aspose.Words do przetłumaczenia dokumentu na język arabski:

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

Tłumaczenie dokumentów za pomocą Aspose.Words oszczędza czas i ułatwia integrację funkcji tłumaczenia z projektami. Aby uzyskać więcej informacji, sprawdź dokumentację [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}