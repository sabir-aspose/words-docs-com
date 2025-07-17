---
title: Converter Word para PDF em C#
second_title: Aspose.Words para .NET
articleTitle: Transformar documento para PDF
linktitle: Transformar documento para PDF
description: "Converter Word para PDF em C#. Exemplos de código simples para conversão de DOCX para PDF. Suporta todos os formatos Word e imagens."
type: docs
weight: 10
url: /pt/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

A capacidade de converter documentos fácil e confiavelmente de um formato para outro é uma característica fundamental do Aspose.Words. PDF é um dos formatos mais populares para conversão – é um formato de layout fixo que preserva a aparência original de um documento durante a renderização em várias plataformas. O termo "renderização" é usado no Aspose.Words para descrever o processo de conversão de um documento para um formato de arquivo paginado ou que tem o conceito de páginas.

## Converter documento Word para PDF

A conversão de Word para PDF é um processo bastante complexo que requer várias etapas de cálculo. O mecanismo de layout do Aspose.Words imita a maneira como o mecanismo de layout de páginas do Microsoft Word funciona, fazendo com que os documentos PDF de saída pareçam o mais próximo possível do que você pode ver no Microsoft Word.

Com o Aspose.Words, você pode transformar programaticamente um documento de formatos Word, como DOC ou DOCX, para PDF sem usar o Microsoft Office. Este artigo explica como realizar essa conversão.

{{% alert color="primary" %}}

Note que o número de páginas em um documento afeta o tempo de conversão.

{{% /alert %}}

### Converter DOCX ou DOC para PDF

Transformar do formato de documento DOC ou DOCX para o formato PDF no Aspose.Words é muito fácil e pode ser realizado com apenas duas linhas de código que:

1. Carregue seu documento em um objeto [Document](https://reference.aspose.com/words/net/aspose.words/document/) usando um de seus construtores especificando o nome do documento com sua extensão de formato.
1. Invoque um dos métodos [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) no objeto **Document** e especifique o formato de saída desejado como PDF digitando um nome de arquivo com a extensão ".PDF".

O exemplo de código a seguir mostra como converter um documento de DOCX para PDF usando o método [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Você pode baixar o arquivo de modelo deste exemplo no [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Às vezes é necessário especificar opções adicionais que podem afetar o resultado de salvar um documento como PDF. Essas opções podem ser especificadas usando a classe [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), que contém propriedades que determinam como a saída PDF será exibida.

Note que com a mesma técnica você pode transformar qualquer documento de formato flow-layout para formato PDF.

{{% /alert %}}

### Converter para diferentes padrões PDF

O Aspose.Words fornece a enumeração [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) para suportar a conversão de DOC ou DOCX para vários padrões de formato PDF (como PDF 1.7, PDF 1.5, etc.).

O exemplo de código a seguir demonstra como mudar um documento para PDF 1.7 usando [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) com conformidade ao PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Converter imagens para PDF

A conversão para PDF não é restrita a formatos de documentos Microsoft Word. Qualquer formato suportado pelo Aspose.Words, incluindo aqueles criados programaticamente, também pode ser transformado para PDF. Por exemplo, podemos converter imagens de página única, como JPEG, PNG, BMP, EMF, ou WMF, bem como imagens de múltiplas páginas, como TIFF e GIF, para PDF.

O exemplo de código a seguir mostra como mudar imagens JPEG e TIFF para PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Para fazer este código funcionar, você precisa adicionar referências ao Aspose.Words e `System.Drawing` ao seu projeto.

## Reduzir o tamanho de saída PDF

Ao salvar para PDF, você pode especificar se deseja otimizar a saída. Para fazer isso, você precisa definir a flag [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) como true, e então telas aninhadas redundantes e vazias serão removidas, glifos adjacentes com a mesma formatação serão concatenados.

O exemplo de código a seguir mostra como otimizar a saída:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Usar a propriedade **OptimizeOutput** pode afetar a precisão da exibição do conteúdo.

{{% /alert %}}

## Veja também

- O artigo [Renderização](/words/pt/net/rendering/) para mais informações sobre formatos de página fixa e flow-layout
- O artigo [Conversão para formato de página fixa](/words/pt/net/converting-to-fixed-page-format/#what-is-a-page-layout) para mais informações sobre layout de página
- O artigo [Especificar opções de renderização ao transformar para PDF](/words/pt/net/specify-rendering-options-when-converting-to-pdf/) para mais informações sobre o uso da classe `PdfSaveOptions`
- O artigo [Aprenda os recursos de conversão para PDF/A e PDF/UA](/words/pt/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) que descreve qual padrão PDF e os ISOs relevantes para padrões PDF são suportados pelo Aspose.Words
- O artigo [Qual padrão PDF é melhor escolher](/words/pt/net/which-pdf-standard-is-better-to-choose/) para determinar quais padrões PDF fazem sentido para quais casos

- O artigo [Trabalhando com PDF/A ou PDF/UA](/words/pt/net/working-with-pdfa-or-pdfua/) descreve os requisitos para conteúdo do documento em formatos PDF/A e PDF/UA – principalmente os requisitos para estrutura e fontes

- O artigo [Avisos de problemas de acessibilidade ao salvar para PDF/A e PDF/UA](/words/pt/net/warnings-when-saving-to-pdfa-and-pdfua/) descreve quais requisitos de acessibilidade de conteúdo o PDF/A e PDF/UA impõem
