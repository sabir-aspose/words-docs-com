---
title: Wstaw Checkboxes, wprowadzanie tekstu lub obrazy podczas Mail Merge
second_title: Aspose.Words dla Java
articleTitle: Wstaw Checkboxes, wprowadzanie tekstu lub obrazy
linktitle: Wstaw Checkboxes, wprowadzanie tekstu lub obrazy
description: "Wstaw checkboxes lub pola wprowadzania tekstu podczas Mail Merge przy użyciu Java. Wstaw także obrazy z bazy danych podczas Mail Merge w Java."
type: docs
weight: 20
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pl/java/insert-checkboxes-text-input-or-images-mail-merge/
timestamp: 2024-01-27-14-07-04
---

Silnik scalania przyjmuje dokument jako dane wejściowe, szuka w nim pól `MERGEFIELD` i zastępuje je danymi uzyskanymi ze źródła danych. Zazwyczaj wstawiany jest zwykły tekst i HTML, ale użytkownicy Aspose.Words mogą również wygenerować dokument, który obsługuje bardziej nietypowe scenariusze dla pól Mail Merge.

Potężna funkcjonalność Aspose.Words pozwala rozszerzyć proces Mail Merge:

- Wstaw checkboxpola formularza es i wprowadzania tekstu do dokumentu podczas mail merge
- Wstaw obrazy z dowolnego niestandardowego magazynu (pliki, pola BLOB itp.)

## Insert Checkboxes i wprowadzanie tekstu podczas Mail Merge

Czasami konieczne jest wykonanie operacji Mail Merge, aby w polu scalania nie podstawiono tekstu, ale checkbox lub pole wprowadzania tekstu. Chociaż nie jest to najczęstszy scenariusz, jest bardzo przydatny w przypadku niektórych zadań.

Poniższy zrzut ekranu dokumentu Word pokazuje szablon z polami scalania:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-1](insert-checkboxes-html-or-images-during-mail-merge_1.jpeg)

Ten zrzut ekranu dokumentu Word poniżej pokazuje już wygenerowany dokument:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-2](insert-checkboxes-html-or-images-during-mail-merge-2.png)

{{% alert color="primary" %}}

Zwróć uwagę, że niektóre pola zostały zastąpione zwykłym tekstem, niektóre pola zostały zastąpione polami formularza checkbox, A pole `Subject` zostało zastąpione polem wprowadzania tekstu.

{{% /alert %}}

Poniższy przykład kodu pokazuje, jak wstawić checkboxes i wprowadzić pola tekstowe do dokumentu podczas mail merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-MailMergeFormFields.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-HandleMergeField.java" >}}

## Wstawianie obrazów podczas Mail Merge

Podczas wykonywania operacji Mail Merge można wstawiać obrazy z bazy danych do dokumentu za pomocą specjalnych pól image Mail Merge. Pole image Mail Merge jest polem scalania o nazwie Image: MyFieldName.

### Wstawianie obrazów z bazy danych

Podczas mail merge, gdy napotkane jest pole obraz Mail Merge w dokumencie, Zdarzenie [FieldMergingCallback](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#getFieldMergingCallback) jest uruchamiane. Możesz odpowiedzieć na to zdarzenie, aby zwrócić nazwę pliku, strumień lub obiekt obrazu do silnika Mail Merge, aby można go było wstawić do dokumentu.

Poniższy przykład kodu pokazuje, jak wstawić obrazy zapisane w bazie danych BLOB pole do raportu:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageFromBlob.java" >}}

### Ustaw właściwości obrazu podczas Mail Merge

Podczas scalania pola scalania obrazu czasami może być konieczne kontrolowanie różnych właściwości obrazu, takich jak [WrapType](https://reference.aspose.com/words/java/com.aspose.words/wraptype/).

Obecnie za pomocą [ImageFieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/) można ustawić tylko odpowiednio właściwości szerokości lub wysokości obrazu. Aby rozwiązać ten problem, Aspose.Words udostępnia Właściwość [Shape](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/#getShape), która ułatwia uzyskanie pełnej kontroli nad wstawionym obrazem lub dowolnym innym kształtem.

Poniższy przykład kodu pokazuje, jak ustawić różne właściwości obrazu:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-MailMergeImageField.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-FieldMergingHandler.java" >}}

