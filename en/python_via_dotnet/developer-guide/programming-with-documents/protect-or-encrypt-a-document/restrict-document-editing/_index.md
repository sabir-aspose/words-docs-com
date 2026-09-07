---
title: Restrict Document Editing in Python
second_title: Aspose.Words for Python via .NET
articleTitle: Restrict Document Editing
linktitle: Restrict Document Editing
description: "Restrict editing a document by setting a restriction type using Python. You can also remove protection and make unrestricted editable regions."
type: docs
weight: 30
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/restrict-document-editing/
aliases: [/python/restrict-document-editing/]
timestamp: 2026-02-03-11-08-55
---

{{% alert color="grey" %}}
*Purpose Summary. What is this page about?*

This page shows how to use Aspose.Words for Python via .NET to apply editing restrictions, add or remove document protection, and define unrestricted editable regions in a Word document.
{{% /alert %}}

Sometimes you may need to limit the ability to edit a document and only allow certain actions with it. This can be useful to prevent other people from editing sensitive and confidential information in your document.

Aspose.Words allows you to restrict editing a document by setting a restriction type. In addition, Aspose.Words also enables you to specify write protection settings for a document.

This article explains how to use Aspose.Words to select a restriction type, how to add or remove protection, and how to make unrestricted editable regions.

## Select Editing Restriction Type

Aspose.Words allows you to control the way you restrict the content using the [ProtectionType](https://reference.aspose.com/words/python-net/aspose.words/protectiontype/) enumeration parameter. This will enable you to select an exact type of protection such as the following:

* AllowOnlyComments
* AllowOnlyFormFields
* AllowOnlyRevisions
* ReadOnly
* NoProtection

All types are password-secured, and if this password is not entered correctly, a user will not be able to legally change the content of your document. Thus, if your document is returned to you without a requirement to provide the necessary password, this is a sign that something is wrong.

If you did not set a password when choosing the security type, other users can simply ignore the protection of your document.

{{% alert color="primary" %}}

Note that the password being set is just a property in a document that can be removed if the document properties are accessed. Accordingly, such a password is not a guarantee of the document security. The [Document.unprotect](https://reference.aspose.com/words/python-net/aspose.words/document/unprotect/) method shows just that.

{{% /alert %}}

## Add Document Protection

Adding protection to your document is a simple process, as all you need to do is apply one of the protection methods detailed in this section.

Aspose.Words allows you to protect your documents from changes using the [Document.protect](https://reference.aspose.com/words/python-net/aspose.words/document/protect/) method. This method is not a security feature and does not encrypt a document.

{{% alert color="primary" %}}

In Microsoft Word, you can restrict editing in a similar way using both:

* Restrict Editing (File → Info → Protect Document)
* Alternative feature – “Restrict Editing” (Review → Protect → Restrict Editing)

{{% /alert %}}

The following code example shows how to add password protection to your document:

{{< gist "aspose-words-gists" "7bc1619f98f7517ddcbf0b38a3b68989" "password-protection.py" >}}

The following code example shows how to restrict editing in a document so only editing in form fields is possible:

{{< gist "aspose-words-gists" "7bc1619f98f7517ddcbf0b38a3b68989" "allow-only-form-fields-protect.py" >}}

## Remove Document Protection

Aspose.Words allows you to remove protection from a document with simple and direct document modification. You can either remove the document protection without knowing the actual password or provide the correct password to unlock the document by using the [unprotect](https://reference.aspose.com/words/python-net/aspose.words/document/unprotect/) method. Both removing ways have no difference.

The following code example shows how to remove protection from your document:

{{< gist "aspose-words-gists" "7bc1619f98f7517ddcbf0b38a3b68989" "remove-document-protection.py" >}}

## Specify Unrestricted Editable Regions

You can restrict editing of your document and at the same time allow changes to selected parts of it. So, anyone who opens your document will be able to access these unrestricted parts and make changes to the content.

Aspose.Words allows you to mark the parts that can be changed in your document using the [start_editable_range](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/start_editable_range/) and [end_editable_range](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/end_editable_range/) methods.

The following code example shows how to mark the whole document as read-only and specify editable regions in it:

{{< gist "aspose-words-gists" "7bc1619f98f7517ddcbf0b38a3b68989" "unrestricted-editable-regions.py" >}}

You can also choose different document editing restrictions for different sections.

The following code example shows how to add a restriction for the entire document, and then remove the restriction for one of the sections:

{{< gist "aspose-words-gists" "7bc1619f98f7517ddcbf0b38a3b68989" "unrestricted-section.py" >}}

## Limitations and Considerations

- Aspose.Words protection is not encryption — it stores only a password hash in the document properties and does not secure the document content.
- Protection does not prevent programmatic access or modification — any Aspose.Words application can remove protection or modify the document regardless of restrictions.
- The `document.protect(...)` method only sets a metadata flag; it does not prevent changes via API calls such as `document.unprotect()` or `document_builder.start_editable_range()`.
- Editable ranges do not override section‑level protection settings — they apply only to the document‑level protection state and require correct section break types to function as expected.

## Related APIs

- [ProtectionType](https://reference.aspose.com/words/python-net/aspose.words/protectiontype/)
- [Document.protect(ProtectionType, str)](https://reference.aspose.com/words/python-net/aspose.words/document/protect/)
- [Document.unprotect()](https://reference.aspose.com/words/python-net/aspose.words/document/unprotect/)
- [DocumentBuilder.start_editable_range()](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/start_editable_range/)
- [DocumentBuilder.end_editable_range()](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/end_editable_range/)
