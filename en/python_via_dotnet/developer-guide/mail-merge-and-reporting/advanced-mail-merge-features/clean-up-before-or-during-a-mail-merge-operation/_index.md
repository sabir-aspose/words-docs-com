---
title: Clean Up Before or During Mail Merge
second_title: Aspose.Words for Python via .NET
articleTitle: Clean Up Before or During a Mail Merge Operation
linktitle: Clean Up Before or During a Mail Merge Operation
type: docs
description: "Apply different cleaning and removing options such as deleting merge fields before performing a Mail Merge operation or removing unused regions during a Mail Merge operation using Python."
keywords: "cleanup options Mail Merge python"
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/clean-up-before-or-during-mail-merge/
timestamp: 2026-08-24-16-41-00
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page explains how to perform cleanup operations before or during a Mail Merge in Aspose.Words for Python via .NET to ensure document integrity.

{{% /alert %}}

Aspose.Words allows you to apply different cleaning and removing options such as deleting merge fields before performing a Mail Merge operation or removing unused regions during a Mail Merge operation. This section will explain how to delete merged fields and how to set up a removing option.

## Delete Merged Fields

When you are using some long template that is created by someone else, you may want to delete all the merge fields that already exist in that template before performing a Mail Merge operation. You can use the [delete_fields](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/delete_fields/) method if you want to delete all merge fields from a document without executing a Mail Merge operation. This method is not affected by any removing options of the [cleanup_options](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/cleanup_options/) property and executing it only removes merged fields, not any containing fields or empty paragraphs.

The following code example shows how to delete all merge fields from your template without executing a Mail Merge operation:

{{< gist "aspose-words-gists" "d7e717546d32e7dd25f0198a15f8ebf2" "delete-fields.py" >}}

## Set Up a `Removing` Option

Aspose.Words enables you to remove unmerged fields, regions, and paragraphs from a template during a Mail Merge operation using removing options.

Use the **cleanup_options** property along with the [MailMergeCleanupOptions](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmergecleanupoptions/) enumeration to set the removing option. Specify which items you want to remove by choosing the following options (you can combine more than one):

* Remove empty paragraphs
* Remove unused regions
* Remove unused fields
* Remove containing fields
* Remove static fields
* Remove empty table rows

You can consider a merge field as unmerged in one of the following conditions:

1. If the merge field in the data source does not have a corresponding field or a mapping field.
2. If the merge field in the data source contains a mapping field but the data is `None`.

{{% alert color="primary" %}}

If you are merging data using separate data sources then those removing options will be enabled only with the last call of Mail Merge execute method.

{{% /alert %}}

### Remove Empty Paragraphs

A paragraph that only includes merge fields will be empty when the Mail Merge process removes all its merge fields as unmerged. Those empty paragraphs can add unwanted space and change how the generated report will look. You may face two situations with paragraphs during a Mail Merge operation:

1. The Mail Merge field will be merged with empty data.
2. The merge field is unused and will be removed.

In both situations the **REMOVE_EMPTY_PARAGRAPHS** option will automatically remove empty paragraphs from the document. Also, it will remove the `TableStart` and `TableEnd` merge fields if the rest of the paragraph is empty.

The following code example shows how to remove the empty paragraphs:

{{< gist "aspose-words-gists" "d7e717546d32e7dd25f0198a15f8ebf2" "remove-empty-paragraphs.py" >}}

{{% alert color="primary" %}}

You can download the sample file of this example from [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Table%20with%20fields.docx).

{{% /alert %}}

### Remove Unused Regions

In previous versions of Aspose.Words, empty Mail Merge regions were removed from the document automatically during the Mail Merge operation. With the latest version of Aspose.words, empty Mail Merge regions remain after the Mail Merge operation by default. However, you can use the **REMOVE_UNUSED_REGIONS** option to remove the unused Mail Merge regions during the Mail Merge operation. For example, you can merge a document with an empty data source containing no records that lead to unused regions in the document.

The following code example shows how to remove the unused merge regions:

{{< gist "aspose-words-gists" "d7e717546d32e7dd25f0198a15f8ebf2" "remove-unmerged-regions.py" >}}

{{% alert color="primary" %}}

You can download the sample file of this example from [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Mail%20merge%20destination%20-%20Northwind%20suppliers.docx).

{{% /alert %}}

**Note**: This option will remove any Mail Merge region in the document which is not found in the current data source. If you are merging data from many data sources by using separate calls of [execute_with_regions](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/execute_with_regions/) then you need to make sure that this option is enabled only with the very last merge operation. Otherwise, all unused Mail Merge regions will be removed from the document before they can be merged.

### Remove Unused Fields

Aspose.Words allows you to remove any unused Mail Merge fields by assigning the **REMOVE_UNUSED_FIELDS** flag to **cleanup_options**. This option will remove merge fields that don't have the corresponding data in the data source.

The following code example shows how to remove any unused merge fields from a document automatically during a Mail Merge operation:

{{< gist "aspose-words-gists" "d7e717546d32e7dd25f0198a15f8ebf2" "remove-unused-fields.py" >}}

### Removing Containing Fields

A merge field can be contained within another field such as an **IF** field or a formula field. Remove this outer field when the merge field is merged or removed from the document.

The following code example shows how to remove fields that contain merge fields from a document:

{{< gist "aspose-words-gists" "d7e717546d32e7dd25f0198a15f8ebf2" "remove-containing-fields.py" >}}

**Note**: This option will only remove a containing field if the field was actually merged with data or if the merge field was removed by using the **REMOVE_UNUSED_FIELDS** option. This option matches the behavior of Microsoft Word during Mail Merge which always automatically removes outer fields from a merged field and keeps only the plain text result.

### Remove Empty Table Rows

Aspose.Words allows you to remove empty table rows by assigning the **REMOVE_EMPTY_TABLE_ROWS** flag to **cleanup_options**. This option will remove table rows that contain empty merge fields.

The following code example shows how to remove empty table rows that contain Mail Merge regions from a document:

{{< gist "aspose-words-gists" "d7e717546d32e7dd25f0198a15f8ebf2" "remove-empty-table-rows.py" >}}

------

## Troubleshoot

1. **Problem:** After a mail merge an empty paragraph remains above a merge field, creating unwanted space.
   **Solution:** Enable the `REMOVE_EMPTY_PARAGRAPHS` flag in `cleanup_options` before executing the merge. This removes paragraphs that become empty after fields are cleared. If the paragraph still persists, call `builder.move_to_merge_field("FieldName")` and delete the paragraph manually, or use `delete_fields` to remove the field before the merge.

2. **Problem:** Unused mail‑merge regions are still present in the generated document even though `REMOVE_UNUSED_REGIONS` was set.
   **Solution:** Ensure that `REMOVE_UNUSED_REGIONS` is applied on the **last** call to `mail_merge.execute_with_regions`. When merging data from multiple sources, set the flag only on the final merge; earlier calls will otherwise delete regions prematurely.

3. **Problem:** Cleanup options (e.g., `REMOVE_UNUSED_FIELDS`, `REMOVE_EMPTY_TABLE_ROWS`) have no effect when performing several `execute_with_regions` calls.
   **Solution:** `cleanup_options` are evaluated only after the merge operation finishes. Apply the desired flags once, after the final `execute_with_regions` call, or re‑assign `cleanup_options` before the last execution. Do not change the options between intermediate merges, as they will be ignored.
