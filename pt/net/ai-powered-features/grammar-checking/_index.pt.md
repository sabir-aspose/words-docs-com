---
title: AI Verificação Gramatical
second_title: Aspose.Words Para .NET
articleTitle: Verificação Gramatical
linktitle: Verificação Gramatical
type: docs
weight: 40
description: "Verifique a gramática de um documento. Aspose.Words para .NET permite aos utilizadores verificar a gramática e detetar erros em documentos utilizando modelos OpenAI."
url: /pt/net/grammar checking/
timestamp: 2025-01-15-16-40-05
---

A verificação gramatical em documentos é importante para garantir clareza, profissionalismo e precisão. Documentos bem escritos deixam uma impressão positiva e evitam mal-entendidos. As verificações gramaticais ajudam a identificar e corrigir erros rapidamente, poupando tempo e melhorando a qualidade.

Aspose.Words permite aos utilizadores verificar a gramática e detetar erros em documentos utilizando **OpenAI** modelos generativos. Use o método [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/), disponível no namespace [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/). **CheckGrammar** analisa o texto em um documento e destaca problemas gramaticais.

O exemplo de código a seguir mostra como usar o modelo GPT-4o mini em Aspose.Words para verificar a gramática:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Big document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use OpenAI generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gpt4OMini).WithApiKey(apiKey);

CheckGrammarOptions grammarOptions = new CheckGrammarOptions();
grammarOptions.ImproveStylistics = true;

Document proofedDoc = model.CheckGrammar(doc, grammarOptions);
proofedDoc.Save("AI.AiGrammar.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Verificar a gramática com Aspose.Words melhora a qualidade do seu trabalho e facilita a integração da revisão nos seus projetos. Para obter mais informações, consulte a documentação [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}