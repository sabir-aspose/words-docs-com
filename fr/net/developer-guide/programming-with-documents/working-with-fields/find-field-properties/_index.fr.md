---
title: Comment trouver les propriétés de champ dans C#
second_title: Aspose.Words pour .NET
articleTitle: Rechercher les propriétés du champ
linktitle: Rechercher les propriétés du champ
description: "Comment trouver certaines propriétés de champ telles que le code de champ et le résultat du champ dans C#."
type: docs
weight: 25
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/net/find-field-properties/
timestamp: 2024-01-27-14-07-04
---

Un champ inséré à l'aide de [DocumentBuilder](https://reference.aspose.com/words/fr/net/aspose.words/documentbuilder/).[InsertField](https://reference.aspose.com/words/fr/net/aspose.words/documentbuilder/insertfield/) renvoie un objet [Field](https://reference.aspose.com/words/fr/net/aspose.words.fields/field/). Il s'agit d'une classe de façade qui fournit des méthodes utiles pour trouver rapidement certaines propriétés d'un champ.

L'exemple de code suivant montre comment trouver le code de champ et le résultat du champ:

{{< gist "aspose-words-gists" "eacc4fc7407a98d683f3084bb86d58f7" "Examples-CSharp-Programming-Documents-Fields-FieldCode.cs" >}}

Notez que si vous recherchez uniquement les noms des champs de fusion dans un document, vous pouvez utiliser la méthode [GetFieldNames](https://reference.aspose.com/words/fr/net/aspose.words.mailmerging/mailmerge/getfieldnames/) intégrée.

L'exemple de code suivant montre comment obtenir les noms de tous les champs de fusion dans un document:

{{< gist "aspose-words-gists" "eacc4fc7407a98d683f3084bb86d58f7" "Examples-CSharp-Programming-Documents-Fields-GetFieldNames-GetFieldNames.cs" >}}
