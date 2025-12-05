---
title: Convertir un document de plusieurs pages en une image dans Java
second_title: Aspose.Words pour Java
articleTitle: Convertir un document de plusieurs pages en image
linktitle: Convertir un document de plusieurs pages en image
type: docs
description: "Exporter des documents de plusieurs pages vers des images raster(JPG, PNG, GIF, BMP, TIFF, WebP) en utilisant Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Words pour Java permet aux utilisateurs d'exporter des documents de plusieurs pages vers des images raster. Cela peut être utile pour générer des aperçus, des archives ou des représentations visuelles de documents pour une utilisation non modifiable.

## Quels Formats Prennent En Charge L'Exportation Multipage?

Aspose.Words prend en charge l'exportation multipage vers les formats d'image raster suivants:

* JPEG
* GIF
* PNG
* PRM
* Tiff
* WebP

## Comment exporter un Document de plusieurs pages vers une Image

La fonctionnalité d'exportation d'un document de plusieurs pages vers une image est implémentée à l'aide de la classe [MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) – vous pouvez spécifier comment les pages doivent être organisées lors de l'enregistrement dans une image:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage) - enregistre uniquement la première des pages spécifiées
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float) - disposez les pages dans une grille, de gauche à droite et de haut en bas, tout en spécifiant le nombre de colonnes
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float) - disposez les pages horizontalement côte à côte, de gauche à droite, en une seule sortie
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float) - disposez les pages verticalement les unes au-dessous des autres en une seule sortie
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames) – organise chaque page comme un cadre séparé dans une image TIFF multi-images, s'applique uniquement aux formats d'image TIFF 

L'exemple de code suivant montre comment enregistrer un document DOCX de plusieurs pages en tant qu'image JPEG avec une mise en page horizontale:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

Vous pouvez également personnaliser l'apparence de la page du fichier de sortie – spécifiez [BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor), [BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor) et [BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

L'exemple de code suivant montre comment enregistrer un document DOCX de plusieurs pages en tant qu'image PNG avec une disposition en grille:

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