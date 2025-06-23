---
title: Convertir un document de plusieurs pages en une image dans C#
second_title: Aspose.Words pour .NET
articleTitle: Convertir un document de plusieurs pages en image
linktitle: Convertir un document de plusieurs pages en image
type: docs
description: "Exporter des documents de plusieurs pages vers des images raster(JPG, PNG, GIF, BMP, TIFF, WebP) en utilisant C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /fr/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words pour .NET permet aux utilisateurs d'exporter des documents de plusieurs pages vers des images raster. Cela peut être utile pour générer des aperçus, des archives ou des représentations visuelles de documents pour une utilisation non modifiable.

## Quels Formats Prennent En Charge L'Exportation Multipage?

Aspose.Words prend en charge l'exportation multipage vers les formats d'image raster suivants:

* JPEG
* GIF
* PNG
* PRM
* Tiff
* WebP

## Comment exporter un Document de plusieurs pages vers une Image

La fonctionnalité d'exportation d'un document de plusieurs pages vers une image est implémentée à l'aide de la classe [MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) – vous pouvez spécifier comment les pages doivent être organisées lors de l'enregistrement dans une image:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/) - enregistre uniquement la première des pages spécifiées
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/) - disposez les pages dans une grille, de gauche à droite et de haut en bas, tout en spécifiant le nombre de colonnes
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/) - disposez les pages horizontalement côte à côte, de gauche à droite, en une seule sortie
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/) - disposez les pages verticalement les unes au-dessous des autres en une seule sortie
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/) – organise chaque page comme un cadre séparé dans une image TIFF multi-images, s'applique uniquement aux formats d'image TIFF 

L'exemple de code suivant montre comment enregistrer un document DOCX de plusieurs pages en tant qu'image JPEG avec une mise en page horizontale:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Vous pouvez également personnaliser l'apparence de la page du fichier de sortie – spécifiez [BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/), [BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/) et [BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

L'exemple de code suivant montre comment enregistrer un document DOCX de plusieurs pages en tant qu'image PNG avec une disposition en grille:

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