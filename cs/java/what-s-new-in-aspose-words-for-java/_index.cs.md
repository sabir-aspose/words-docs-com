---
title: Co je nového
second_title: Aspose.Words pro Java
articleTitle: Co je nového v Aspose.Words pro Java
linktitle: Co je nového v Aspose.Words pro Java
type: docs
description: "Aspose.Words pro Java rozšiřuje a zvyšuje denně. Na této stránce se můžete dozvědět o obrovských a nejzajímavějších vlastnostech produktu."
weight: 2
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/java/what-s-new-in-aspose-words-for-java/
timestamp: 2025-06-23-21-02-49
---

Tato stránka popisuje nejzajímavější nové funkce Aspose.Words představené v posledních verzích.

## Aspose.Words pro Java 25.5, 25.6

Aspose.Words 25.5 vylepšuje přizpůsobení grafu novými možnostmi stylingu a vylepšuje export Markdown tím, že nabízí kontrolu nad tím, jak jsou zpracovávány prázdné odstavce.

Aspose.Words 25.6 vylepšuje přesnost Vykreslování a vizualizační funkce zavedením pokročilých možností exportu obrázků, vylepšené manipulace MathML a lepší reprezentace grafu.

### Převod, načítání a ukládání dokumentů

#### Export prázdných odstavců do Markdown <sup>25.5</sup>

Schopnost řídit, jak jsou prázdné odstavce exportovány do Markdown, byla zavedena přidáním výčtu [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownemptyparagraphexportmode/) a vlastnosti [EmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getEmptyParagraphExportMode).

#### Export vícestránkových dokumentů do formátů rastrových obrázků <sup>25.6</sup>

Možnost exportovat vícestránkové dokumenty do formátů rastrových obrázků (například PNG a JPEG) s [customizable layouts](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) – horizontální, vertikální nebo mřížka – byla zavedena rozšířením funkce exportu obrázků.

### Vykreslování

#### Nastavení stylu grafu <sup>25.5</sup>

Možnost nastavit styl grafu byla zavedena přidáním výčtu [ChartStyle](https://reference.aspose.com/words/java/com.aspose.words/chartstyle/) a vlastnosti [Style](https://reference.aspose.com/words/java/com.aspose.words/chart/#getStyle).

#### Vykreslování řádků konektoru ve výrazech MathML  <sup>25.6</sup>

Vykreslování konektorových čar ve výrazech MathML bylo implementováno, aby bylo zajištěno přesnější a vizuálně konzistentní zobrazení matematických vzorců.

#### Vykreslování Legend Pro Vodopád grafy <sup>25.6</sup>

Bylo zavedeno Vykreslování Legend Pro ["Waterfall" charts](https://reference.aspose.com/words/java/com.aspose.words/chartseriestype/), což zvyšuje transparentnost dat a zlepšuje interpretovatelnost těchto grafů.

### Jiný

* Byla vylepšena schopnost zabalit matematické vzorce obsahující více lomítek, což zlepšuje přehlednost rozvržení a čitelnost vzorce. <sup>25.6</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words pro Java 25.5 Poznámky k vydání](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-5-release-notes/).

Další informace o [Aspose.Words pro Java 25.6 Poznámky k vydání](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words Pro Java 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 zavádí kontrolu gramatiky pomocí AI a vylepšuje ukládání dokumentů pomocí pokročilých možností pro formáty HTML, SVG a Markdown.

Aspose.Words 25.2 zavádí shrnutí textu pomocí modelů Anthropic AI, přidává podporu formátu MsWorks, vylepšuje typografické ovládání a zlepšuje strukturu a zpracování seznamu PDF.

Aspose.Words 25.3 vylepšuje kontrolu gramatiky a výběr písma pomocí AI s vlastností UpdateAmbiguousTextFont a také vylepšuje export příloh PDF.

Aspose.Words 25.4 zavádí podporu pro nové velikosti papíru, umožňuje pokročilé řízení exportu HTML, zlepšuje manipulaci s vodoznakem a zvyšuje použitelnost LowCode API.

### AI - poháněné funkce

#### Kontrola Gramatiky AI

* Schopnost kontrolovat gramatiku poskytnutého dokumentu pomocí OpenAI generativních modelů byla zavedena přidáním nové metody [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions). <sup>25.1</sup>
* Funkce kontroly gramatiky založená na AI byla aktualizována tak, aby podporovala všechny modely dostupné ve výčtu [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). <sup>25.3</sup>

#### Shrnutí Pomocí Anthropic Generativních Jazykových Modelů <sup>25.2</sup>

Shrnutí textu pomocí Anthropic generativních jazykových modelů bylo povoleno zavedením nové veřejné třídy [AnthropicAiModel](https://reference.aspose.com/words/java/com.aspose.words/anthropicaimodel/).

### Low Code

#### Low Code API použitelnost <sup>25.4</sup>

Byla zavedena významná vylepšení použitelnosti **LowCode API**, která zjednodušují zpracování dokumentů a snižují potřebu opakovaného kódu.

### Podporované Formáty <sup>25.2</sup>

Od verze 25.2 byla přidána kompatibilita s novým formátem načítání MsWorks pro pracovní dokumenty Microsoft.

### Převod, načítání a ukládání dokumentů

#### Vylepšené ukládání do formátů HTML a SVG <sup>25.1</sup>

Ukládání do formátů HTML a SVG bylo vylepšeno přidáním vlastností **IdPrefix** a **RemoveJavaScriptFromLinks** do tříd [HtmlFixedSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlfixedsaveoptions/) a [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/).

#### Nastavte rozlišení obrazu a výstupní režim OfficeMath při ukládání do Markdown <sup>25.1</sup>

* Do třídy [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) byla přidána nová možnost [ImageResolution](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImageResolution) pro nastavení rozlišení obrazu.
* Do třídy [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) byla přidána nová volba [OfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getOfficeMathExportMode) a výčet [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownofficemathexportmode/) pro nastavení výstupního režimu OfficeMath.
* Možnost nastavit vodoznak obrázku ze streamu byla zavedena přidáním nového přetížení do metody [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.io.InputStream-com.aspose.words.ImageWatermarkOptions). <sup>25.4</sup>

### Vykreslování

#### Vylepšené Typografické Ovládání <sup>25.2</sup>

Vlastnost [NumberSpacing](https://reference.aspose.com/words/java/com.aspose.words/font/#getNumberSpacing) byla přidána pro lepší typografické ovládání.

#### Ovládání výběru písma pro nejednoznačné znaky <sup>25.3</sup>

Do třídy [SaveOptions](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/) byla přidána nová veřejná vlastnost [UpdateAmbiguousTextFont](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/#getUpdateAmbiguousTextFont), která řídí výběr písma podle použitého znakového kódu.

#### Možnosti Velikosti Papíru <sup>25.4</sup>

Schopnost používat JIS B4 a JIS B5 velikosti papíru byla zavedena přidáním nových hodnot do výčtu [PaperSize](https://reference.aspose.com/words/java/com.aspose.words/papersize/).

#### HTML Výstupní Řízení <sup>25.4</sup>

Možnost odebrat JavaScript z hypertextového odkazu URLs během exportu HTML byla zavedena přidáním vlastnosti [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/#getRemoveJavaScriptFromLinks).

### Jiný

* Logická struktura PDF byla vylepšena podporou polí TOA, BIBLIOGRAPHY a INDEX. <sup>25.2</sup>
* Pro lepší zpracování seznamu byla zavedena metoda [AddSingleLevelList](https://reference.aspose.com/words/java/com.aspose.words/listcollection/#addSingleLevelList-int). <sup>25.2</sup>
* Byla přidána nová vlastnost [AttachmentsEmbeddingMode](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getAttachmentsEmbeddingMode), která nahradí **EmbedAttachments** a zlepší export příloh PDF. Do výčtu [PdfCompliance](https://reference.aspose.com/words/java/com.aspose.words/pdfcompliance/) byly také přidány nové hodnoty, které podporují přílohy verze PDF/A. Kromě toho jsou přílohy nyní podporovány šifrováním. <sup>25.3</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words Pro Java 25.1 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-1-release-notes/).

Další informace o [Aspose.Words pro Java 25.2 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-2-release-notes/).

Další informace o [Aspose.Words Pro Java 25.3 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-3-release-notes/).

Další informace o [Aspose.Words Pro Java 25.4 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words pro Java 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 zavádí group shape vkládání a StructuredDocumentTag vkládání pomocí DocumentBuilder, vylepšuje Vykreslování radiálního grafu s odstupňováním, vylepšuje digitální podpisy s podporou XAdES-EPES, přidává Markdown rozpoznávání podtržení a poskytuje přístup k oddělovačům poznámek pod čarou/vysvětlivek.

Aspose.Words 24.10 zavádí vylepšenou podporu řízení ActiveX s vytvářením CommandButton, novým ovládáním viditelnosti tvarů, schopností group shapes, vylepšeným exportem Markdown pro tabulky, formátováním grafů pro grafy Pie a Doughnut, lepší manipulací s kódováním Big5 a podporou zastaralých tchajwanských písem.

Aspose.Words 24.11 představuje souhrn dokumentů poháněný AI, vylepšené možnosti Vykreslování, vylepšený přístup k vlastnostem dokumentu a ActiveX Ovládání titulků.

Aspose.Words 24.12 zavádí přizpůsobitelné umístění datových štítků, překlad textu pomocí Google AI, vylepšené možnosti vyčištění Mail Merge a nové třídy zpracování LowCode.

### AI - poháněné funkce

#### Shrnutí dokumentu pomocí OpenAI a Google <sup>24.11</sup>

Byla integrována podpora sumarizace dokumentů pomocí generativních jazykových modelů **OpenAI** a **Google**.

#### Překlad textu pomocí generativních jazykových modelů Google <sup>24.12</sup>

Schopnost překládat text pomocí generativních jazykových modelů Google byla implementována v Aspose.Words přidáním metody [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) a výčtu [Language](https://reference.aspose.com/words/java/com.aspose.words/language/).

### Low Code <sup>24.12</sup>

Nové LowCode třídy jako [Comparer](https://reference.aspose.com/words/java/com.aspose.words/comparer/), [MailMerger](https://reference.aspose.com/words/java/com.aspose.words/mailmerger/), [Replacer](https://reference.aspose.com/words/java/com.aspose.words/replacer/), [Splitter](https://reference.aspose.com/words/java/com.aspose.words/splitter/) atd. byl představen a nabízí sadu metod, které vytvářejí dokonalou rovnováhu mezi jednoduchostí a flexibilitou pro zpracování dokumentů.

### Vykreslování a tisk

#### Promoce na radiálních grafech <sup>24.9</sup>

Bylo implementováno Vykreslování promocí na radiálních grafech.

#### CommandButton ActiveX ovládací prvky <sup>24.10</sup>

Schopnost vytvářet ovládací prvky CommandButton ActiveX byla zavedena přidáním nové veřejné metody [InsertForms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertForms2OleControl-com.aspose.words.Forms2OleControl) a nové veřejné třídy [Forms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/).

#### Kontrola Viditelnosti Tvaru <sup>24.10</sup>

Byla přidána nová veřejná vlastnost [Hidden](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#getHidden) pro řízení viditelnosti obrazců.

#### Změny v grafech Pie a Doughnut <sup>24.10</sup>

Do grafů format Pie a Doughnut bylo přidáno několik nových veřejných vlastností.

#### Řízení Vykreslování PDF výběrový formulář ohraničení polí <sup>24.11</sup>

Byla implementována nová možnost pro řízení Vykreslování okrajů polí PDF výběrového formuláře přidáním nové veřejné volby [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getRenderChoiceFormFieldBorder).

#### Získejte a nastavte kódy formátu pro data grafu <sup>24.11</sup>

Schopnost získat a nastavit kódy formátu pro data grafu byla přidána implementací vlastnosti [FormatCode](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/#getFormatCode) do tříd [ChartXValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartyvaluecollection/) a [BubbleSizeCollection](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/).

#### Vykreslení Histogramových grafů s přihrádkami a štítky <sup>24.11</sup>

Vykreslování grafu histogramu bylo vylepšeno umožněním zadaného počtu přihrádek a štítků.

### Převod, načítání a ukládání dokumentů

#### Při načítání souborů Markdown podtrhněte formátování <sup>24.9</sup>

Možnost rozpoznat formátování podtržení při načítání dokumentů Markdown byla začleněna přidáním nové veřejné vlastnosti [ImportUnderlineFormatting](https://reference.aspose.com/words/java/com.aspose.words/markdownloadoptions/#getImportUnderlineFormatting).

#### Export tabulek jako HTML při ukládání do Markdown <sup>24.10</sup>

Možnost exportovat tabulky jako HTML při ukládání dokumentů do formátu Markdown byla implementována přidáním nové veřejné vlastnosti [ExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getExportAsHtml) a výčtu [MarkdownExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownexportashtml/).

#### Export PDF s aktualizovanou logickou strukturou <sup>24.11</sup>

Export PDF byl vylepšen zahrnutím vlastností názvu tabulky jako názvů prvků logické struktury PDF.

### Mail Merge a podávání zpráv

#### Odstraňte prázdné tabulky během Mail Merge <sup>24.12</sup>

Do výčtu [MailMergeCleanupOptions](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/) byla přidána nová možnost **RemoveEmptyTables** pro upřesnění výstupu Mail Merge.

### Digitální Podpisy

#### Podepisujte dokumenty XAdES-EPES <sup>24.9</sup>

Schopnost podepisovat dokumenty s podpisy XAdES-EPES úrovně XML-DSig byla zavedena přidáním nového veřejného majetku [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/signoptions/#getXmlDsigLevel) a nového veřejného výčtu [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/xmldsiglevel/)

### Jiný

* Do group shapes byla přidána nová veřejná metoda [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-com.aspose.words.Shape...). <sup>24.9</sup>
* Byla přidána nová veřejná metoda [InsertStructuredDocumentTag](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertStructuredDocumentTag-int) pro vložení **StructuredDocumentTags** do dokumentu. <sup>24.9</sup>
* Veřejný přístup k oddělovačům poznámek pod čarou/vysvětlivek byl poskytnut přidáním několika veřejných tříd a vlastností. <sup>24.9</sup>
* Schopnost seskupovat jednotlivé tvary group shapes dohromady a přímo seskupovat oba tvary a group shapes byla zavedena přidáním metody [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-double-double-double-double-com.aspose.words.ShapeBase...). <sup>24.10</sup>
* Zpracování kódování Big5 pro TrueType CMAP tabulky bylo vylepšeno. <sup>24.10</sup>
* Byla rozšířena podpora zastaralých tchajwanských písem. <sup>24.10</sup>
* Pro přístup k rozšířeným vlastnostem dokumentu byly do třídy [BuiltInDocumentProperties](https://reference.aspose.com/words/java/com.aspose.words/builtindocumentproperties/) přidány vlastnosti pouze pro čtení. <sup>24.11</sup>
* Nastavení titulků pro ovládací prvky ActiveX bylo povoleno přidáním nového veřejného nastavovače do vlastnosti [Forms2OleControl.Caption](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/#getCaption). <sup>24.11</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words pro Java 24.9 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-9-release-notes/).

Další informace o [Aspose.Words Pro Java 24.10 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-10-release-notes/).

Další informace o [Aspose.Words Pro Java 24.11 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-11-release-notes/).

Další informace o [Aspose.Words Pro Java 24.12 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words pro Java 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 rozšiřuje možnosti sestav, zlepšuje možnosti Vykreslování a rozšiřuje některé další možnosti.

Aspose.Words 24.6 vylepšuje možnosti Vykreslování, vylepšuje funkce vyhledávání a porovnávání a rozšiřuje několik dalších funkcí.

Aspose.Words 24.7 mění způsob práce s ActiveX, rozšiřuje možnosti Vykreslování a exportuje do formátů Markdown a XLSX.

Aspose.Words 24.8 vylepšuje přizpůsobení grafu s přesnou kontrolou nad popisky os, rozšiřuje správu písem, zlepšuje manipulaci se strukturou dokumentů a přidává nové možnosti pro export HTML/XAML, funkčnost PDF, převod dokumentů a digitální podpisy.

### Podporované Formáty

Počínaje verzí 24.7 je podporován export do PDF/UA-2, aby byla zajištěna dostupnost pro uživatele se zdravotním postižením.

### Vykreslování a tisk

#### Změny v grafech, tvarech a DrawingML <sup>24.5</sup>

- DrawingML Vykreslování efektů pro grafiku SVG, Rozšíření předchozí funkce omezené na obrázky, bylo implementováno.
- Podpora pro vytváření kombinovaných grafů a úpravy vlastností, jako je šířka mezery, překrytí a stupnice bublin v rámci skupin sérií, byla zavedena přidáním tříd [ChartSeriesGroup](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroup/) a [ChartSeriesGroupCollection](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroupcollection/) a vlastnosti [SeriesGroups](https://reference.aspose.com/words/java/com.aspose.words/chart/#getSeriesGroups).
- Funkce pro manipulaci s efektem tvarů SoftEdge byla implementována přidáním třídy [SoftEdgeFormat](https://reference.aspose.com/words/java/com.aspose.words/softedgeformat/).
- Možnost upravit upravit hodnoty tvarů byla implementována přidáním veřejných tříd [AdjustmentCollection](https://reference.aspose.com/words/java/com.aspose.words/adjustmentcollection/) a [Adjustment](https://reference.aspose.com/words/java/com.aspose.words/adjustment/) a vlastnosti [Adjustments](https://reference.aspose.com/words/java/com.aspose.words/shape/#getAdjustments).

#### Změny v grafech, tvarech a kreslení <sup>24.6</sup>

- Byly vylepšeny možnosti mapování. Nyní můžete vytvořit širší škálu grafů, včetně *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* grafy, *Box & Whisker* grafy, *Waterfalls* a *Funnels*. To vám umožní vizualizovat vaše data rozmanitějším a informativnějším způsobem.
- Ovládání barev pro formátování stínů bylo vylepšeno. Přesnější kontrolu nad vzhledem dokumentů můžete získat přístupem k barvám stínů.
- Zvýšení výkonu pro vykreslování pozadí bylo vylepšeno. Díky nativní technologii obkladů můžete výrazně urychlit vykreslování pozadí obsahujících malé prvky.
- Byly přidány realistické přechody pro tvary. Nyní můžete vytvářet DML tvary s nelineárními přechody, napodobující vizuální styl Microsoft Word pro vyleštěnější vzhled.

#### Přizpůsobení Štítku Dat Grafu <sup>24.7</sup>

Byla přidána možnost přizpůsobit štítky dat grafu, jako jsou **Orientation** a **Rotation**.

#### Vlastní styl čísel pro úrovně seznamu <sup>24.7</sup>

Byl přidán setr pro veřejný majetek [CustomNumberStyleFormat](https://reference.aspose.com/words/java/com.aspose.words/listlevel/#getCustomNumberStyleFormat). Nyní můžete definovat vlastní styl čísel pro úrovně seznamu.

#### Změny v práci s ActiveX <sup>24.7</sup>

* Vlastnosti objektů ActiveX lze nyní upravit, což vám dává větší kontrolu nad jejich chováním.
* Byla přidána možnost upravit hodnotu ovládacího prvku přepínače ActiveX, aby byla povolena dynamická interakce.
* Byla přidána možnost přepnout ActiveX checkbox na "zaškrtnuto" nebo "nezaškrtnuto".

#### Kontrola nad osou grafu klíště popisky orientace a rotace <sup>24.8</sup>

Pro pohodlnější přizpůsobení grafu byla přidána přesná kontrola nad orientací a rotací štítků klíštěte osy grafu – třída [AxisTickLabels](https://reference.aspose.com/words/java/com.aspose.words/axisticklabels/) byla rozšířena o nové vlastnosti **Orientation** a **Rotation**.

#### Nahrazení zpětného lomítka znakem jenu <sup>24.8</sup>

Zpětně kompatibilní HTML a XAML export pro nahrazení znaku zpětného lomítka znakem jenu byl vylepšen. K dosažení tohoto cíle byla vlastnost **ReplaceBackslashWithYenSign** přidána do tříd [HtmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/) a [XamlFlowSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/).

#### Použití značek SDT jako názvů polí formuláře při exportu do PDF <sup>24.8</sup>

PDF export s podporou použití značek SDT jako názvů polí formuláře byl vylepšen přidáním nové vlastnosti **UseSdtTagAsFormFieldName** do třídy [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/).

### Převod, načítání a ukládání dokumentů

#### Export odkazů do formátu Markdown <sup>24.7</sup>

Schopnost řídit export odkazů ve formátu Markdown byla přidána implementací vlastnosti [LinkExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getLinkExportMode).

#### LowCode 24.8 <sup>24.8</sup>

Byla zavedena nová třída **LowCode.Converter**, navržená tak, aby poskytovala sadu metod pro převod různých typů dokumentů pomocí jediného řádku kódu.

### Hledat a porovnávat

#### Pokročilé Možnosti Porovnání <sup>24.6</sup>

Byla přidána možnost zefektivnit pracovní postupy analýzy dat s vylepšenou funkcí porovnávání. To zahrnuje novou možnost [IgnoreStoreItemId](https://reference.aspose.com/words/java/com.aspose.words/advancedcompareoptions/#getIgnoreStoreItemId) a přepracované rozhraní pro pokročilá srovnání.

### Jiný

* Funkce pro odstranění prázdných stránek z dokumentu byla implementována přidáním metody [RemoveBlankPages](https://reference.aspose.com/words/java/com.aspose.words/document/#removeBlankPages). <sup>24.5</sup>
* Možnost zkontrolovat přítomnost Maker VBA bez načtení dokumentu byla poskytnuta přidáním vlastnosti [HasMacros](https://reference.aspose.com/words/java/com.aspose.words/fileformatinfo/#hasMacros). <sup>24.5</sup>
* Nyní je podporováno udržování číslování zdrojů při vkládání dokumentu pomocí LINQ Reporting Engine. <sup>24.5</sup>
* Byla přidána nová vlastnost [DateTimeUtc](https://reference.aspose.com/words/java/com.aspose.words/comment/#getDateTimeUtc) - poskytuje přesnější časové razítko pro Komentáře, zlepšuje organizaci a sledovatelnost. <sup>24.6</sup>
* LINQ Reporting Engine byl vylepšen. Bylo provedeno selektivní odstranění prázdných odstavců a definice vlastních zpráv pro chybějící členy objektu, což vede k čistším a informativnějším zprávám. <sup>24.6</sup>
* Formát datetime je nyní automaticky detekován pro bezproblémový export do formátu XLSX. <sup>24.7</sup>
* Byla přidána veřejná vlastnost [IsProtected](https://reference.aspose.com/words/java/com.aspose.words/vbaproject/#isProtected), která umožňuje ověřit, zda je projekt VBA chráněn. <sup>24.7</sup>
* Informace o Písmu byly rozšířeny o vlastnost **EmbeddingLicensingRights** přidanou do tříd [FontInfo](https://reference.aspose.com/words/java/com.aspose.words/fontinfo/) a [PhysicalFontInfo](https://reference.aspose.com/words/java/com.aspose.words/physicalfontinfo/). <sup>24.8</sup>
* Pro přesnější práci se strukturou dokumentu byl přidán způsob, jak efektivně vymazat záhlaví a zápatí sekcí při zachování vodoznaků. Chcete-li vymazat záhlaví a zápatí oddílů, použijte novou veřejnou metodu **ClearHeadersFooters**. <sup>24.8</sup>
* Bylo povoleno digitální podepisování dokumentů XPS Pomocí [XpsSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xpssaveoptions/) – pro tento účel byla přidána nová vlastnost **DigitalSignatureDetails**. <sup>24.8</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words Pro Java 24.5 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-5-release-notes/).

Další informace o [Aspose.Words pro Java 24.6 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-6-release-notes/).

Další informace o [Aspose.Words pro Java 24.7 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-7-release-notes/).

Další informace o [Aspose.Words pro Java 24.8 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words pro Java 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 zlepšuje zážitek kolem správy barev tahů, vylepšuje OLE objekty a LINQ hlášení, stejně jako zavádí novou bibliografii zdroje veřejné API.

Aspose.Words 24.2 rozšířené grafy API, Správa stylů a LINQ možnosti. Tato verze Aspose.Words také zavedla schopnost specifikovat SvgSaveOptions během Vykreslování, flexibilnější ovládání načítání souborů Markdown a práci s referenčním textem pro poznámky pod čarou a vysvětlivky.

Aspose.Words 24.3 zavádí nový TIFF Reader / Writer a emulaci binárních rastrových operací pro WMF metasoubory. Aspose.Words 24.3 také pokračuje v rozšiřování grafů API.

Aspose.Words 24.4 vylepšuje ukládání formátů, některé možnosti Vykreslování a zlepšuje práci s digitálními podpisy.

### Podporované Formáty <sup>24.4</sup>

Moderní formát obrázku **WebP** je nyní podporován v Aspose.Words. Nyní můžete číst a vkládat obrázky WebP do dokumentů a také ukládat obrázky ve formátu WebP.

### Vykreslování a tisk

#### Ovládání Barev Tahu <sup>24.1</sup>

Třída [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) byla rozšířena o sadu nových veřejných vlastností souvisejících se správou barev tahů: [ForeThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeThemeColor) a [BackThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackThemeColor), [ForeTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeTintAndShade) a [BackTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackTintAndShade).

#### DrawingML Grafy API Rozšíření <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** se stále rozšiřuje.

#### Vložit písma deklarovaná v pravidlech @font-face <sup>24.4</sup>

Přidána možnost vkládat písma deklarovaná v pravidlech @font-face do definic písem výsledného dokumentu byla zavedena přidáním nové vlastnosti [SupportFontFaceRules](https://reference.aspose.com/words/java/com.aspose.words/htmlloadoptions/#getSupportFontFaceRules).

#### Práce s formátováním záře a odrazu <sup>24.4</sup>

Byla implementována schopnost pracovat s formátováním záře a odrazu pro kreslící objekt.

### Načítání a ukládání dokumentů

#### Zadejte SvgSaveOptions Během Vykreslování <sup>24.2</sup>

Schopnost specifikovat [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/) během Vykreslování byla přidána pomocí [ShapeRenderer](https://reference.aspose.com/words/java/com.aspose.words/shaperenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) a [OfficeMathRenderer](https://reference.aspose.com/words/java/com.aspose.words/officemathrenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) metody.

#### Při načítání souborů Markdown Zachovejte prázdné řádky <sup>24.2</sup>

Byla přidána možnost zachovat prázdné řádky při načítání souborů Markdown.

#### Nový TIFF Čtenář / Spisovatel <sup>24.3</sup>

Byl vyvinut nový TIFF reader/writer pro Aspose.Words pro .NET Standard, .NET 6 a později. Aspose.Words pro .NET 24.3 přidána podpora pro čtení TIFF obrázků s JPEG a starými typy komprese JPEG a také výrazně zlepšila kvalitu operací čtení a zápisu.

### Jiný

* Schopnost upravit text ovládacího prvku `TextBox` OLE byla zavedena přidáním nové vlastnosti [Text](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/#getText) do nové třídy [TextBoxControl](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/). 24.1 <sup>24.1</sup>
* Bibliografické zdroje veřejné API byly implementovány přidáním několika nových [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/bibliography/), [Source](https://reference.aspose.com/words/java/com.aspose.words/source/), [ContributorCollection](https://reference.aspose.com/words/java/com.aspose.words/contributorcollection/), [Contributor](https://reference.aspose.com/words/java/com.aspose.words/contributor/), [Corporate](https://reference.aspose.com/words/java/com.aspose.words/corporate/), [PersonCollection](https://reference.aspose.com/words/java/com.aspose.words/personcollection/) a [Person](https://reference.aspose.com/words/java/com.aspose.words/person/) třídy A a [SourceType](https://reference.aspose.com/words/java/com.aspose.words/sourcetype/) výčet, stejně jako přidáním nové vlastnosti [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/document/#getBibliography) do třídy [Document](https://reference.aspose.com/words/java/com.aspose.words/document/). <sup>24.1</sup>
* API k omezení přístupu k členům typu pomocí syntaxe šablony pro LINQ Reporting Engine byl poskytnut. <sup>24.1</sup>
* Do třídy [Style](https://reference.aspose.com/words/net/aspose.words/style/) byly přidány nové veřejné vlastnosti [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) a [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) pro rozšířenou správu stylů. <sup>24.2</sup>
* Funkce pro načtení skutečného textu referenční značky pro poznámky pod čarou a vysvětlivky byla vylepšena vlastností [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) a metodou [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* Kompatibilita s `Word 2016` grafy pro `LINQ Reporting Engine` byla povolena. <sup>24.2</sup>
* Byla implementována emulace binárních rastrových operací pro metasoubory WMF. <sup>24.3</sup>
* Možnost definovat možnosti podpisu pro dokumenty v rámci **SaveOptions** byla povolena přidáním nové třídy [DigitalSignatureDetails](https://reference.aspose.com/words/java/com.aspose.words/digitalsignaturedetails/) s novými veřejnými členy a přidáním nových vlastností do tříd [OoxmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/docsaveoptions/) a [OdtSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words Pro Java 24.1 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-1-release-notes/).

Další informace o [Aspose.Words pro Java 24.2 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-2-release-notes/).

Další informace o [Aspose.Words Pro Java 24.3 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-3-release-notes/).

Další informace o [Aspose.Words pro Java 24.4 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words pro Java 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 rozšiřuje možnosti Vykreslování, emulaci Vykreslování metafile a markdown Možnosti uložení.

Aspose.Words 23.10 zlepšuje vykreslování, rozšiřuje možnosti načítání a ukládání dokumentů a umožňuje uživatelům sloučit dokumenty novými způsoby.

Aspose.Words 23.11 vylepšuje práci s revizemi, formátem XLSX a fonty na legendě grafu s dalšími možnostmi.

Aspose.Words 23.12 zavádí nové vlastnosti a výčty pro práci s dokumenty PDF, podporu obrázků WebP a aktualizovanou knihovnu skákacího hradu.

### Vykreslování a tisk

#### Přizpůsobení názvů OS v grafech DrawingML <sup>23.9</sup>

Schopnost přizpůsobit názvy os v grafech DrawingML byla zavedena implementací nové veřejné třídy [ChartAxisTitle](https://reference.aspose.com/words/java/com.aspose.words/chartaxistitle/) a [Title](https://reference.aspose.com/words/java/com.aspose.words/chartaxis/#getTitle) vlastnost.

#### Určení svislé polohy písem v odstavci <sup>23.9</sup>

Nyní je možné definovat svislou polohu písem v odstavci pomocí nové veřejné vlastnosti [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getBaselineAlignment) a Nového výčtu [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/baselinealignment/).

#### Ovládání Barev Popředí <sup>23.10</sup>

Schopnost načíst barvu popředí bez modifikátorů byla přidána do tříd [Fill](https://reference.aspose.com/words/java/com.aspose.words/fill/) a [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) pomocí Vlastnosti **BaseForeColor**.

#### Rozšíření funkčnosti grafů <sup>23.10</sup>

Funkce tříd [ChartDataPointCollection](https://reference.aspose.com/words/java/com.aspose.words/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/java/com.aspose.words/chartseries/) a [ChartFormat](https://reference.aspose.com/words/java/com.aspose.words/chartformat/) byla rozšířena o nové metody a vlastnosti.

#### Automatické nastavení a přizpůsobení obrázku do tvaru <sup>23.10</sup>

Jednoduchý způsob, jak automaticky upravit a přizpůsobit obrázek do určitého tvaru, byl poskytnut pomocí nové metody [FitImageToShape](https://reference.aspose.com/words/java/com.aspose.words/imagedata/#fitImageToShape).

#### Výchozí formátování písma pro DrawingML položky legendy grafu <sup>23.11</sup>

Možnost zadat výchozí formátování písma pro položky legendy DrawingML grafů byla přidána pomocí vlastnosti **Font**. Tato funkce usnadňuje efektivnější a konzistentnější vzhled prvků grafu a zlepšuje celkovou estetiku dokumentu.

#### Určete Rozložení stránky při otevírání PDF v Readeru <sup>23.12</sup>

Schopnost určit rozvržení stránky, které se má použít při otevírání dokumentu ve čtečce PDF, byla přidána zavedením nové vlastnosti [PageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getPageLayout) do třídy [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/) a zavedením nového výčtu [PdfPageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfpagelayout/).

### Načítání a ukládání dokumentů

#### Zadání názvu složky pro vytvoření obrázku URIs v Markdown <sup>23.9</sup>

Třída [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) byla rozšířena o vlastnost [ImagesFolderAlias](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImagesFolderAlias), která umožňuje určit název složky použité ke konstrukci obrazu URIs zapsaného do dokumentu Markdown.

#### Zmenšit Velikost Výstupu PDF <sup>23.10</sup>

Byly implementovány různé optimalizace Vykreslování PDF pro zmenšení velikosti výstupu při použití nastavení [OptimizeOutput](https://reference.aspose.com/words/java/com.aspose.words/fixedpagesaveoptions/#getOptimizeOutput).

#### Rozpoznání hypertextových odkazů při načítání dokumentů TXT <sup>23.10</sup>

Funkce rozpoznání hypertextových odkazů při načítání dokumentů TXT byla implementována přidáním nové vlastnosti [DetectHyperlinks](https://reference.aspose.com/words/java/com.aspose.words/txtloadoptions/#getDetectHyperlinks).

### Jiný

- Byla implementována emulace Metafile rendering pro určení velikosti rasterizace, konkrétně pro WMF šířku pera a EMF šířku kosmetického pera. K dosažení tohoto cíle byla vlastnost **ScaleWmfFontsToMetafileSize** nahrazena vlastností [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPage) a byla přidána vlastnost [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPageResolution). <sup>23.9</sup>
- Byla zavedena zjednodušená metoda pro vložení jednoho dokumentu do jiného dokumentu na aktuální pozici kurzoru pomocí metody [InsertDocumentInline](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertDocumentInline-com.aspose.words.Document-int-com.aspose.words.ImportFormatOptions). <sup>23.10</sup>
- Možnost přístupu a úpravy vlastností stylu byla přidána zavedením nové vlastnosti [Locked](https://reference.aspose.com/words/java/com.aspose.words/style/#getLocked). <sup>23.10</sup>
- K metodám třídy [CompositeNode](https://reference.aspose.com/words/java/com.aspose.words/compositenode/) byl přidán obecný parametr typu. <sup>23.10</sup>
- Způsob, jak kontrolovat, kdy by měla být určitá revize přijata/odmítnuta nebo ne, byl implementován pomocí metod [Accept](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#accept-com.aspose.words.IRevisionCriteria) a [Reject](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#reject-com.aspose.words.IRevisionCriteria). Toto vylepšení poskytuje uživatelům jemnější kontrolu nad procesem revize. <sup>23.11</sup>
- Možnost zapsat všechny části dokumentu do stejného listu XLSX byla poskytnuta prostřednictvím nového typu výčtu [XlsxSectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsectionmode/) a nové vlastnosti [SectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/#getSectionMode). <sup>23.11</sup>
- Byla zavedena podpora pro WebP image. Upozorňujeme, že tato funkce je k dispozici pouze pro .NetStandart a .NET6+ verze. <sup>23.12</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words pro Java 23.9 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-9-release-notes/).

Další informace o [Aspose.Words Pro Java 23.10 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-10-release-notes/).

Další informace o [Aspose.Words Pro Java 23.11 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-11-release-notes/).

Další informace o [Aspose.Words Pro Java 23.12 Poznámky K Vydání](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-12-release-notes/).

{{% /alert %}}

## Vidět

{{% alert color="primary" %}}

Tato stránka obsahuje nejnovější zprávy o vydání za poslední 2 let. Podrobnosti o dřívějších verzích najdete v [Poznámky K Vydání"](https://releases.aspose.com/words/java/release-notes/) stránky v příslušných sekcích.

{{% /alert %}}
