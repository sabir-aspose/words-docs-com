---
title: Convertir un document de plusieurs pages en une image dans Python
second_title: Aspose.Words pour Python
articleTitle: Convertir un document de plusieurs pages en image
linktitle: Convertir un document de plusieurs pages en image
type: docs
description: "Exporter des documents de plusieurs pages vers des images raster(JPG, PNG, GIF, BMP, TIFF, WebP) en utilisant Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words pour Python via .NET permet aux utilisateurs d'exporter des documents de plusieurs pages vers des images raster. Cela peut être utile pour générer des aperçus, des archives ou des représentations visuelles de documents pour une utilisation non modifiable.

## Quels Formats Prennent En Charge L'Exportation Multipage?

Aspose.Words prend en charge l'exportation multipage vers les formats d'image raster suivants:

* JPEG
* GIF
* PNG
* PRM
* Tiff
* WebP

## Comment exporter un Document de plusieurs pages vers une Image

La fonctionnalité d'exportation d'un document de plusieurs pages vers une image est implémentée à l'aide de la classe [MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) – vous pouvez spécifier comment les pages doivent être organisées lors de l'enregistrement dans une image:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/) - enregistre uniquement la première des pages spécifiées
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float) - disposez les pages dans une grille, de gauche à droite et de haut en bas, tout en spécifiant le nombre de colonnes
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float) - disposez les pages horizontalement côte à côte, de gauche à droite, en une seule sortie
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float) - disposez les pages verticalement les unes au-dessous des autres en une seule sortie
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/) – organise chaque page comme un cadre séparé dans une image TIFF multi-images, s'applique uniquement aux formats d'image TIFF 

L'exemple de code suivant montre comment enregistrer un document DOCX de plusieurs pages en tant qu'image JPEG avec une mise en page horizontale:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

Vous pouvez également personnaliser l'apparence de la page du fichier de sortie – spécifiez [back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/), [border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/) et [border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

L'exemple de code suivant montre comment enregistrer un document DOCX de plusieurs pages en tant qu'image PNG avec une disposition en grille:

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