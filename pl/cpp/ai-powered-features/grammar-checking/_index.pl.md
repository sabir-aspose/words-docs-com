---
title: AI Sprawdzanie Gramatyki
second_title: Aspose.Words dla C++
articleTitle: Sprawdzanie Gramatyki
linktitle: Sprawdzanie Gramatyki
type: docs
weight: 40
description: "Sprawdź gramatykę dokumentu. Aspose.Words dla C++ umożliwia użytkownikom sprawdzanie gramatyki i wykrywanie błędów w dokumentach za pomocą modeli OpenAI, Google i Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pl/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Sprawdzanie gramatyki w dokumentach jest ważne, aby zapewnić jasność, profesjonalizm i dokładność. Dobrze napisane dokumenty pozostawiają pozytywne wrażenie i unikają nieporozumień. Sprawdzanie gramatyki pomaga szybko identyfikować i poprawiać błędy, oszczędzając czas i poprawiając jakość.

Aspose.Words umożliwia użytkownikom sprawdzanie gramatyki i wykrywanie błędów w dokumentach przy użyciu rodzin modeli OpenAI, Google i Claude wymienionych w wyliczeniu [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). Użyj metody [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), dostępnej w przestrzeni nazw [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** analizuje tekst w dokumencie i podkreśla problemy gramatyczne.

Poniższy przykład kodu pokazuje, jak używać modelu GPT-4o mini w Aspose.Words do sprawdzania gramatyki:

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

Sprawdzanie gramatyki za pomocą Aspose.Words poprawia jakość pracy i ułatwia integrację korekty z projektami. Aby uzyskać więcej informacji, sprawdź dokumentację [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}