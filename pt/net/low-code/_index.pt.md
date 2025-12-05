---
title: Low Code
second_title: Aspose.Words Para .NET
articleTitle: Trabalhar com documentos utilizando LowCode API
linktitle: Low Code
type: docs
description: "Simplifique tarefas de processamento de documentos como comparar, converter, dividir, mesclar, localizar e substituir e outras usando Low Code API. Aspose.Words LowCode API com sintaxe limpa, resultados rápidos e esforço mínimo de codificação."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pt/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words para .NET fornece o namespace [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/), que simplifica as tarefas comuns de processamento de documentos. Este API é projetado para desenvolvedores que desejam realizar operações de alto nível, como comparação de documentos, extração de conteúdo, conversão de imagens e substituição de texto com o mínimo esforço.

O LowCode API é ideal para cenários em que a implementação rápida é mais importante do que o controlo refinado. Vamos dar uma olhada mais de perto nas capacidades LowCode de Aspose.Words para .NET.

{{% alert color="primary" %}}

É importante notar que o LowCode API não permite alterar a estrutura do documento.

{{% /alert %}}

## Recursos disponíveis em LowCode API

O namespace `Aspose.Words.LowCode` suporta atualmente:

* **Converting** documentos de um formato para outro
* **Comparing** documentos
* **Mail merging**
* **Reporting** baseado na sintaxe LINQ
* **Merging** documentos
* **Search and replace**
* **Digital signing** dos documentos
* **Splitting** um documento em partes utilizando critérios diferentes
* Adicionando um **watermark**

{{% alert color="primary" %}}

Observe que uma descrição detalhada de cada função fora de Low Code pode ser encontrada na seção do Guia do desenvolvedor.

{{% /alert %}}

## Fluente e não fluente API

Aspose.Words Para .NET suporta Fluent e Non-Fluent APIs, permitindo que os desenvolvedores escolham o estilo que melhor se adapta às suas preferências de codificação e necessidades do projeto. Vejamos alguns exemplos para ver como esses dois tipos de API diferem.

{{% alert color="primary" %}}

No fluente API, as operações podem ser configuradas e executadas através de um contexto (como ComparerContext ou ReplacerContext). Este contexto contém opções comuns. Assegura que todos os métodos relacionados funcionam com uma configuração consistente, tornando o API poderoso e fácil de gerir em cenários complexos.

{{% /alert %}}

### Comparar Documentos

Use `LowCode` para comparar dois Word documentos e salvar o resultado.

**exemplo de api não fluente:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**exemplo de API fluente:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

Você também pode passar `CompareOptions` para comparação ajustada.

**exemplo de api não fluente:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

CompareOptions options = new CompareOptions
{
    IgnoreFormatting = true,
    IgnoreCaseChanges = true
};

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc, options);
{{< /highlight >}}

**exemplo de API fluente:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

ComparerContext comparerContext = new ComparerContext();
comparerContext.CompareOptions.IgnoreCaseChanges = true;

Comparer.Create(comparerContext)
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.3.docx")
   .Execute();
{{< /highlight >}}

### Converter documento em imagens

Use `LowCode` para converter Word documento em PDF.

**exemplo de api não fluente:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**exemplo de API fluente:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Localizar e substituir texto

Use `LowCode` para substituir rapidamente o texto em todo o documento.

**exemplo de api não fluente:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**exemplo de API fluente:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";

ReplacerContext replacerContext = new ReplacerContext();
replacerContext.SetReplacement("ReplaceMe", "Replacement");

Replacer.Create(replacerContext)
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

## Porquê Utilizar Aspose.Words Low Code

O namespace **Aspose.Words.LowCode** ajuda a implementar rapidamente tarefas de processamento de documentos de alto nível com uma sintaxe limpa e legível. É especialmente útil para desenvolvedores que precisam de velocidade, simplicidade e Código sustentável ao trabalhar com documentos Word.

Para explorar opções mais avançadas, você sempre pode combinar LowCode APIs com o modelo de objeto completo Aspose.Words. Veja mais Low Code Exemplos em [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).