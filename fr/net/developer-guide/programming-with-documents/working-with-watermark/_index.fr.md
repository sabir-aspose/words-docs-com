---
title: Utilisation du filigrane dans C#
second_title: Aspose.Words pour .NET
articleTitle: Travailler avec un filigrane
linktitle: Travailler avec un filigrane
description: "Manipulation du filigrane du document à l'aide de C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Cette rubrique explique comment travailler par programmation avec un filigrane à l'aide de Aspose.Words. Un filigrane est une image d'arrière-plan qui s'affiche derrière le texte d'un document. Un filigrane peut contenir un texte ou une image représentée par la classe [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Essayez en ligne**

Vous pouvez essayer cette fonctionnalité avec notre [Filigrane de document en ligne gratuit](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Ajouter un filigrane à un document

Dans Microsoft Word, un filigrane peut facilement être inséré dans un document à l'aide de la commande Insérer un filigrane. Aspose.Words fournit la classe [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) pour ajouter ou supprimer un filigrane dans les documents. Aspose.Words fournit l'énumération [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)définissant trois types de filigranes possibles (Texte, Image et Aucun) avec lesquels travailler.

### Ajouter Un Filigrane De Texte

L'exemple de code suivant montre comment insérer un filigrane de texte dans un document en définissant [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) à l'aide de la méthode [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Ajouter Un Filigrane D'Image

L'exemple de code suivant montre comment insérer un filigrane d'image dans un document en définissant [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) à l'aide de la méthode [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Le filigrane d'image peut être inséré en tant qu'image, chaîne ou flux.

Le filigrane peut également être inséré à l'aide de la classe de forme. Il est très facile d'insérer n'importe quelle forme ou image dans un en-tête ou un pied de page et ainsi créer un filigrane de n'importe quel type imaginable.

L'exemple de code suivant insère un filigrane dans un document Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Vous pouvez télécharger le fichier d'exemple de cet exemple à partir de [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Supprimer le filigrane d'un document

La classe [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) fournit la méthode remove pour supprimer le filigrane d'un document.

L'exemple de code suivant montre comment supprimer un filigrane des documents:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Si les filigranes sont ajoutés à l'aide de l'objet de classe [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/), pour supprimer le filigrane d'un document, vous devez définir uniquement le nom de la forme du filigrane lors de l'insertion, puis supprimer la forme du filigrane par un nom attribué.

L'exemple de code suivant vous montre comment définir le nom de la forme de filigrane et la supprimer du document:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Ajouter un filigrane dans une cellule de tableau

Parfois, vous devez insérer un filigrane/une image dans la cellule d'un tableau et l'afficher en dehors du tableau, vous pouvez utiliser la propriété [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). Cette propriété obtient ou définit un indicateur indiquant si la forme est affichée à l'intérieur ou à l'extérieur d'un tableau. Notez que cette propriété ne fonctionne que lorsque vous optimisez le document pour Microsoft Word 2010 à l'aide de la méthode [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

L'exemple de code suivant montre comment utiliser cette propriété:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
