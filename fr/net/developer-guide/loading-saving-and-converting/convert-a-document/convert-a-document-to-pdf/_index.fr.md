---
title: Convertir Word en PDF en C#
second_title: Aspose.Words pour .NET
articleTitle: Transformer un document en PDF
linktitle: Transformer un document en PDF
description: "Convertir Word en PDF en C#. Exemples de code simples pour conversion DOCX en PDF. Prend en charge tous les formats Word et images."
type: docs
weight: 10
url: /fr/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

La capacité de convertir facilement et de manière fiable des documents d'un format à un autre est une fonctionnalité clé d'Aspose.Words. Le PDF est l'un des formats les plus populaires pour la conversion – c'est un format à mise en page fixe qui préserve l'apparence originale d'un document lors de son rendu sur diverses plateformes. Le terme "rendu" est utilisé dans Aspose.Words pour décrire le processus de transformation d'un document vers un format de fichier paginé ou ayant le concept de pages.

## Convertir un document Word en PDF

La conversion de Word en PDF est un processus assez complexe qui nécessite plusieurs étapes de calcul. Le moteur de mise en page d'Aspose.Words imite le fonctionnement du moteur de mise en page de Microsoft Word, rendant les documents PDF de sortie aussi proches que possible de ce que vous pouvez voir dans Microsoft Word.

Avec Aspose.Words, vous pouvez convertir par programmation un document depuis des formats Word, tels que DOC ou DOCX, vers PDF sans utiliser Microsoft Office. Cet article explique comment effectuer cette transformation.

{{% alert color="primary" %}}

Notez que le nombre de pages dans un document affecte le temps de conversion.

{{% /alert %}}

### Convertir DOCX ou DOC en PDF

La transformation des formats de document DOC ou DOCX vers le format PDF dans Aspose.Words est très facile et peut être accomplie avec seulement deux lignes de code qui :

1. Chargez votre document dans un objet [Document](https://reference.aspose.com/words/net/aspose.words/document/) en utilisant l'un de ses constructeurs en spécifiant le nom du document avec son extension de format.
1. Invoquez l'une des méthodes [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) sur l'objet **Document** et spécifiez le format de sortie désiré comme PDF en entrant un nom de fichier avec l'extension ".PDF".

L'exemple de code suivant montre comment convertir un document de DOCX en PDF en utilisant la méthode [Save](https://reference.aspose.com/words/net/aspose.words/document/save/) :

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Vous pouvez télécharger le fichier modèle de cet exemple depuis [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Parfois, il est nécessaire de spécifier des options supplémentaires qui peuvent affecter le résultat de la sauvegarde d'un document en PDF. Ces options peuvent être spécifiées en utilisant la classe [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), contenant des propriétés qui déterminent comment la sortie PDF sera affichée.

Notez qu'avec la même technique, vous pouvez transformer tout document au format de mise en page fluide vers le format PDF.

{{% /alert %}}

### Convertir vers différents standards PDF

Aspose.Words fournit l'énumération [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) pour prendre en charge la conversion de DOC ou DOCX vers différents standards de format PDF (comme PDF 1.7, PDF 1.5, etc.).

L'exemple de code suivant démontre comment changer un document vers PDF 1.7 en utilisant [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) avec conformité à PDF17 :

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Convertir des images en PDF

La conversion vers PDF n'est pas restreinte aux formats de documents Microsoft Word. Tout format pris en charge par Aspose.Words, y compris ceux créés par programmation, peut également être transformé en PDF. Par exemple, nous pouvons convertir des images à page unique, telles que JPEG, PNG, BMP, EMF, ou WMF, ainsi que des images multi-pages, telles que TIFF et GIF, en PDF.

L'exemple de code suivant montre comment changer des images JPEG et TIFF en PDF :

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Pour que ce code fonctionne, vous devez ajouter des références à Aspose.Words et `System.Drawing` dans votre projet.

## Réduire la taille de sortie PDF

Lors de la sauvegarde en PDF, vous pouvez spécifier si vous souhaitez optimiser la sortie. Pour ce faire, vous devez définir le drapeau [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) sur true, et alors les toiles imbriquées redondantes et vides seront supprimées, les glyphes voisins avec la même mise en forme seront concaténés.

L'exemple de code suivant montre comment optimiser la sortie :

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

L'utilisation de la propriété **OptimizeOutput** peut affecter la précision de l'affichage du contenu.

{{% /alert %}}

## Voir aussi

- L'article [Rendu](/words/fr/net/rendering/) pour plus d'informations sur les formats de page fixe et de mise en page fluide
- L'article [Conversion vers un format de page fixe](/words/net/converting-to-fixed-page-format/#what-is-a-page-layout) pour plus d'informations sur la mise en page
- L'article [Spécifier les options de rendu lors de la transformation en PDF](/words/fr/net/specify-rendering-options-when-converting-to-pdf/) pour plus d'informations sur l'utilisation de la classe `PdfSaveOptions`
- L'article [Apprenez les fonctionnalités de conversion vers PDF/A et PDF/UA](/words/fr/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) décrivant quel standard PDF et les ISO pertinents pour les standards PDF sont pris en charge par Aspose.Words
- L'article [Quel standard PDF est préférable de choisir](/words/fr/net/which-pdf-standard-is-better-to-choose/) pour déterminer quels standards PDF conviennent à quels cas

- L'article [Travailler avec PDF/A ou PDF/UA](/words/fr/net/working-with-pdfa-or-pdfua/) décrit les exigences pour le contenu du document dans les formats PDF/A et PDF/UA – principalement les exigences pour la structure et les polices

- L'article [Avertissements de problèmes d'accessibilité lors de la sauvegarde en PDF/A et PDF/UA](/words/fr/net/warnings-when-saving-to-pdfa-and-pdfua/) décrit quelles exigences d'accessibilité du contenu imposent PDF/A et PDF/UA
