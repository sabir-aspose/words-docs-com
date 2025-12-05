---
title: AI Verificação Gramatical
second_title: Aspose.Words Para Java
articleTitle: Verificação Gramatical
linktitle: Verificação Gramatical
type: docs
weight: 40
description: "Verifique a gramática de um documento. Aspose.Words Para Java permite aos utilizadores verificar a gramática e detetar erros em documentos utilizando os modelos OpenAI, Google e Claude."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pt/java/grammar-checking/
timestamp: 2025-03-17-19-00-00
---

A verificação gramatical em documentos é importante para garantir clareza, profissionalismo e precisão. Documentos bem escritos deixam uma impressão positiva e evitam mal-entendidos. As verificações gramaticais ajudam a identificar e corrigir erros rapidamente, poupando tempo e melhorando a qualidade.

Aspose.Words permite aos utilizadores verificar a gramática e detetar erros em documentos utilizando as famílias dos modelos OpenAI, Google e Claude enumeradas na enumeração [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). Use o método [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) para analisar o texto em um documento e destacar problemas gramaticais.

O exemplo de código a seguir mostra como usar o modelo GPT-4o mini em Aspose.Words para verificar a gramática:

{{< highlight java >}}
 Document doc = new Document("Big document.docx");

 String apiKey = System.getenv("API_KEY");
 // Use OpenAI generative language models.
 IAiModelText model = (OpenAiModel)AiModel.create(AiModelType.GPT_4_O_MINI).withApiKey(apiKey);

 CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
 grammarOptions.setImproveStylistics(true);

 Document proofedDoc = model.checkGrammar(doc, grammarOptions);
 proofedDoc.save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Verificar a gramática com Aspose.Words melhora a qualidade do seu trabalho e facilita a integração da revisão nos seus projetos. Para mais informações, verifique o [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}