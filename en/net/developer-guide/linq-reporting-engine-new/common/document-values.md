---
draft: true {{/* Hide the page from rendering on its own. */}}
---
## Supported Values Providing Document Data

LINQ Reporting Engine supports working with values providing document data of the following types:
* A byte array containing document data
* A [`Stream`](https://learn.microsoft.com/en-us/dotnet/api/system.io.stream) instance able to read document data (the stream
is automatically closed after loading a document)
* An instance of the [`Document`](https://reference.aspose.com/words/net/aspose.words/document/) class
* A string containing a document [URI](https://en.wikipedia.org/wiki/Uniform_Resource_Identifier), path, or
[Base64](https://en.wikipedia.org/wiki/Base64)-encoded document data