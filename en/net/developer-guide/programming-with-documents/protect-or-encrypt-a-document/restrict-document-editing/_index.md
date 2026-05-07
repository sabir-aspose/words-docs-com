---
title: Restrict Document Editing in C#
second_title: Aspose.Words for .NET
articleTitle: Restrict Document Editing
linktitle: Restrict Document Editing
description: "Restrict editing a document by setting a restriction type using C#. You can also remove protection and make unrestricted editable regions."
type: docs
weight: 30
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/restrict-document-editing/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

## Purpose Summary

This page explains how to restrict editing of a document or selected parts.

{{% /alert %}}

Sometimes you may need to limit the ability to edit a document and only allow certain actions with it. This can be useful to prevent other people from editing sensitive and confidential information in your document.

Aspose.Words allows you to restrict editing a document by setting a restriction type. In addition, Aspose.Words also enables you to specify write protection settings for a document.

This article explains how to use Aspose.Words to select a restriction type, how to add or remove protection, and how to make unrestricted editable regions.

## Select Editing Restriction Type

Aspose.Words allows you to control the way you restrict the content using the [ProtectionType](https://reference.aspose.com/words/net/aspose.words/protectiontype/) enumeration parameter. This will enable you to select an exact type of protection such as the following:

* AllowOnlyComments
* AllowOnlyFormFields
* AllowOnlyRevisions
* ReadOnly
* NoProtection

All types are password‑secured, and if this password is not entered correctly, a user will not be able to legally change the content of your document. Thus, if your document is returned to you without a requirement to provide the necessary password, this is a sign that something is wrong.

If you did not set a password when choosing the security type, other users can simply ignore the protection of your document.

{{% alert color="primary" %}}

Note that the password being set is just a property in a document that can be removed if the document properties are accessed. Accordingly, such a password is not a guarantee of the document security. The [Unprotect](https://reference.aspose.com/words/net/aspose.words/document/unprotect/#unprotect/) method shows just that.

{{% /alert %}}

## Add Document Protection

Adding protection to your document is a simple process, as all you need to do is apply one of the protection methods detailed in this section.

Aspose.Words allows you to protect your documents from changes using the [Protect](https://reference.aspose.com/words/net/aspose.words/document/protect/#protect/) method. This method is not a security feature and does not encrypt a document.

{{% alert color="primary" %}}

In Microsoft Word, you can restrict editing in a similar way using both:

* Restrict Editing (File → Info → Protect Document)
* Alternative feature – “Restrict Editing” (Review → Protect → Restrict Editing)

{{% /alert %}}

The following code example shows how to add password protection to your document:

{{< gist "aspose-words-gists" "856ba85fa704fa728b0ec20aafddd16b" "password-protection.cs" >}}

The following code example shows how to restrict editing in a document so only editing in form fields is possible:

{{< gist "aspose-words-gists" "856ba85fa704fa728b0ec20aafddd16b" "allow-only-form-fields-protect.cs" >}}

## Remove Document Protection

Aspose.Words allows you to remove protection from a document with simple and direct document modification. You can either remove the document protection without knowing the actual password or provide the correct password to unlock the document by using the [Unprotect](https://reference.aspose.com/words/net/aspose.words/document/unprotect/#unprotect/) method. Both removing ways have no difference.

The following code example shows how to remove protection from your document:

{{< gist "aspose-words-gists" "856ba85fa704fa728b0ec20aafddd16b" "remove-document-protection.cs" >}}

## Specify Unrestricted Editable Regions

You can restrict editing of your document and at the same time allow changes to selected parts of it. So, anyone who opens your document will be able to access these unrestricted parts and make changes to the content.

Aspose.Words allows you to mark the parts that can be changed in your document using the [StartEditableRange](https://reference.aspose.com/words/net/aspose.words/documentbuilder/starteditablerange/) and [EndEditableRange](https://reference.aspose.com/words/net/aspose.words/documentbuilder/endeditablerange/#endeditablerange/) methods.

The following code example shows how to mark the whole document as read‑only and specify editable regions in it:

{{< gist "aspose-words-gists" "856ba85fa704fa728b0ec20aafddd16b" "unrestricted-editable-regions.cs" >}}

You can also choose different document editing restrictions for different sections.

The following code example shows how to add a restriction for the entire document, and then remove the restriction for one of the sections:

{{< gist "aspose-words-gists" "856ba85fa704fa728b0ec20aafddd16b" "unrestricted-section.cs" >}}

## Limitations and Considerations

## Related APIs


- [ProtectionType](https://reference.aspose.com/words/net/aspose.words/protectiontype/)
- [Document.Protect(ProtectionType, string)](https://reference.aspose.com/words/net/aspose.words/document/protect/#protect/)
- [Document.Unprotect()](https://reference.aspose.com/words/net/aspose.words/document/unprotect/#unprotect/)
- [DocumentBuilder.StartEditableRange()](https://reference.aspose.com/words/net/aspose.words/documentbuilder/starteditablerange/)
- [DocumentBuilder.EndEditableRange()](https://reference.aspose.com/words/net/aspose.words/documentbuilder/endeditablerange/#endeditablerange/)

## FAQ

1. **Q:** How do I apply password protection to a document?  
   **A:** Use the `Document.Protect` method, passing the desired `ProtectionType` and a password string. The password is stored in the document properties and is required to modify the protected content.

2. **Q:** Can I remove protection without knowing the password?  
   **A:** Yes. Calling `Document.Unprotect()` without a password removes protection regardless of the original password. If you provide the correct password, the document is unlocked in the same way.

3. **Q:** Which editing restriction types are available and what do they allow?  
   **A:** The `ProtectionType` enumeration includes `AllowOnlyComments`, `AllowOnlyFormFields`, `AllowOnlyRevisions`, `ReadOnly`, and `NoProtection`. Each type limits user actions accordingly—for example, `AllowOnlyFormFields` permits changes only in form fields.

4. **Q:** How can I allow users to edit only specific parts of a protected document?  
   **A:** Use `DocumentBuilder.StartEditableRange` and `DocumentBuilder.EndEditableRange` to define unrestricted editable regions within a read‑only document. Content inside these ranges can be edited even when the rest of the document is protected.

5. **Q:** Are Aspose.Words licenses retro‑compatible with older library versions?  
   **A:** Yes. An Aspose.Words license file works with earlier versions of the library, provided the license file format has not changed. However, it is recommended to use a license that matches the major version of the library for full feature support.