---
title: Accessing CSV Data in C#
second_title: Aspose.Words for .NET
articleTitle: Accessing CSV Data
linktitle: Accessing CSV Data
description: "Learn how to access CSV data while building a report using LINQ in C#."
type: docs
weight: 40
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/accessing-csv-data/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*What is this page about?*

This page outlines how to use CSV data in Aspose.Words reporting by connecting it through CsvDataSource for template-based document generation.

{{% /alert %}}

To access CSV data while building a report, you can pass a `CsvDataSource` instance to the engine as a data source.

Using of `CsvDataSource` enables you to work with typed values rather than just strings in template documents. Although CSV as a format does not define a way to store values of types other than strings, `CsvDataSource` is capable to recognize values of the following types by their string representations:

- Int64?
- Double?
- Boolean?
- DateTime?

**Note** – For recognition of data types to work, string representations of corresponding values must be formed using invariant culture settings.

In template documents, a`CsvDataSource` instance should be treated as a sequence of objects having corresponding fields as shown in the following example.

CSV

{{< highlight csv >}}
John Doe,30,1989-04-01 4:00:00 pm
Jane Doe,27,1992-01-31 07:00:00 am
John Smith,51,1968-03-08 1:00:00 pm
{{< /highlight >}}

Template document

{{< highlight xml >}}
<<foreach [in persons]>>Name: <<[Column1]>>, Age: <<[Column2]>>, Date of Birth: <<[Column3]:"dd.MM.yyyy">>
<</foreach>>

Average age: <<[persons.Average(p => p.Column2)]>>
{{< /highlight >}}

Source code

{{< highlight csharp >}}
Document doc = ...             // Loading a template document.
CsvDataSource dataSource = ... // Loading CSV.

ReportingEngine engine = new ReportingEngine();
engine.BuildReport(doc, dataSource, "persons");
{{< /highlight >}}

Result document

{{< highlight text >}}
Name: John Doe, Age: 30, Date of Birth: 01.04.1989
Name: Jane Doe, Age: 27, Date of Birth: 31.01.1992
Name: John Smith, Age: 51, Date of Birth: 08.03.1968

Average age: 36
{{< /highlight >}}

By default, `CsvDataSource` uses column names such as “Column1”, “Column2”, and so on, as you can see from the previous example. However, `CsvDataSource` can be configured to read column names from the first line of CSV data as shown in the following example.

CSV

{{< highlight csv >}}
Name,Age,Birth
John Doe,30,1989-04-01 4:00:00 pm
Jane Doe,27,1992-01-31 07:00:00 am
John Smith,51,1968-03-08 1:00:00 pm
{{< /highlight >}}

Template document

{{< highlight xml >}}
<<foreach [in persons]>>Name: <<[Name]>>, Age: <<[Age]>>, Date of Birth: <<[Birth]:"dd.MM.yyyy">>
<</foreach>>

Average age: <<[persons.Average(p => p.Age)]>>
{{< /highlight >}}

Source code

{{< highlight csharp >}}
Document doc = ... // Loading a template document.
CsvDataLoadOptions options = new CsvDataLoadOptions(true);
CsvDataSource dataSource = new CsvDataSource(..., options); // Loading CSV.

ReportingEngine engine = new ReportingEngine();
engine.BuildReport(doc, dataSource, "persons");
{{< /highlight >}}

Result document

{{< highlight text >}}
Name: John Doe, Age: 30, Date of Birth: 01.04.1989
Name: Jane Doe, Age: 27, Date of Birth: 31.01.1992
Name: John Smith, Age: 51, Date of Birth: 08.03.1968

Average age: 36
{{< /highlight >}}

Also, you can use `CsvDataLoadOptions` to customize the following characters playing special roles while loading CSV data:

- Value separator (the default is comma)
- Single-line comment start (the default is sharp)
- Quotation mark enabling to use other special characters within a value (the default is double quotes)
