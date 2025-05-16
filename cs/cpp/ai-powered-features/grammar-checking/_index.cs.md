---
title: AI Kontrola Gramatiky
second_title: Aspose.Words pro C++
articleTitle: Gramatik
linktitle: Gramatik
type: docs
weight: 40
description: "Zkontrolujte gramatiku dokumentu. Aspose.Words pro C++ umožňuje uživatelům kontrolovat gramatiku a detekovat chyby v dokumentech pomocí modelů OpenAI, Google a Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Kontrola gramatiky v dokumentech je důležitá pro zajištění jasnosti, profesionality a přesnosti. Dobře napsané dokumenty zanechávají pozitivní dojem a vyhýbají se nedorozuměním. Gramatické kontroly pomáhají rychle identifikovat a opravit chyby, šetří čas a zlepšují kvalitu.

Aspose.Words umožňuje uživatelům kontrolovat gramatiku a detekovat chyby v dokumentech pomocí rodin modelů OpenAI, Google a Claude uvedených ve výčtu [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). Použijte metodu [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), která je k dispozici v oboru názvů [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** analyzuje text v dokumentu a zdůrazňuje gramatické problémy.

Následující příklad kódu ukazuje, jak použít model GPT-4o mini v Aspose.Words ke kontrole gramatiky:

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

Kontrola gramatiky pomocí Aspose.Words zlepšuje kvalitu vaší práce a usnadňuje integraci korektur do vašich projektů. Další informace najdete v dokumentaci [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}