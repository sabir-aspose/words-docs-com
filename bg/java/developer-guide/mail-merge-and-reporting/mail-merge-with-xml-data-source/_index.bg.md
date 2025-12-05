---
title: Mail Merge с XML източник на данни в Java
second_title: Aspose.Words за Java
articleTitle: Mail Merge с XML източник на данни
linktitle: Mail Merge с XML източник на данни
type: docs
description: "Използвайте различни източници на данни, когато извършвате операция Mail Merge, включително файл XML. Основното предимство на използването на XML е възможността да се определи йерархия директно в документа в Java."
keywords: "mail merge XML data source Java, Mail Merge Java"
weight: 30
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/java/mail-merge-with-xml-data-source/
timestamp: 2024-01-27-14-07-04
---

Можете да използвате различни източници на данни, когато извършвате операция Mail Merge, включително файл XML. Основното предимство на използването на XML е възможността да се определи йерархия в документа и след това просто да се подаде до Aspose.Words.

Тази статия ще опише как да се четат данни от файл XML, а не директно от база данни и включва XML като източник на данни за извършване на операция Mail Merge.

## Предимства на XML като източник на данни

XML източници на данни са много удобни за съхранение на данни без режийни на база данни. Те са чудесни за офлайн приложения, където потребителите трябва да добавят, редактират и изтриват данни, когато не могат да се свържат с база данни.

XML данните могат да бъдат добър източник на данни алтернатива на релационни бази данни, особено ако работите с уеб приложения. Повечето уеб услуги използват XML за обмен на информация. XML - ориентираните бази данни се използват активно на текущия пазар, а разработчиците на релационни бази данни добавят XML Съвместимост към своите продукти, за да имат връщане на базата данни XML.

Тъй като XML съхранява данни в обикновен текстов формат, съхранението е независимо от платформата. По този начин данните могат лесно да бъдат експортирани, импортирани или просто преместени. XML е популярен като източник на данни, защото предлага начин за запазване на семантичното значение на данните при комуникация между различни приложения.

## Попълване на шаблон за обединяване с данни от XML Използване на DataSet

XML е универсалният стандарт за обмен на данни, а Microsoft Word форматите на документи са най-популярните формати за Mail Merge шаблони. Следователно, възможността за стартиране на Mail Merge от XML Файл на Word шаблон документ се превърна в общо изискване.

Microsoft Word не предоставя директен метод за работа с XML данни като източник на данни за Mail Merge операция, докато Aspose.Words ви позволява да извършите Mail Merge операция с данни от XML източник на данни. Имайте предвид, че структурата на документа XML също може да се променя и данните все още ще бъдат прочетени правилно. Това позволява лесно Обединяване на различни видове XML документи.

Използвайте метода `ReadXML`, За да прочетете схемата XML и данните в обекта `DataSet`. След това този обект се използва като източник на данни за mail merge.

{{% alert color="primary" %}}

Можете да използвате едни и същи шаблони за различни източници на данни.

{{% /alert %}}

Следното XML съдържа данните, които са необходими за попълване на шаблон за обединяване:

{{< highlight xml >}}
<?xml version="1.0" encoding="utf-8"?>
<customers>
	 <customer Name="John Ben Jan" ID="1" Domain="History" City="Boston"/>
 	<customer Name="Lisa Lane" ID="2" Domain="Chemistry" City="LA"/>
	 <customer Name="Dagomir Zits" ID="3" Domain="Heraldry" City="Milwaukee"/>
 	<customer Name="Sara Careira Santy" ID="4" Domain="IT" City="Miami"/>
</customers> 
{{< /highlight >}}

Следващият пример за код показва как да заредите XML данни в DataSet и след това да ги използвате като източник на данни:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-XMLMailMerge-XMLMailMerge.java" >}}

{{% alert color="primary" %}}

Можете да изтеглите примерния файл на този пример от [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20data%20-%20Customers.xml).

{{% /alert %}}

Можете да забележите разликата между шаблона, преди да изпълните операцията Mail Merge:

<img src="fill-merge-template-from-xml-using-dataset-1.png" alt="fill_merge_template_from_xml_using_dataset_aspose_words_java" style="width:250px"/>

И след извършване на операцията Mail Merge:

<img src="fill-merge-template-from-xml-using-dataset-2.png" alt="fill_merge_template_from_xml_aspose_words_java" style="width:285px"/>
