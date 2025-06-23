---
title: Converter um documento de várias páginas numa imagem em Java
second_title: Aspose.Words para Java
articleTitle: Converter um documento de várias páginas numa imagem
linktitle: Converter um documento de várias páginas numa imagem
type: docs
description: "Exportar documentos de várias páginas para imagens rasterizadas (JPG, PNG, GIF, BMP, TIFF, WebP) Usando Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pt/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words para Java permite aos utilizadores exportar documentos de várias páginas para imagens rasterizadas. Isso pode ser útil para gerar visualizações, arquivos ou representações visuais de documentos para uso não editável.

## Quais formatos suportam a exportação de várias páginas?

Aspose.Words suporta exportação de várias páginas para os seguintes formatos de Imagem raster:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Como exportar um documento de várias páginas para uma imagem

O recurso de exportar um documento de várias páginas para uma imagem é implementado usando a classe [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) – você pode especificar como as páginas devem ser organizadas ao salvar em uma imagem:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - guardar apenas a primeira das páginas especificadas
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - organizar as páginas numa grelha, da esquerda para a direita e de cima para baixo, especificando o número de colunas
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - organizar as páginas horizontalmente lado a lado, da esquerda para a direita, numa única saída
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - organizar as páginas verticalmente uma abaixo da outra em uma única saída
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) - organizar cada página como um quadro separado em uma imagem multi-quadro TIFF, aplica-se apenas aos formatos de imagem TIFF 

O exemplo de código a seguir mostra como salvar um documento DOCX de várias páginas como imagem JPEG com layout Horizontal:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Você também pode personalizar a aparência da página do arquivo de saída-especifique [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) e [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

O exemplo de código a seguir mostra como salvar um documento DOCX de várias páginas como imagem PNG com layout de grade:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.PNG);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.setPageLayout(MultiPageLayout.grid(3, 10f, 10f));

// Customize the background and border.
options.getPageLayout().setBackColor(Color.lightGray);
options.getPageLayout().setBorderColor(Color.BLUE);
options.getPageLayout().setBorderWidth(2f);

doc.save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}