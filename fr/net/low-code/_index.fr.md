---
title: Low Code
second_title: Aspose.Words pour .NET
articleTitle: Travailler avec des Documents en utilisant LowCode API
linktitle: Low Code
type: docs
description: "Simplifiez les tâches de traitement de documents telles que comparer, convertir, diviser, fusionner, rechercher et remplacer, et d'autres en utilisant Low Code API. Aspose.Words LowCode API avec une syntaxe claire, des résultats rapides et un effort de codage minimal."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /fr/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words pour .NET fournit l'espace de noms [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/), qui simplifie les tâches courantes de traitement des documents. Ce API est conçu pour les développeurs qui souhaitent effectuer des opérations de haut niveau telles que la comparaison de documents, l'extraction de contenu, la conversion d'images et le remplacement de texte avec un minimum d'effort.

Le LowCode API est idéal pour les scénarios où une mise en œuvre rapide est plus importante qu'un contrôle précis. Examinons de plus près les LowCode capacités de Aspose.Words pour .NET.

{{% alert color="primary" %}}

Il est important de noter que le LowCode API ne vous permet pas de modifier la structure du document.

{{% /alert %}}

## Fonctionnalités disponibles dans LowCode API

L'espace de noms `Aspose.Words.LowCode` prend actuellement en charge:

* **Converting** documents d'un format à l'autre
* **Comparing** documents
* **Mail merging**
* **Reporting** basé sur la syntaxe LINQ
* **Merging** documents
* **Search and replace**
* **Digital signing** de documents
* **Splitting** un document en plusieurs parties utilisant différents critères
* Ajout d'un **watermark**

{{% alert color="primary" %}}

Veuillez noter qu'une description détaillée de chaque fonction en dehors de Low Code se trouve dans la section Guide du développeur.

{{% /alert %}}

## Courant et Non courant API

Aspose.Words pour .NET prend en charge à la fois Couramment et Non couramment APIs, permettant aux développeurs de choisir le style qui correspond le mieux à leurs préférences de codage et aux besoins de leur projet. Regardons quelques exemples pour voir en quoi ces deux types de API diffèrent.

{{% alert color="primary" %}}

Dans le courant API, les opérations peuvent être configurées et exécutées via un contexte (tel que ComparerContext ou ReplacerContext). Ce contexte contient des options communes. Il garantit que toutes les méthodes associées fonctionnent avec une configuration cohérente, ce qui rend le API puissant et facile à gérer dans des scénarios complexes.

{{% /alert %}}

### Comparer des Documents

Utilisez `LowCode` pour comparer deux documents Word et enregistrer le résultat.

**exemple d'API non fluide:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**exemple d'api fluide:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

Vous pouvez également passer `CompareOptions` pour une comparaison affinée.

**exemple d'API non fluide:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

CompareOptions options = new CompareOptions
{
    IgnoreFormatting = true,
    IgnoreCaseChanges = true
};

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc, options);
{{< /highlight >}}

**exemple d'api fluide:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

ComparerContext comparerContext = new ComparerContext();
comparerContext.CompareOptions.IgnoreCaseChanges = true;

Comparer.Create(comparerContext)
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.3.docx")
   .Execute();
{{< /highlight >}}

### Convertir un document en Images

Utilisez `LowCode` pour convertir le document Word en PDF.

**exemple d'API non fluide:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**exemple d'api fluide:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Rechercher et remplacer du Texte

Utilisez `LowCode` pour remplacer rapidement du texte dans l'ensemble du document.

**exemple d'API non fluide:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**exemple d'api fluide:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";

ReplacerContext replacerContext = new ReplacerContext();
replacerContext.SetReplacement("ReplaceMe", "Replacement");

Replacer.Create(replacerContext)
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

## Pourquoi utiliser Aspose.Words Low Code

L'espace de noms **Aspose.Words.LowCode** vous aide à implémenter rapidement des tâches de traitement de documents de haut niveau avec une syntaxe claire et lisible. Il est particulièrement utile pour les développeurs qui ont besoin de rapidité, de simplicité et de code maintenable lorsqu'ils travaillent avec des documents Word.

Pour explorer des options plus avancées, vous pouvez toujours combiner LowCode APIs avec le modèle d'objet Aspose.Words complet. Voir plus d'exemples Low Code dans le [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).