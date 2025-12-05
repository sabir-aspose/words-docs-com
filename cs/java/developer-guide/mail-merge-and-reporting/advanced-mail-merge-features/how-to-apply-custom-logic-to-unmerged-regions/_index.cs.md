---
title: Jak aplikovat vlastní logiku na nespojené oblasti
second_title: Aspose.Words pro Java
articleTitle: Jak aplikovat vlastní logiku na nespojené oblasti
linktitle: Jak aplikovat vlastní logiku na nespojené oblasti
type: docs
description: "Použijte vlastní logiku na nespojené oblasti během operace Mail Merge pomocí Java."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cs/java/how-to-apply-custom-logic-to-unmerged-regions/
timestamp: 2024-01-27-14-07-04
---

Existují situace, kdy úplné odstranění nespojených oblastí z dokumentu během Mail Merge není žádoucí nebo vede k tomu, že dokument vypadá neúplně. K tomu může dojít, když by měla být uživateli zobrazena absence vstupních dat ve formě zprávy namísto úplného odstranění oblasti.

Jsou také chvíle, kdy samotné odstranění nevyužité oblasti nestačí, například pokud oblasti předchází název nebo je oblast obsažena v tabulce. Pokud je tato oblast nevyužitá, zůstane název a tabulka i po odstranění oblasti, která bude v dokumentu vypadat nepatřičně.

Tento článek poskytuje řešení pro ruční definování způsobu zpracování nepoužívaných oblastí v dokumentu. Základní kód pro tuto funkci je dodáván a lze jej snadno znovu použít v jiném projektu.

Logika, která se má použít pro každou oblast, je definována uvnitř třídy, která implementuje rozhraní [IFieldMergingCallback](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/). Stejným způsobem lze nastavit obslužnou rutinu Mail Merge, která řídí, jak je každé pole sloučeno, tuto obslužnou rutinu lze nastavit tak, aby prováděla akce na každém poli v nepoužívané oblasti nebo v oblasti jako celku. V rámci této obslužné rutiny můžete nastavit kód pro změnu textu oblasti, odstranění uzlů nebo prázdných řádků a buněk atd.

V této ukázce použijeme níže uvedený dokument. Obsahuje vnořené oblasti a oblast obsaženou v tabulce.

![apply-custom-logic-to-unmerged-regions-aspose-words-java](how-to-apply-custom-logic-to-unmerged-regions-1.png)

Jako rychlou demonstraci můžeme spustit ukázkovou databázi na ukázkovém dokumentu s povoleným příznakem [MailMergeCleanupOptions.REMOVE_UNUSED_REGIONS](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/). Tato vlastnost automaticky odstraní nespojené oblasti z dokumentu během mail merge.

Zdroj dat obsahuje dva záznamy pro oblast **StoreDetails**, ale záměrně má jakákoli data pro podřízené oblasti **ContactDetails** pro jeden ze záznamů. Kromě toho oblast **Suppliers** nemá žádné datové řádky. To způsobí, že v dokumentu zůstanou nevyužité oblasti. Výsledek po sloučení dokumentu s tímto zdrojem dat je níže.

![merged-regions-aspose-words-java](how-to-apply-custom-logic-to-unmerged-regions-2.png)

Jak je uvedeno na obrázku, můžete vidět, že **ContactDetails** oblast pro druhý záznam a **Suppliers** oblasti byly automaticky odstraněny motorem Mail Merge, protože nemají žádná data. Existuje však několik problémů, díky nimž tento výstupní dokument vypadá neúplně:

- Oblast **ContactDetails** stále ponechává odstavec s textem "kontaktní údaje".
- Ve stejném případě nic nenasvědčuje tomu, že neexistují žádná telefonní čísla, pouze prázdné místo, které by mohlo vést ke zmatku.
- Tabulka a název související s oblastí **Suppliers** také zůstanou po odstranění oblasti uvnitř tabulky.

Technika uvedená v tomto článku ukazuje, jak aplikovat vlastní logiku na každou nespojenou oblast, aby se těmto problémům zabránilo.

**Řešení**

Chcete-li ručně použít logiku pro každou nepoužitou oblast v dokumentu, využíváme výhod funkcí, které jsou již k dispozici v Aspose.Words.

Motor Mail Merge poskytuje vlastnost pro odstranění nepoužívaných oblastí pomocí příznaku **MailMergeCleanupOptions.RemoveUnusedRegions**. To lze deaktivovat tak, aby tyto oblasti zůstaly nedotčeny během mail merge. To nám umožňuje ponechat nespojené oblasti v dokumentu a místo toho je zpracovat ručně.

Poté můžeme využít vlastnosti **MailMerge.FieldMergingCallback** jako prostředek k aplikaci naší vlastní logiky na tyto nespojené oblasti během Mail Merge pomocí třídy handler implementující rozhraní **IFieldMergingCallback**.

Tento kód ve třídě handler je jedinou třídou, kterou budete muset upravit, abyste mohli ovládat logiku aplikovanou na nespojené oblasti. Druhý kód v tomto vzorku lze znovu použít bez úprav v jakémkoli projektu.

Tento ukázkový projekt demonstruje tuto techniku. Zahrnuje následující kroky:

1. Spusťte Mail Merge na dokumentu pomocí zdroje dat. Příznak **MailMergeCleanupOptions.RemoveUnusedRegions** je prozatím deaktivován chceme, aby regiony zůstaly, abychom je mohli zpracovat ručně. Všechny oblasti bez dat zůstanou v dokumentu nespojené.
1. Zavolejte metodu **ExecuteCustomLogicOnEmptyRegions**. Tato metoda je uvedena v tomto vzorku. Provádí akce, které umožňují volání zadané obslužné rutiny pro každou nespojenou oblast. Tato metoda je opakovaně použitelná a lze ji beze změny zkopírovat do jakéhokoli projektu, který ji vyžaduje (spolu s jakýmikoli závislými metodami).Tato metoda provede následující kroky:
   1. Nastaví obslužnou rutinu určenou uživatelem na vlastnost **MailMerge.FieldMergingCallback**.
   1. Volá metodu **CreateDataSourceFromDocumentRegions**, která přijímá názvy oblastí obsahující uživatele **Document** a **ArrayList**. Tato metoda vytvoří fiktivní zdroj dat obsahující tabulky pro každou nespojenou oblast v dokumentu.
   1. Provede Mail Merge na dokumentu pomocí fiktivního zdroje dat. Když je Mail Merge spuštěn s tímto zdrojem dat, umožňuje volat uživatelem zadanou obslužnou rutinu pro každou oblast unmerge a použít vlastní logiku

**Kód**

Implementace metody **ExecuteCustomLogicOnEmptyRegions** je uvedena níže. Tato metoda přijímá několik parametrů:

1. Objekt [Document](https://reference.aspose.com/words/java/com.aspose.words/document/) obsahující nespojené oblasti, které mají být zpracovány předanou obslužnou rutinou.
1. Třída obslužné rutiny, která definuje logiku, která se má použít na nespojené oblasti. Tento psovod musí implementovat [IFieldMergingCallback](https://www.aspose.com/api/java/words/com.aspose.words/interfaces/IFieldMergingCallback) rozhraní.
1. Pomocí vhodného přetížení může metoda také přijmout třetí parametr-seznam názvů oblastí jako řetězce. Pokud je toto zadáno, budou ručně zpracovány pouze názvy oblastí zbývající v dokumentu zadaném v seznamu. Ostatní oblasti, které se vyskytnou, nebudou volány obslužnou rutinou a automaticky odstraněny. Když je zadáno přetížení pouze se dvěma parametry, každá zbývající oblast v dokumentu je zahrnuta metodou, která má být zpracována ručně.

**Příklad**

Ukazuje, jak spustit vlastní logiku v nepoužívaných oblastech pomocí zadané obslužné rutiny.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ExecuteCustomLogicOnUnusedRegions.java" >}}

{{% alert color="primary" %}}

Pokud uvažujete o spuštění metody **ExecuteCustomLogicOnEmptyRegions** postupně s různými obslužnými rutinami (např. každá obslužná rutina aplikuje logiku na určitá pole), budete muset zakázat odstranění nepoužívaných oblastí, aby tyto oblasti nebyly odstraněny mezi těmito voláními.

{{% /alert %}}

**Příklad**

Definuje metodu použitou k ručnímu zpracování nespojených oblastí.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ManuallyHandleUnmergedRegions.java" >}}

Tato metoda zahrnuje nalezení všech nespojených oblastí v dokumentu. To se provádí pomocí metody **MailMerge.GetFieldNames**. Tato metoda vrací všechna slučovací pole v dokumentu, včetně značek začátku a konce regionu (reprezentovaných sloučenými poli s předponou *TableStart* nebo *TableEnd*).

Když se objeví pole sloučení `TableStart`, přidá se jako nové **DataTable** do **DataSet**. Protože se oblast může objevit více než jednou (například proto, že se jedná o vnořenou oblast, kde byla nadřazená oblast sloučena s více záznamy), tabulka se vytvoří a přidá pouze v případě, že již neexistuje v **DataSet**.

Když byl nalezen příslušný začátek oblasti a přidán do databáze, přidá se do **DataTable** další pole (které odpovídá prvnímu poli v oblasti). Pro každé pole v oblasti, které má být sloučeno a předáno obslužné rutině, je nutné přidat pouze první pole.

Také jsme nastavili hodnotu pole prvního pole na " FirstField", abychom usnadnili použití logiky na první nebo jiná pole v oblasti. Zahrnutím to znamená, že není nutné tvrdě kódovat název prvního pole nebo implementovat další kód, abyste zkontrolovali, zda je aktuální pole první v kódu obslužné rutiny.

Níže uvedený kód ukazuje, jak tento systém funguje. Dokument zobrazený na začátku tohoto článku je remerged se stejným zdrojem dat, ale tentokrát, nevyužité oblasti jsou zpracovány vlastním kódem.

**Příklad**

Ukazuje, jak zacházet s nespojenými oblastmi po Mail Merge s uživatelem definovaným kódem.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-HandleUnmergedRegionsAfterMailMerge.java" >}}


Kód provádí různé operace na základě názvu oblasti načtené pomocí vlastnosti **FieldMergingArgs.TableName**. Všimněte si, že v závislosti na dokumentu a oblastech můžete kódovat obslužnou rutinu a spouštět logiku závislou na každé oblasti nebo kódu, který platí pro každou nespojenou oblast v dokumentu nebo kombinaci obou.

Logika pro oblast **ContactDetails** zahrnuje změnu textu každého pole v oblasti **ContactDetails** s příslušnou zprávou, že neexistují žádná data. Názvy každého pole jsou porovnány v obslužné rutině pomocí vlastnosti **FieldMergingArgs.FieldName**.

Podobný proces se aplikuje na oblast **Suppliers** s přidáním dalšího kódu pro zpracování tabulky, která oblast obsahuje. Kód zkontroluje, zda je oblast obsažena v tabulce (protože již mohla být odstraněna). Pokud ano, odstraní z dokumentu celou tabulku i odstavec, který jí předchází, pokud je naformátován stylem nadpisu, např. "Heading 1".

**Příklad**

Ukazuje, jak definovat vlastní logiku v obslužné rutině implementující IFieldMergingCallback, která je spuštěna pro nespojené oblasti v dokumentu.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-EmptyRegionsHandler.java" >}}

Výsledek výše uvedeného kódu je uveden níže. Nespojená pole v první oblasti jsou nahrazena informativním textem a odstranění tabulky a nadpisu umožňuje, aby dokument vypadal jako úplný.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-2](how-to-apply-custom-logic-to-unmerged-regions-3.png)


Kód, který odebere nadřazenou tabulku, lze také spustit v každé nepoužívané oblasti místo pouze v konkrétní oblasti odstraněním kontroly názvu tabulky. V tomto případě, pokud žádná oblast uvnitř tabulky nebyla sloučena s žádnými daty, bude oblast i tabulka kontejnerů automaticky odebrána.

Do obslužné rutiny můžeme vložit jiný kód, abychom určili, jak se zachází s nespojenými oblastmi. Použití kódu níže v obslužné rutině místo toho změní text v prvním odstavci oblasti na užitečnou zprávu, zatímco všechny následující odstavce v oblasti budou odstraněny. Tyto další odstavce jsou odstraněny, protože by zůstaly v regionu po sloučení naší zprávy.

Náhradní text je sloučen do prvního pole nastavením zadaného textu do vlastnosti **FieldMergingArgs.Text**. Text z této vlastnosti je sloučen do pole motorem Mail Merge.

Kód to použije pouze pro první pole v regionu zaškrtnutím vlastnosti **FieldMergingArgs.FieldValue**. Hodnota pole prvního pole v oblasti je označena "FirstField". To usnadňuje implementaci tohoto typu logiky v mnoha regionech, protože není vyžadován žádný další kód.

**Příklad**

Ukazuje, jak nahradit nepoužívanou oblast zprávou a odstranit další odstavce.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ReplaceAnUnusedRegionWithAMessage.java" >}}

Výsledný dokument po provedení výše uvedeného kódu je uveden níže. Nevyužitá oblast je nahrazena zprávou, že nejsou k dispozici žádné záznamy k zobrazení.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-3](how-to-apply-custom-logic-to-unmerged-regions-4.png)


Jako další příklad můžeme vložit níže uvedený kód místo kódu původně zpracovávajícího **SuppliersRegion**. Zobrazí se Zpráva v tabulce a sloučí se buňky namísto odebrání tabulky z dokumentu. Vzhledem k tomu, že oblast se nachází v tabulce s více buňkami, vypadá hezčí, když se buňky tabulky spojí dohromady a zpráva se vycentruje.

**Příklad**

Ukazuje, jak sloučit všechny nadřazené buňky nepoužívané oblasti a zobrazit zprávu v tabulce.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-MergeAllTheParentCellsOfAnUnusedRegion.java" >}}

Výsledný dokument po provedení výše uvedeného kódu je uveden níže.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-4](how-to-apply-custom-logic-to-unmerged-regions-5.png)


Nakonec můžeme zavolat metodu **ExecuteCustomLogicOnEmptyRegions** a určit názvy tabulek, které by měly být zpracovány v rámci naší metody obslužné rutiny, zatímco určíme ostatní, které mají být automaticky odstraněny.

**Příklad**

Ukazuje, jak určit pouze oblast `ContactDetails`, která má být zpracována pomocí třídy obslužné rutiny.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-HandleTheContactDetailsRegion.java" >}}

Volání tohoto přetížení zadaným ArrayList vytvoří zdroj dat, který obsahuje pouze datové řádky pro zadané oblasti. Jiné oblasti než oblast `ContactDetails` nebudou zpracovány a místo toho budou automaticky odstraněny motorem Mail Merge. Výsledek výše uvedeného volání pomocí kódu v našem původním obslužném programu je uveden níže.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-5](how-to-apply-custom-logic-to-unmerged-regions-6.png)
