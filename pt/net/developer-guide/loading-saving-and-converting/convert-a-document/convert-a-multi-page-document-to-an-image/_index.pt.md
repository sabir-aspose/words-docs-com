---
title: Converter um documento de várias páginas numa imagem em C#
second_title: Aspose.Words para .NET
articleTitle: Converter um documento de várias páginas numa imagem
linktitle: Converter um documento de várias páginas numa imagem
type: docs
description: "Exportar documentos de várias páginas para imagens rasterizadas (JPG, PNG, GIF, BMP, TIFF, WebP) Usando C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pt/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words para .NET permite aos utilizadores exportar documentos de várias páginas para imagens rasterizadas. Isso pode ser útil para gerar visualizações, arquivos ou representações visuais de documentos para uso não editável.

## Quais formatos suportam a exportação de várias páginas?

Aspose.Words suporta exportação de várias páginas para os seguintes formatos de Imagem raster:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Como exportar um documento de várias páginas para uma imagem

O recurso de exportar um documento de várias páginas para uma imagem é implementado usando a classe [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) – você pode especificar como as páginas devem ser organizadas ao salvar em uma imagem:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - guardar apenas a primeira das páginas especificadas
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - organizar as páginas numa grelha, da esquerda para a direita e de cima para baixo, especificando o número de colunas
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - organizar as páginas horizontalmente lado a lado, da esquerda para a direita, numa única saída
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - organizar as páginas verticalmente uma abaixo da outra em uma única saída
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) - organizar cada página como um quadro separado em uma imagem multi-quadro TIFF, aplica-se apenas aos formatos de imagem TIFF 

O exemplo de código a seguir mostra como salvar um documento DOCX de várias páginas como imagem JPEG com layout Horizontal:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Você também pode personalizar a aparência da página do arquivo de saída-especifique [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) e [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

O exemplo de código a seguir mostra como salvar um documento DOCX de várias páginas como imagem PNG com layout de grade:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Png);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.PageLayout = MultiPageLayout.Grid(3, 10, 10);

// Customize the background and border.
options.PageLayout.BackColor = Color.LightGray;
options.PageLayout.BorderColor = Color.Blue;
options.PageLayout.BorderWidth = 2;

doc.Save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}