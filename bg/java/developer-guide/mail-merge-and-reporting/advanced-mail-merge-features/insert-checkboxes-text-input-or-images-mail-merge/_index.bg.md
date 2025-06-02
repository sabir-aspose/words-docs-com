---
title: Вмъкване на CheckboxЕС, въвеждане на текст или изображения по време на Mail Merge
second_title: Aspose.Words за Java
articleTitle: Вмъкване CheckboxЕС, въвеждане на текст или изображения
linktitle: Вмъкване CheckboxЕС, въвеждане на текст или изображения
description: "Въведете checkboxЕС или полетата за въвеждане на текст по време на Mail Merge използване на Java. Също така вмъквайте изображения от База данни по време на Mail Merge в Java."
type: docs
weight: 20
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /bg/java/insert-checkboxes-text-input-or-images-mail-merge/
timestamp: 2024-01-27-14-07-04
---

Обединяващият двигател взема документ като вход, търси `MERGEFIELD` полета в него и ги замества с данните, получени от източника на данни. Обикновено се вмъкват обикновен текст и HTML, но Aspose.Words потребителите могат също да генерират документ, който обработва по-необичайни сценарии за Mail Merge полета.

Мощната Aspose.Words функционалност ви позволява да разширите процеса Mail Merge:

- въведете полетата checkboxи текстова форма за въвеждане в документа по време на А mail merge
- вмъкване на изображения от всяко персонализирано хранилище (файлове, BLOB полета и т.н.)

## Въведете CheckboxЕС и текст по време на Mail Merge

Понякога е необходимо да се извърши операция Mail Merge, така че в полето за обединяване да не се замества текст, а поле checkbox или въвеждане на текст. Въпреки че това не е най-често срещаният сценарий, той е много удобен за някои задачи.

Следващата екранна снимка на документ Word показва шаблон с полета за обединяване:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-1](insert-checkboxes-html-or-images-during-mail-merge_1.jpeg)

Тази екранна снимка на документа Word по-долу показва вече генерирания документ:

![insert-checkboxes-html-or-images-during-mail-merge-aspose-words-java-2](insert-checkboxes-html-or-images-during-mail-merge-2.png)

{{% alert color="primary" %}}

Обърнете внимание, че някои полета са заменени с обикновен текст, някои полета са заменени с полета на формуляр checkbox, а полето `Subject` е заменено с поле за въвеждане на текст.

{{% /alert %}}

Следващият пример за код показва как да вмъквате checkboxЕС и полета за въвеждане на текст в документ по време на mail merge:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-MailMergeFormFields.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeFormFields-HandleMergeField.java" >}}

## Вмъкване на изображения по време на Mail Merge

Когато извършвате операция Mail Merge, можете да вмъкнете изображения от базата данни в документа, като използвате специални полета за изображение Mail Merge. Полето изображение Mail Merge е поле за сливане, наречено изображение: MyFieldName.

### Вмъкване на изображения от База данни

По време на mail merge, Когато поле за изображение Mail Merge се срещне в документ, събитието [FieldMergingCallback](https://reference.aspose.com/words/java/com.aspose.words/mailmerge/#getFieldMergingCallback) се задейства. Можете да отговорите на това събитие, за да върнете име на файл, поток или обект на изображение на двигателя Mail Merge, така че да може да бъде вмъкнат в документа.

Следващият пример за код показва как да вмъкнете изображения, съхранени в поле на база данни BLOB, в отчет:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageFromBlob.java" >}}

### Задаване на свойства на изображението по време на Mail Merge

Докато обединявате поле за обединяване на изображение, понякога може да се наложи да контролирате различни свойства на изображението, като [WrapType](https://reference.aspose.com/words/java/com.aspose.words/wraptype/).

В момента, използвайки [ImageFieldMergingArgs](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/), можете да зададете съответно само свойства за ширина или височина на изображението. За да се преодолее този проблем, Aspose.Words осигурява [Shape](https://reference.aspose.com/words/java/com.aspose.words/imagefieldmergingargs/#getShape) свойство, което улеснява получаването на пълен контрол върху вмъкнатото изображение или всяка друга форма.

Следният пример за код показва как да зададете различни свойства на изображението:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-MailMergeImageField.java" >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-MailMergeImageField-FieldMergingHandler.java" >}}

