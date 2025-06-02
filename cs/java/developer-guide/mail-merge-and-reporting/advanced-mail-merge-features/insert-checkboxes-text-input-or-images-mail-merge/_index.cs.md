---
title: Vložení Checkboxes, zadávání textu nebo obrázků během Mail Merge
second_title: Aspose.Words pro Java
articleTitle: Vložení Checkboxes, zadávání textu nebo obrázků
linktitle: Vložení Checkboxes, zadávání textu nebo obrázků
description: "Vložte checkboxES nebo pole pro zadávání textu během Mail Merge pomocí Java. Také vložte obrázky z databáze během Mail Merge v Java."
type: docs
weight: 20
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/java/insert-checkboxes-text-input-or-images-mail-merge/
timestamp: 2024-01-27-14-07-04
---

Slučovací modul vezme dokument jako vstup, vyhledá v něm pole `MERGEFIELD` a nahradí je daty získanými ze zdroje dat. Obvykle se vkládají prostý text a HTML, ale Uživatelé Aspose.Words mohou také vygenerovat dokument, který zpracovává neobvyklejší scénáře pro pole Mail Merge.

Výkonná funkce Aspose.Words umožňuje rozšířit proces Mail Merge:

- vložit checkboxES a pole formuláře pro zadávání textu do dokumentu během mail merge
- vkládejte obrázky z libovolného vlastního úložiště(soubory, pole BLOB atd.)

## Vložte Checkboxes a zadávání textu během Mail Merge

Někdy je nutné provést operaci Mail Merge, aby v poli sloučení nebyl nahrazen text, ale checkbox nebo pole pro zadávání textu. I když to není nejběžnější scénář, je to velmi užitečné pro některé úkoly.

Následující snímek obrazovky dokumentu Word zobrazuje šablonu se sloučenými poli:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-1](insert-checkboxes-html-or-images-during-mail-merge_1.jpeg)

Tento snímek obrazovky níže uvedeného dokumentu Word ukazuje již vygenerovaný dokument:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-2](insert-checkboxes-html-or-images-during-mail-merge-2.png)

{{% alert color="primary" %}}

Všimněte si, že některá pole byla nahrazena prostým textem, některá pole byla nahrazena poli formuláře checkbox a pole `Subject` bylo nahrazeno polem pro zadávání textu.

{{% /alert %}}

Následující příklad kódu ukazuje, jak vložit checkboxes a zadat textová pole do dokumentu během mail merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-MailMergeFormFields.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-HandleMergeField.java" >}}

## Vkládání obrázků během Mail Merge

Při provádění operace Mail Merge můžete do dokumentu vložit obrázky z databáze pomocí speciálních polí image Mail Merge. Pole image Mail Merge je sloučené pole s názvem Image:MyFieldName.

### Vkládání obrázků z databáze

Během mail merge, když se v dokumentu objeví pole image Mail Merge, je vyvolána událost [FieldMergingCallback](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#getFieldMergingCallback). Na tuto událost můžete odpovědět a vrátit název souboru, stream nebo obrazový objekt do motoru Mail Merge, aby jej bylo možné vložit do dokumentu.

Následující příklad kódu ukazuje, jak vložit obrázky uložené v poli databáze BLOB do sestavy:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageFromBlob.java" >}}

### Nastavení vlastností obrazu během Mail Merge

Při slučování pole pro sloučení obrázků může být někdy nutné ovládat různé vlastnosti obrázku, například [WrapType](https://reference.aspose.com/words/java/com.aspose.words/wraptype/).

V současné době můžete pomocí [ImageFieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/) nastavit pouze vlastnosti šířky nebo výšky obrázku. K překonání tohoto problému poskytuje Aspose.Words Vlastnost [Shape](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/#getShape), která usnadňuje získání plné kontroly nad vloženým obrázkem nebo jakýmkoli jiným tvarem.

Následující příklad kódu ukazuje, jak nastavit různé vlastnosti obrázku:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-MailMergeImageField.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-FieldMergingHandler.java" >}}

