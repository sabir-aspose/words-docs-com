---
title: Customize Field Properties in Node.js
second_title: Aspose.Words for Node.js via .NET
articleTitle: Customize Field Properties
linktitle: Customize Field Properties
description: "Learn how to customize field properties in Node.js. Rename merge fields or obtain results for fields without separator node in Node.js via .NET."
type: docs
weight: 27
ai_search_scope: words_nodejs
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nodejs-net/customize-field-properties/
timestamp: 2025-07-09-10-05-05
---

Aspose.Words provides the ability to programmatically interact with various field properties. In this article, we will look at a couple of examples so that you understand the basic principle of working with field properties. You can see the full list of properties for each field type in the corresponding class in the [Fields module](https://reference.aspose.com/words/nodejs-net/aspose.words.fields/).

## Field Property Update

Sometimes users need to change the value of a field property. For example, update the [authorName](https://reference.aspose.com/words/nodejs-net/aspose.words.fields/fieldauthor/authorname/) property of the `AUTHOR` field or change the [fieldName](https://reference.aspose.com/words/nodejs-net/aspose.words.fields/fieldmergefield/fieldname/) property of the `MERGEFIELD` field.

The following code example shows how to rename merge fields in a Word document:

{{< gist "aspose-words-gists" "ce43c0268e53b9e7df2f581cafc2d748" "rename-merge-fields.js" >}}

## Field Display Result

Aspose.Words provides a property to obtain the field's result for fields that do not have a field separator node. We call this "fake result" or display result; MS Word displays it in the document by calculating the field's value on the fly, but there is no such value in the document model.

The following code example shows the usage of [displayResult](https://reference.aspose.com/words/nodejs-net/aspose.words/field/displayresult/) property:

{{< gist "aspose-words-gists" "ce43c0268e53b9e7df2f581cafc2d748" "field-display-results.js" >}}
