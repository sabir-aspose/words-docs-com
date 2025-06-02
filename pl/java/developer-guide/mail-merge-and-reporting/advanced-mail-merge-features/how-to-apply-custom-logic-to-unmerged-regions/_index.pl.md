---
title: Jak zastosować logikę niestandardową do regionów Niezłączonych
second_title: Aspose.Words dla Java
articleTitle: Jak zastosować logikę niestandardową do regionów Niezłączonych
linktitle: Jak zastosować logikę niestandardową do regionów Niezłączonych
type: docs
description: "Zastosuj logikę niestandardową do regionów niezłączonych podczas operacji Mail Merge przy użyciu Java."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pl/java/how-to-apply-custom-logic-to-unmerged-regions/
timestamp: 2024-01-27-14-07-04
---

Istnieją sytuacje, w których całkowite usunięcie niezłączonych regionów z dokumentu podczas Mail Merge nie jest pożądane lub powoduje, że dokument wygląda na niekompletny. Może się to zdarzyć, gdy brak danych wejściowych powinien zostać wyświetlony użytkownikowi w postaci wiadomości zamiast całkowitego usunięcia regionu.

Są też chwile, kiedy samo usunięcie nieużywanego regionu nie wystarczy, na przykład, jeśli region jest poprzedzony tytułem lub region jest zawarty w tabeli. Jeśli ten region jest nieużywany, tytuł i tabela pozostaną po usunięciu regionu, który będzie wyglądał nie na miejscu w dokumencie.

W tym artykule przedstawiono rozwiązanie umożliwiające ręczne zdefiniowanie sposobu obsługi nieużywanych regionów w dokumencie. Kod podstawowy dla tej funkcji jest dostarczany i można go łatwo ponownie wykorzystać w innym projekcie.

Logika, która ma być zastosowana do każdego regionu, jest zdefiniowana wewnątrz klasy, która implementuje interfejs [IFieldMergingCallback](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/). W ten sam sposób można skonfigurować procedurę obsługi Mail Merge, aby kontrolować sposób scalania każdego pola, tę procedurę obsługi można skonfigurować tak, aby wykonywała działania na każdym polu w nieużywanym regionie lub w regionie jako całości. W ramach tej procedury obsługi możesz ustawić kod, aby zmienić tekst regionu, usunąć węzły lub puste wiersze i komórki itp.

W tym przykładzie będziemy używać dokumentu wyświetlanego poniżej. Zawiera zagnieżdżone regiony i region zawarty w tabeli.

![apply-custom-logic-to-unmerged-regions-aspose-words-java](how-to-apply-custom-logic-to-unmerged-regions-1.png)

Jako szybką demonstrację możemy wykonać przykładową bazę danych na przykładowym dokumencie z włączoną flagą [MailMergeCleanupOptions.REMOVE_UNUSED_REGIONS](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/). Ta właściwość automatycznie usunie niezmergowane regiony z dokumentu podczas mail merge.

Źródło danych zawiera dwa rekordy dla regionu **StoreDetails**, ale celowo zawiera dowolne dane dla regionów potomnych **ContactDetails** dla jednego z rekordów. Ponadto Region **Suppliers** również nie ma żadnych wierszy danych. Spowoduje to, że niewykorzystane regiony pozostaną w dokumencie. Wynik po scaleniu dokumentu z tym źródłem danych znajduje się poniżej.

![merged-regions-aspose-words-java](how-to-apply-custom-logic-to-unmerged-regions-2.png)

Jak zaznaczono na obrazku widać, że region **ContactDetails** dla drugiego rekordu i regiony **Suppliers** zostały automatycznie usunięte przez silnik Mail Merge, ponieważ nie mają danych. Istnieje jednak kilka problemów, które sprawiają, że ten dokument wyjściowy wygląda na niekompletny:

- Region **ContactDetails** nadal pozostawia akapit z tekstem"dane kontaktowe".
- W tym samym przypadku nic nie wskazuje na brak numerów telefonów, tylko puste miejsce, które może prowadzić do nieporozumień.
- Tabela i tytuł związane z regionem **Suppliers** pozostają również po usunięciu regionu wewnątrz tabeli.

Technika przedstawiona w tym artykule pokazuje, jak zastosować logikę niestandardową do każdego niezłączonego regionu, aby uniknąć tych problemów.

**Rozwiązanie**

Aby ręcznie zastosować logikę do każdego nieużywanego regionu w dokumencie, korzystamy z funkcji już dostępnych w Aspose.Words.

Silnik Mail Merge zapewnia właściwość usuwania nieużywanych regionów za pomocą flagi **MailMergeCleanupOptions.RemoveUnusedRegions**. Można to wyłączyć, aby takie regiony pozostały nietknięte podczas mail merge. To pozwala nam pozostawić niezmergowane regiony w dokumencie i zamiast tego obsługiwać je ręcznie.

Następnie możemy skorzystać z właściwości **MailMerge.FieldMergingCallback** jako środka do zastosowania naszej własnej logiki niestandardowej do tych niezłączonych regionów podczas Mail Merge za pomocą klasy obsługi implementującej interfejs **IFieldMergingCallback**.

Ten kod w klasie obsługi jest jedyną klasą, którą musisz zmodyfikować, aby kontrolować logikę stosowaną do regionów niezmergowanych. Drugi kod w tej próbce może być ponownie użyty bez modyfikacji w dowolnym projekcie.

Ten przykładowy projekt demonstruje tę technikę. Obejmuje następujące kroki:

1. Wykonaj Mail Merge na dokumencie przy użyciu źródła danych. Flaga **MailMergeCleanupOptions.RemoveUnusedRegions** jest wyłączona na razie chcemy, aby regiony pozostały, abyśmy mogli obsługiwać je ręcznie. Wszystkie regiony bez danych zostaną pozostawione bez połączenia w dokumencie.
1. Wywołaj metodę **ExecuteCustomLogicOnEmptyRegions**. Ta metoda jest podana w tej próbce. Wykonuje akcje, które pozwalają na wywołanie określonego programu obsługi dla każdego niezmergowanego regionu. Ta metoda jest wielokrotnego użytku i może być kopiowana w niezmienionej formie do dowolnego projektu, który jej wymaga (wraz z dowolnymi zależnymi metodami).Ta metoda wykonuje następujące kroki:
   1. Ustawia procedurę obsługi określoną przez użytkownika na Właściwość **MailMerge.FieldMergingCallback**.
   1. Wywołuje metodę **CreateDataSourceFromDocumentRegions**, która akceptuje **Document** i **ArrayList** użytkownika zawierające nazwy regionów. Ta metoda utworzy fikcyjne źródło danych zawierające tabele dla każdego niezłączonego regionu w dokumencie.
   1. Wykonuje Mail Merge Na dokumencie przy użyciu fikcyjnego źródła danych. Gdy Mail Merge jest wykonywany z tym źródłem danych, umożliwia wywołanie obsługi określonej przez użytkownika dla każdego regionu unmerge i zastosowanej logiki niestandardowej

**Kodeks**

Implementacja metody **ExecuteCustomLogicOnEmptyRegions** znajduje się poniżej. Ta metoda akceptuje kilka parametrów:

1. [Document](https://reference.aspose.com/words/java/com.aspose.words/document/) obiekt zawierający niezmergowane regiony, które mają być obsługiwane przez przekazaną procedurę obsługi.
1. Klasa obsługi, która definiuje logikę do zastosowania do regionów niezmergowanych. Ten program obsługi musi zaimplementować [IFieldMergingCallback](https://www.aspose.com/api/java/words/com.aspose.words/interfaces/IFieldMergingCallback) interfejs.
1. Dzięki zastosowaniu odpowiedniego przeciążenia metoda może również przyjąć trzeci parametr-listę nazw regionów jako ciągi. Jeśli jest to określone, tylko nazwy regionów Pozostałe dokument określony na liście będą obsługiwane ręcznie. Inne napotkane regiony nie będą wywoływane przez program obsługi i usuwane automatycznie. Gdy podano przeciążenie tylko dwoma parametrami, każdy pozostały region w dokumencie jest uwzględniany metodą, która ma być obsługiwana ręcznie.

**Przykład**

Pokazuje, jak wykonać niestandardową logikę na nieużywanych regionach przy użyciu określonej procedury obsługi.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ExecuteCustomLogicOnUnusedRegions.java" >}}

{{% alert color="primary" %}}

Jeśli rozważasz uruchomienie metody **ExecuteCustomLogicOnEmptyRegions** kolejno z różnymi programami obsługi (np. każdy program obsługi stosuje logikę do niektórych pól), musisz wyłączyć usuwanie nieużywanych regionów, aby takie regiony nie były usuwane między tymi wywołaniami.

{{% /alert %}}

**Przykład**

Definiuje metodę używaną do ręcznej obsługi regionów niezmergowanych.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ManuallyHandleUnmergedRegions.java" >}}

Ta metoda polega na znalezieniu wszystkich niezłączonych regionów w dokumencie. Odbywa się to za pomocą metody **MailMerge.GetFieldNames**. Ta metoda zwraca wszystkie pola scalania w dokumencie, w tym znaczniki początku i końca regionu (reprezentowane przez pola scalania z przedrostkiem *TableStart* lub *TableEnd*).

Po napotkaniu pola scalania `TableStart` jest ono dodawane jako nowe **DataTable** do **DataSet**. Ponieważ region może pojawić się więcej niż raz (na przykład dlatego, że jest to region zagnieżdżony, w którym region nadrzędny został scalony z wieloma rekordami), tabela jest tworzona i dodawana tylko wtedy, gdy nie istnieje jeszcze w pliku **DataSet**.

Po znalezieniu odpowiedniego początku regionu i dodaniu go do bazy danych, następne pole (odpowiadające pierwszemu polowi w regionie) jest dodawane do **DataTable**. Dla każdego pola w regionie, które ma zostać scalone i przekazane do modułu obsługi, wymagane jest dodanie tylko pierwszego pola.

Ustawiamy również wartość pola pierwszego pola na " FirstField", aby ułatwić zastosowanie logiki do pierwszego lub innych pól w regionie. Włączając to, oznacza to, że nie jest konieczne twarde kodowanie nazwy pierwszego pola lub implementuje dodatkowy kod, aby sprawdzić, czy bieżące pole jest pierwszym w kodzie obsługi.

Poniższy kod pokazuje, jak działa ten system. Dokument pokazany na początku tego artykułu jest uzupełniany o to samo źródło danych, ale tym razem nieużywane regiony są obsługiwane przez niestandardowy kod.

**Przykład**

Pokazuje, jak obsługiwać niezmergowane regiony po Mail Merge z kodem zdefiniowanym przez użytkownika.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-HandleUnmergedRegionsAfterMailMerge.java" >}}


Kod wykonuje różne operacje na podstawie nazwy regionu pobranego przy użyciu właściwości **FieldMergingArgs.TableName**. Należy pamiętać, że w zależności od dokumentu i regionów można zakodować program obsługi, aby uruchamiał logikę zależną od każdego regionu lub kodu, który ma zastosowanie do każdego niezłączonego regionu w dokumencie lub kombinacji obu.

Logika dla regionu **ContactDetails** polega na zmianie tekstu każdego pola w regionie **ContactDetails** z odpowiednim komunikatem informującym, że nie ma danych. Nazwy każdego pola są dopasowywane w programie obsługi przy użyciu właściwości **FieldMergingArgs.FieldName**.

Podobny proces jest stosowany do regionu **Suppliers** z dodaniem dodatkowego kodu do obsługi tabeli, która zawiera region. Kod sprawdzi, czy region jest zawarty w tabeli (ponieważ mógł zostać już usunięty). Jeśli tak, usunie całą tabelę z dokumentu, a także akapit, który ją poprzedza, o ile jest sformatowany za pomocą stylu nagłówka, np. "Heading 1".

**Przykład**

Pokazuje, jak zdefiniować logikę niestandardową w procedurze obsługi implementującej IFieldMergingCallback, która jest wykonywana dla regionów niezłączonych w dokumencie.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-EmptyRegionsHandler.java" >}}

Wynik powyższego kodu pokazano poniżej. Niezmergowane pola w pierwszym regionie są zastępowane tekstem informacyjnym, a usunięcie tabeli i nagłówka pozwala dokumentowi wyglądać na kompletny.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-2](how-to-apply-custom-logic-to-unmerged-regions-3.png)


Kod, który usuwa tabelę nadrzędną, można również uruchomić w każdym nieużywanym regionie, a nie tylko w określonym regionie, usuwając zaznaczenie nazwy tabeli. W takim przypadku, jeśli jakikolwiek region wewnątrz tabeli nie został scalony z żadnymi danymi, zarówno region, jak i tabela kontenerów również zostaną automatycznie usunięte.

Możemy wstawić inny kod w programie obsługi, aby kontrolować sposób obsługi niezmergowanych regionów. Użycie poniższego kodu w programie obsługi zamiast tego zmieni tekst w pierwszym akapicie regionu na pomocny komunikat, podczas gdy wszystkie kolejne akapity w regionie zostaną usunięte. Te inne akapity są usuwane, ponieważ pozostaną w regionie po scaleniu naszej wiadomości.

Tekst zastępczy jest scalany z pierwszym polem, ustawiając określony tekst we właściwości **FieldMergingArgs.Text**. Tekst z tej właściwości jest scalany w pole przez silnik Mail Merge.

Kod stosuje to tylko dla pierwszego pola w regionie, sprawdzając Właściwość **FieldMergingArgs.FieldValue**. Wartość pola pierwszego pola w regionie jest oznaczona " FirstField". Ułatwia to implementację tego typu logiki w wielu regionach, ponieważ nie jest wymagany dodatkowy kod.

**Przykład**

Pokazuje, jak zastąpić nieużywany region Komunikatem i usunąć dodatkowe akapity.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ReplaceAnUnusedRegionWithAMessage.java" >}}

Wynikowy dokument po wykonaniu powyższego kodu pokazano poniżej. Nieużywany region zostanie zastąpiony komunikatem informującym, że nie ma żadnych rekordów do wyświetlenia.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-3](how-to-apply-custom-logic-to-unmerged-regions-4.png)


Jako kolejny przykład możemy wstawić poniższy kod zamiast kodu pierwotnie obsługującego **SuppliersRegion**. Spowoduje to wyświetlenie komunikatu w tabeli i scalenie komórek zamiast usuwania tabeli z dokumentu. Ponieważ region znajduje się w tabeli z wieloma komórkami, ładniej wygląda scalanie komórek tabeli i wyśrodkowanie wiadomości.

**Przykład**

Pokazuje, jak scalić wszystkie komórki nadrzędne nieużywanego regionu i wyświetlić komunikat w tabeli.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-MergeAllTheParentCellsOfAnUnusedRegion.java" >}}

Wynikowy dokument po wykonaniu powyższego kodu pokazano poniżej.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-4](how-to-apply-custom-logic-to-unmerged-regions-5.png)


Na koniec możemy wywołać metodę **ExecuteCustomLogicOnEmptyRegions** i określić nazwy tabel, które powinny być obsługiwane w ramach naszej metody obsługi, jednocześnie określając inne, które mają zostać automatycznie usunięte.

**Przykład**

Pokazuje, jak określić tylko region `ContactDetails`, który ma być obsługiwany przez klasę obsługi.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-HandleTheContactDetailsRegion.java" >}}

Wywołanie tego przeciążenia za pomocą określonego ArrayList spowoduje utworzenie źródła danych, które zawiera tylko wiersze danych dla określonych regionów. Regiony inne niż region `ContactDetails` nie będą obsługiwane i zostaną automatycznie usunięte przez silnik Mail Merge. Wynik powyższego wywołania przy użyciu kodu w naszym oryginalnym programie obsługi pokazano poniżej.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-5](how-to-apply-custom-logic-to-unmerged-regions-6.png)
