---
title: Hoe vind ik veldeigenschappen in C#
second_title: Aspose.Words voor .NET
articleTitle: Veldeigenschappen zoeken
linktitle: Veldeigenschappen zoeken
description: "Hoe vind ik een aantal veldeigenschappen zoals veldcode en veld resulteert in C#."
type: docs
weight: 25
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nl/net/find-field-properties/
timestamp: 2024-01-27-14-07-04
---

Een veld dat wordt ingevoegd met behulp van [DocumentBuilder](https://reference.aspose.com/words/net/aspose.words/documentbuilder/).[InsertField](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertfield/) geeft a [Field](https://reference.aspose.com/words/net/aspose.words.fields/field/) object. Dit is een gevelklasse die handige methoden biedt om snel enkele eigenschappen van een veld te vinden.

Het volgende voorbeeld van code laat zien hoe u de veldcode en het veldresultaat kunt vinden:

{{< gist "aspose-words-gists" "eacc4fc7407a98d683f3084bb86d58f7" "Examples-CSharp-Programming-Documents-Fields-FieldCode.cs" >}}

Opmerking als u alleen op zoek bent naar de namen van merge velden in een document, dan kunt u in plaats daarvan de ingebouwde [GetFieldNames](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/getfieldnames/) methode.

Het volgende voorbeeld van code laat zien hoe je namen van alle merge velden in een document krijgt:

{{< gist "aspose-words-gists" "eacc4fc7407a98d683f3084bb86d58f7" "Examples-CSharp-Programming-Documents-Fields-GetFieldNames-GetFieldNames.cs" >}}
