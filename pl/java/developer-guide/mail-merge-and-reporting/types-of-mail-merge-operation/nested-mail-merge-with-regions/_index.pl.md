---
title: Zagnieżdżone Mail Merge z regionami w Java
second_title: Aspose.Words dla Java
articleTitle: Zagnieżdżone Mail Merge z regionami
linktitle: Zagnieżdżone Mail Merge z regionami
type: docs
description: "Wykonaj operację Mail Merge z zagnieżdżonymi regionami. Zagnieżdżone scalanie to funkcja, która umożliwia scalanie danych hierarchicznych ze źródła danych do szablonu scalania za pomocą Java."
keywords: "mail merge with nested regions Java, Nested Mail Merge Regions"
weight: 10
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pl/java/nested-mail-merge-with-regions/
timestamp: 2024-01-27-14-07-04
---

W niektórych scenariuszach może być konieczne użycie zagnieżdżonego Mail Merge z regionami. Zagnieżdżone scalanie to funkcja, która umożliwia scalanie danych hierarchicznych ze źródła danych do szablonu scalania w celu łatwego zapełnienia dokumentu. Zasadniczo dane hierarchiczne są reprezentowane jako zestaw elementów danych, a relacje hierarchiczne opisują, w jaki sposób elementy danych są ze sobą powiązane (jeden element danych jest rodzicem innego).

Aspose.Words umożliwia wykonanie operacji Mail Merge z zagnieżdżonymi regionami. Możesz użyć tej funkcji, jeśli masz źródło danych zorganizowane w strukturę podobną do drzewa i chcesz wykonać operację Mail Merge, aby wypełnić szablon danymi hierarchicznymi.

{{% alert color="primary" %}}

Zagnieżdżone Mail Merge jest istotne tylko podczas wykonywania Mail Merge z regionami.

{{% /alert %}}

## Co to jest zagnieżdżone Mail Merge

Region Mail Merge jest nazywany zagnieżdżonym, jeśli masz dwa lub więcej regionów Mail Merge, w których jeden z nich znajduje się wewnątrz drugiego w formie hierarchicznej. Zauważ, że Każdy region zawiera dane z jednej tabeli.

Najczęstszym przykładem zagnieżdżonego Mail Merge jest kolejność zawierająca wiele elementów, w których należy połączyć wiele tabel danych i przedstawić informacje w szablonie.

Poniższy rysunek pokazuje dwa zagnieżdżone regiony, w których region *Order* Mail Merge jest rodzicem regionu *Item* Mail Merge.

<img src="nested-mail-merge-with-regions-1.png" alt="nested_mail_merge_with_regions_aspose_words_java" style="width:650px"/>

## Jak przetwarzać Mail Merge z zagnieżdżonymi regionami

Dane do scalenia w szablon mogą pochodzić z różnych źródeł, głównie relacyjnych baz danych lub dokumentów XML. W naszym przykładzie użyjemy pliku XML do przechowywania naszych danych i załadowania ich bezpośrednio do **DataSet**.

Aspose.Words umożliwia przetwarzanie Mail Merge z zagnieżdżonymi regionami przy użyciu relacji danych określonych w **DataSet**. Kiedy obiekt **DataSet** ładuje XML, albo używa dostarczonego schematu, albo wnioskuje go ze struktury samego XML, aby to osiągnąć. Z tej struktury tworzy relacje między tabelami w razie potrzeby.

Poniższy obrazek pokazuje, w jaki sposób dane z tabeli *Order* przekazane do zagnieżdżonych regionów scalania zostaną połączone z Tabelą *Item*, a także dane wyjściowe wygenerowane podczas operacji scalania.

<img src="nested-mail-merge-with-regions-2.png" alt="mail_merge_with_nested_regions_aspose_words_java" style="width:650px"/>

Jak widać z dokumentu wyjściowego, każde zamówienie z tabeli **Order** jest wstawiane do szablonu scalania ze wszystkimi powiązanymi elementami zamówienia z tabeli **Item**. Następne zamówienie zostanie wstawione wraz z ich pozycjami, aż wszystkie zamówienia i pozycje zostaną wyświetlone. Kolejność zagnieżdżania Mail Merge z regionami w szablonie musi być zgodna z relacjami danych między tabelami w źródle danych.

Poniższy przykład kodu pokazuje, jak wygenerować fakturę za pomocą zagnieżdżonego Mail Merge z regionami:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e"  "Examples-src-main-java-com-aspose-words-examples-mail_merge-TypesofMailMergeOperations-NestedMailMerge.java" >}}

{{% alert color="primary" %}}

Możesz pobrać przykładowy plik tego przykładu z [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20data%20-%20Customers.xml).

{{% /alert %}}

## Jak skonfigurować relacje danych w zagnieżdżonym Mail Merge z regionami

Musisz skonfigurować wszystkie relacje danych w strukturze rodzic-dziecko, aby poprawnie wykonać zagnieżdżone Mail Merge z regionami. Pominięcie tego ważnego kroku może prowadzić do niepowodzenia w wykonywaniu zagnieżdżonego Mail Merge z regionami.

Podczas pobierania danych dla zagnieżdżonego Mail Merge z pliku XML przy użyciu metody **ReadXml** relacje są tworzone automatycznie zgodnie ze strukturą dokumentu XML. Musisz jednak upewnić się, że powstały prawidłowe relacje.

Jeśli Mail Merge nie działa zgodnie z oczekiwaniami, może być konieczna restrukturyzacja pliku XML lub jawne utworzenie relacji między obiektami DataTable w pliku DataSet.

`DataSet`, który ma powiązane tabele danych, użyje obiektu **DataRelation** do reprezentowania relacji rodzic-dziecko między tabelami.

Poniższy przykład kodu pokazuje, jak ustanowić `DataRelation` między tabelą klienta a tabelą zamówienia za pomocą obiektu `DataRelation`:
{{< highlight java >}}
dataSet.getRelations().add(new DataRelation("OrderToItem", orderTable.getColumns().get("Order_Id"), itemTable.getColumns().get("Order_Id"), false));
{{< /highlight >}}
