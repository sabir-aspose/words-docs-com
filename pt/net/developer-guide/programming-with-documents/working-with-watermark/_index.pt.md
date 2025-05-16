---
title: Trabalhando com marca D'água em C#
second_title: Aspose.Words Para .NET
articleTitle: Trabalhando com marca D'água
linktitle: Trabalhando com marca D'água
description: "Manipulação da marca d'água do documento usando C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pt/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Este tópico discute como trabalhar programaticamente com marca d'água usando Aspose.Words. Uma marca d'água é uma imagem de fundo que é exibida atrás do texto em um documento. Uma marca d'água pode conter um texto ou uma imagem representada pela classe [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Experimente online**

Pode experimentar esta funcionalidade com o nosso [Marca d'água de Documento on-line gratuita](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Adicionar uma marca D'água a um documento

Em Microsoft Word, uma marca d'água pode ser facilmente inserida em um documento usando o comando Inserir marca d'água. Aspose.Words fornece a classe [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) para adicionar ou remover marca d'água em documentos. Aspose.Words fornece a enumeração [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)definindo três tipos possíveis de marcas d'água (texto, imagem e nenhum) para trabalhar.

### Adicionar Marca D'Água De Texto

O exemplo de código a seguir demonstra como inserir uma marca d'água de texto em um documento definindo [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) usando o método [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Adicionar Marca D'Água De Imagem

O exemplo de código a seguir demonstra como inserir uma marca d'água de imagem em um documento definindo [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) usando o método [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

A marca d'água da imagem pode ser inserida como imagem, string ou fluxo.

A marca d'água também pode ser inserida usando a classe shape. É muito fácil inserir qualquer forma ou imagem em um cabeçalho ou rodapé e, assim, criar uma marca d'água de qualquer tipo imaginável.

O exemplo de código a seguir insere uma marca d'água em um documento Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Você pode baixar o arquivo de exemplo deste exemplo em [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Remover marca D'água de um documento

A classe [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) fornece o método remove Para remover a marca d'água de um documento.

O exemplo de código a seguir mostra como remover uma marca d'água de documentos:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Se as marcas d'água forem adicionadas usando o objeto de classe [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/), para remover a marca d'água de um documento, você deve definir apenas o nome da forma da marca d'água durante a inserção e, em seguida, remover a forma da marca d'água por um nome atribuído.

O exemplo de código a seguir mostra como definir o nome da forma da marca d'água e removê-la do documento:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Adicionar uma marca D'água a uma célula da tabela

Às vezes você precisa inserir uma marca d'água/Imagem na célula de uma tabela e exibi-la fora da tabela, você pode usar a propriedade [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). Esta propriedade obtém ou define um sinalizador indicando se a forma é exibida dentro ou fora de uma tabela. Observe que essa propriedade só funciona quando você otimiza o documento para Microsoft Word 2010 usando o método [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

O exemplo de código a seguir mostra como usar essa propriedade:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
