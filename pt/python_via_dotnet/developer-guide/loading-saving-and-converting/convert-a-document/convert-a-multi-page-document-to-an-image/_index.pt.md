---
title: Converter um documento de várias páginas numa imagem em Python
second_title: Aspose.Words para Python
articleTitle: Converter um documento de várias páginas numa imagem
linktitle: Converter um documento de várias páginas numa imagem
type: docs
description: "Exportar documentos de várias páginas para imagens rasterizadas (JPG, PNG, GIF, BMP, TIFF, WebP) Usando Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pt/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words Para Python via .NET permite aos utilizadores exportar documentos de várias páginas para imagens rasterizadas. Isso pode ser útil para gerar visualizações, arquivos ou representações visuais de documentos para uso não editável.

## Quais formatos suportam a exportação de várias páginas?

Aspose.Words suporta exportação de várias páginas para os seguintes formatos de Imagem raster:

* Jpeg
* Gif
* Png
* Bmp
* Tiff
* WebP

## Como exportar um documento de várias páginas para uma imagem

O recurso de exportar um documento de várias páginas para uma imagem é implementado usando a classe [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) – você pode especificar como as páginas devem ser organizadas ao salvar em uma imagem:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - guardar apenas a primeira das páginas especificadas
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - organizar as páginas numa grelha, da esquerda para a direita e de cima para baixo, especificando o número de colunas
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - organizar as páginas horizontalmente lado a lado, da esquerda para a direita, numa única saída
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - organizar as páginas verticalmente uma abaixo da outra em uma única saída
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) - organizar cada página como um quadro separado em uma imagem multi-quadro TIFF, aplica-se apenas aos formatos de imagem TIFF 

O exemplo de código a seguir mostra como salvar um documento DOCX de várias páginas como imagem JPEG com layout Horizontal:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Você também pode personalizar a aparência da página do arquivo de saída-especifique [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) e [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

O exemplo de código a seguir mostra como salvar um documento DOCX de várias páginas como imagem PNG com layout de grade:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.PNG)
# Set up a grid layout with:
# - 3 columns per row.
# - 10pts spacing between pages (horizontal and vertical).
options.page_layout = aw.saving.MultiPageLayout.grid(3, 10, 10)

# Customize the background and border.
options.page_layout.back_color = aspose.pydrawing.Color.light_gray
options.page_layout.border_color = aspose.pydrawing.Color.blue
options.page_layout.border_width = 2

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}