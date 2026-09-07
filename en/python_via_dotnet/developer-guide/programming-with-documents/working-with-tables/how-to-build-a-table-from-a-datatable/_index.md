---
title: How to Build a Table from XML Data in Python
second_title: Aspose.Words for Python via .NET
articleTitle: Build a Table from XML Data
linktitle: Build a Table from XML Data
description: "Example of filling a document table from an external XML data source using Python."
type: docs
weight: 120
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/how-to-build-a-table-from-a-datatable/
timestamp: 2026-08-20-11-50-55
---

{{% alert color="grey" %}}

## Purpose Summary

This page explains how to build a table from XML data using Aspose.Words.

{{% /alert %}}

Often your application will pull data from a database or an XML file and store it in the form of rows and columns. You can easily insert this data into your document as a new table and quickly apply formatting to the whole table.

Using Aspose.Words, you can easily retrieve data from a data source and store it as a table:

1. Create a new **DocumentBuilder** object on your **Document**.
1. Start a new table using **DocumentBuilder**.
1. If we want to insert the names of each of the columns from our data source as a header row then iterate through each column name and write it into a row in the table.
1. Iterate through each data row:
   1. Iterate through each item in the row.
   1. Insert the item into the document using **DocumentBuilder**. The method used depends on the type of the item being inserted e.g **DocumentBuilder.writeln** for text and **DocumentBuilder.insert_image** for a byte array which represents an image.
   1. At the end of processing of the row also end the row being created by the **DocumentBuilder** by using **DocumentBuilder.end_row**.
1. Once all rows from the data source have been processed finish the table by calling **DocumentBuilder.end_table**.
1. Finally we can set the desired table style using one of the appropriate table properties such as **Table.style_identifier** to automatically apply formatting to the entire table.

Python has no `DataTable` equivalent, so the `read_xml_table` method uses the standard library to read an XML file into a list of column names and a list of row values.

The **import_table_from_data** method accepts a **DocumentBuilder** object, the column names and rows containing the data, and a flag which specifies if the column headings are included at the top of the table. This method builds a table from these parameters using the builder's current position and formatting.

The following code example shows how to execute the above algorithm in Aspose.Words:

{{< gist "aspose-words-gists" "06721a97657981cdb27970a352300119" "import-table-from-data-table.py" >}}

The method can then be easily called using your **DocumentBuilder** and data.

The following code example shows how to import the data and insert it into a new table in the document:

{{< gist "aspose-words-gists" "06721a97657981cdb27970a352300119" "build-table-from-data-table.py" >}}
