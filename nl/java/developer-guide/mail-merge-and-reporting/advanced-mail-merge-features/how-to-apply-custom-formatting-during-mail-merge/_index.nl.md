---
title: Aangepaste opmaak toepassen tijdens Mail Merge
second_title: Aspose.Words voor Java
articleTitle: Aangepaste opmaak toepassen tijdens Mail Merge
linktitle: Aangepaste opmaak toepassen tijdens Mail Merge
type: docs
description: "Aangepaste opmaak toepassen tijdens een bewerking van Mail Merge met behulp van Java."
weight: 60
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /nl/java/how-to-apply-custom-formatting-during-mail-merge/
timestamp: 2024-01-27-14-07-04
---

De [MailMerge](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/) klasse biedt twee gebeurtenissen die zeer nuttig kunnen zijn bij het uitbreiden van Mail Merge mogelijkheden. De eigenschap [setFieldMergingCallback(IFieldMergingCallback)](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#FieldMergingCallback) accepteert een klasse die de methoden [fieldMerging(FieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#fieldMerging-com.aspose.words.FieldMergingArgs) en [imageFieldMerging(ImageFieldMergingArgs)](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/#imageFieldMerging-com.aspose.words.ImageFieldMergingArgs) implementeert. Deze kunnen worden gebruikt om aangepaste controle over het Mail Merge proces te implementeren.

De gebeurtenis **fieldMerging(FieldMergingArgs)** vindt plaats tijdens Mail Merge Wanneer een eenvoudig Mail Merge veld wordt aangetroffen in het document. Dit geeft meer controle over de Mail Merge en u kunt alle acties uitvoeren wanneer de gebeurtenis plaatsvindt. Deze methode is verpakt in een klasse die de [IFieldMergingCallBack](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/) interface implementeert en een [FieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/fieldmergingargs/) object accepteert dat gegevens levert voor de overeenkomstige gebeurtenis.

Het onderstaande codevoorbeeld laat zien hoe u aangepaste logica implementeert in de gebeurtenis `MergeField` om celopmaak toe te passen.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomFormattingDuringMailMerge-ApplyCustomFormattingDuringMailMerge.java" >}}
