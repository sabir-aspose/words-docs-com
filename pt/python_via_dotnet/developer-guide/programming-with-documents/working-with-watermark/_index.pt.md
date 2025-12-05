---
title: Trabalhando com marca D'água em Python
second_title: Aspose.Words para Python via .NET
articleTitle: Trabalhando com marca D'água
linktitle: Trabalhando com marca D'água
description: "Crie e gerencie marcas d'água em um documento usando Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pt/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Este tópico discute como trabalhar programaticamente com marca d'água usando Aspose.Words. Uma marca d'água é uma imagem de fundo que é exibida atrás do texto em um documento. Uma marca d'água pode conter um texto ou uma imagem representada pela classe [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Experimente online**

Pode experimentar esta funcionalidade com o nosso [Marca d'água de Documento on-line gratuita](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Como adicionar uma marca D'água a um documento

Em Microsoft Word, uma marca d'água pode ser facilmente inserida em um documento usando o comando Inserir marca d'água. Aspose.Words fornece a classe [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) para adicionar ou remover marca d'água em documentos. Aspose.Words fornece a enumeração [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) definindo três tipos possíveis de marcas d'água ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) e [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) para trabalhar.

### Adicionar Marca D'Água De Texto

O exemplo de código a seguir demonstra como inserir uma marca d'água de texto em um documento definindo [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) usando o método [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### Adicionar Marca D'Água De Imagem

O exemplo de código a seguir demonstra como inserir uma marca d'água de imagem em um documento definindo [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) usando o método [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

A marca d'água da imagem pode ser inserida como imagem, string ou fluxo.

A marca d'água também pode ser inserida usando a classe shape. É muito fácil inserir qualquer forma ou imagem em um cabeçalho ou rodapé e, assim, criar uma marca d'água de qualquer tipo imaginável.

O exemplo de código a seguir insere uma marca d'água em um documento Word:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

Você pode baixar o arquivo de modelo deste exemplo em [aqui](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Remover marca D'água de um documento

A classe [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) fornece o método remove Para remover a marca d'água de um documento.

O exemplo de código a seguir mostra como remover uma marca d'água de documentos:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

Se as marcas d'água forem adicionadas usando o objeto de classe [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/), para remover a marca d'água de um documento, você deve definir apenas o nome da forma da marca d'água durante a inserção e, em seguida, remover a forma da marca d'água por um nome atribuído.

O exemplo de código a seguir mostra como definir o nome da forma da marca d'água e removê-la do documento:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## Adicionar uma marca D'água na célula da tabela

Às vezes você precisa inserir uma marca d'água/Imagem na célula de uma tabela e exibi-la fora da tabela, você pode usar a propriedade [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/). Esta propriedade obtém ou define um sinalizador indicando se a forma é exibida dentro ou fora de uma tabela. Observe que essa propriedade só funciona quando você otimiza o documento para Microsoft Word 2010 usando o método [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

O exemplo de código a seguir mostra como usar essa propriedade:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
