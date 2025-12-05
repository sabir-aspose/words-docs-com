---
title: AI Controllo grammaticale
second_title: Aspose.Wordsper C++
articleTitle: Controllo grammaticale
linktitle: Controllo grammaticale
type: docs
weight: 40
description: "Controllare la grammatica di un documento. Aspose.Wordsper C++ consente agli utenti di controllare la grammatica e rilevare errori nei documenti utilizzando i modelli OpenAI, Google e Claude."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /it/cpp/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

Controllare la grammatica nei documenti è importante per garantire chiarezza, professionalità e accuratezza. I documenti ben scritti lasciano un'impressione positiva ed evitano malintesi. I controlli grammaticali aiutano a identificare e correggere rapidamente gli errori, risparmiando tempo e migliorando la qualità.

Aspose.Words consente agli utenti di controllare la grammatica e rilevare errori nei documenti utilizzando le famiglie dei modelli OpenAI, Google e Claude elencate nell'enumerazione [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). Utilizzare il metodo [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/), disponibile nello spazio dei nomi [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/). **CheckGrammar** analizza il testo di un documento ed evidenzia i problemi grammaticali.

Il seguente esempio di codice mostra come utilizzare il modello GPT-4o mini in Aspose.Words per controllare la grammatica:

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

Il controllo della grammatica con Aspose.Words migliora la qualità del tuo lavoro e semplifica l'integrazione della correzione di bozze nei tuoi progetti. Per ulteriori informazioni, controllare la documentazione [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API.

{{% /alert %}}