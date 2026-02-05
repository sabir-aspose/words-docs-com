---
title: Split Table in Node.js
second_title: Aspose.Words for Node.js
articleTitle: Split Table
linktitle: Split Table
description: "Split table in Node.js. How to split one table into two separate tables Python."
type: docs
weight: 100
ai_search_scope: words_nodejs
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /nodejs-net/split-table/
timestamp: 2025-07-09-10-05-05
---

A table, represented in the Aspose.Words Document Object Model, is made up of independent rows and cells, making it easy to split a table.

To manipulate a table to split it into two tables, we just need to move some of the rows from the original table to the new one. To do this, we need to pick the row by which we want to split the table.

We can create two tables from the original table by following these simple steps:

1. Create a clone of the table without cloning the children to keep the moved rows and insert them after the original table
2. Starting at the specified row, move all subsequent rows to this second table

The following code example shows how to split a table into two tables on a specific row:

{{< gist "aspose-words-gists" "b8cd11852d8ab0968ecdda0e2baeda15" "split-table.js" >}}

------ 

## FAQ

1. **Q:** How do I split a table at a particular row using Aspose.Words for Node.js?  
   **A:** Create a clone of the original table without its child nodes (`table.clone(false)`), insert the clone after the original, then move all rows starting from the split row to the cloned table using `table.appendChild(row)`.

2. **Q:** Do I need to clone the table with its rows when splitting?  
   **A:** No. Clone the table without its children (`clone(false)`) so the new table starts empty; the rows you move will populate it, preserving the original formatting.

3. **Q:** Will the formatting of the moved rows be retained after the split?  
   **A:** Yes. Row and cell formatting are stored with each row, so moving rows to the new table keeps their appearance unchanged.

4. **Q:** Can I split a table into more than two tables?  
   **A:** Yes. Perform the same process repeatedly: clone the original (or a previously split) table, insert the clone, and move the desired range of rows to each new table.

5. **Q:** Is there a way to split a table without using the `clone` method?  
   **A:** While you could create a new `Table` instance manually and copy required properties, using `clone(false)` is the simplest and safest approach because it copies all table settings automatically.