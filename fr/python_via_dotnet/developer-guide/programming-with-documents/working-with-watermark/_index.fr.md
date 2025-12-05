---
title: Utilisation du filigrane dans Python
second_title: Aspose.Words pour Python via .NET
articleTitle: Travailler avec un filigrane
linktitle: Travailler avec un filigrane
description: "Créez et gérez des filigranes dans un document à l'aide de Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Cette rubrique explique comment travailler par programmation avec un filigrane à l'aide de Aspose.Words. Un filigrane est une image d'arrière-plan qui s'affiche derrière le texte d'un document. Un filigrane peut contenir un texte ou une image représentée par la classe [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Essayez en ligne**

Vous pouvez essayer cette fonctionnalité avec notre [Filigrane de document en ligne gratuit](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Comment ajouter un filigrane à un Document

Dans Microsoft Word, un filigrane peut facilement être inséré dans un document à l'aide de la commande Insérer un filigrane. Aspose.Words fournit la classe [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) pour ajouter ou supprimer un filigrane dans les documents. Aspose.Words fournit l'énumération [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) définissant trois types possibles de filigranes ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) et [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) avec lesquels travailler.

### Ajouter Un Filigrane De Texte

L'exemple de code suivant montre comment insérer un filigrane de texte dans un document en définissant [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) à l'aide de la méthode [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### Ajouter Un Filigrane D'Image

L'exemple de code suivant montre comment insérer un filigrane d'image dans un document en définissant [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) à l'aide de la méthode [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

Le filigrane d'image peut être inséré en tant qu'image, chaîne ou flux.

Le filigrane peut également être inséré à l'aide de la classe de forme. Il est très facile d'insérer n'importe quelle forme ou image dans un en-tête ou un pied de page et ainsi créer un filigrane de n'importe quel type imaginable.

L'exemple de code suivant insère un filigrane dans un document Word:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

Vous pouvez télécharger le fichier modèle de cet exemple à partir de [ici](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Supprimer le filigrane d'un document

La classe [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) fournit la méthode remove pour supprimer le filigrane d'un document.

L'exemple de code suivant montre comment supprimer un filigrane des documents:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

Si les filigranes sont ajoutés à l'aide de l'objet de classe [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/), pour supprimer le filigrane d'un document, vous devez définir uniquement le nom de la forme du filigrane lors de l'insertion, puis supprimer la forme du filigrane par un nom attribué.

L'exemple de code suivant vous montre comment définir le nom de la forme de filigrane et la supprimer du document:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## Ajouter un filigrane dans la cellule du tableau

Parfois, vous devez insérer un filigrane/une image dans la cellule d'un tableau et l'afficher en dehors du tableau, vous pouvez utiliser la propriété [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/). Cette propriété obtient ou définit un indicateur indiquant si la forme est affichée à l'intérieur ou à l'extérieur d'un tableau. Notez que cette propriété ne fonctionne que lorsque vous optimisez le document pour Microsoft Word 2010 à l'aide de la méthode [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

L'exemple de code suivant montre comment utiliser cette propriété:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
