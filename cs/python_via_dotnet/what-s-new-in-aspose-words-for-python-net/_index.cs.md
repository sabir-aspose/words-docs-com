---
title: Co je nového
second_title: Aspose.Words pro Python via .NET
articleTitle: Co je nového v Aspose.Words pro Python via .NET
linktitle: Co je nového v Aspose.Words pro Python via .NET
type: docs
description: "Aspose.Words pro Python via .NET rozšiřuje a zvyšuje denně. Na této stránce se můžete dozvědět o obrovských a nejzajímavějších vlastnostech produktu."
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-04-16-07-02-05
---

Tato stránka popisuje nejzajímavější nové funkce Aspose.Words představené v posledních verzích.

## Aspose.Words Pro Python přes .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 zavádí kontrolu gramatiky pomocí AI a vylepšuje ukládání dokumentů pomocí pokročilých možností pro formáty HTML, SVG a Markdown.

Aspose.Words 25.2 zavádí shrnutí textu pomocí modelů Anthropic AI, přidává podporu formátu MsWorks, vylepšuje typografické ovládání a zlepšuje strukturu a zpracování seznamu PDF.

Aspose.Words 25.3 vylepšuje kontrolu gramatiky a výběr písma pomocí AI s vlastností UpdateAmbiguousTextFont a také vylepšuje export příloh PDF.

Aspose.Words 25.4 zavádí podporu pro nové velikosti papíru, umožňuje pokročilé řízení exportu HTML a zlepšuje manipulaci s vodoznakem.

### AI - poháněné funkce

#### Kontrola Gramatiky AI

* Schopnost kontrolovat gramatiku poskytnutého dokumentu pomocí OpenAI generativních modelů byla zavedena přidáním nové metody [check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/). <sup>25.1</sup>
* Funkce kontroly gramatiky založená na AI byla aktualizována tak, aby podporovala všechny modely dostupné ve výčtu [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Shrnutí Pomocí Anthropic Generativních Jazykových Modelů <sup>25.2</sup>

Shrnutí textu pomocí Anthropic generativních jazykových modelů bylo povoleno zavedením nové veřejné třídy [AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/).

### Podporované Formáty <sup>25.2</sup>

Od verze 25.2 byla přidána kompatibilita s novým formátem načítání MsWorks pro pracovní dokumenty Microsoft.

### Převod, načítání a ukládání dokumentů

#### Vylepšené ukládání do formátů HTML a SVG <sup>25.1</sup>

Ukládání do formátů HTML a SVG bylo vylepšeno přidáním vlastností **id_prefix** a **remove_java_script_from_links** do tříd [HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/) a [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/).

#### Nastavte rozlišení obrazu a výstupní režim OfficeMath při ukládání do Markdown <sup>25.1</sup>

* Do třídy [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) byla přidána nová možnost [image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/) pro nastavení rozlišení obrazu.
* Do třídy [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) byla přidána nová volba [office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/) a výčet [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/) pro nastavení výstupního režimu OfficeMath.

### Vykreslování

#### Vylepšené Typografické Ovládání <sup>25.2</sup>

Vlastnost [number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/) byla přidána pro lepší typografické ovládání.

#### Ovládání výběru písma pro nejednoznačné znaky <sup>25.3</sup>

Do třídy [SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/) byla přidána nová veřejná vlastnost [update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/), která řídí výběr písma podle použitého znakového kódu.

#### Možnosti Velikosti Papíru <sup>25.4</sup>

Schopnost používat JIS B4 a JIS B5 velikosti papíru byla zavedena přidáním nových hodnot do výčtu [PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/).

#### HTML Výstupní Řízení <sup>25.4</sup>

Možnost odebrat JavaScript z hypertextového odkazu URLs během exportu HTML byla zavedena přidáním vlastnosti [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/).

### Jiný

* Logická struktura PDF byla vylepšena podporou polí TOA, BIBLIOGRAPHY a INDEX. <sup>25.2</sup>
* Pro lepší zpracování seznamu byla zavedena metoda [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate). <sup>25.2</sup>
* Byla přidána nová vlastnost [attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/), která nahradí **EmbedAttachments** a zlepší export příloh PDF. Do výčtu [PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/) byly také přidány nové hodnoty, které podporují přílohy verze PDF/A. Kromě toho jsou přílohy nyní podporovány šifrováním. <sup>25.3</sup>
* Možnost nastavit vodoznak obrázku ze streamu byla zavedena přidáním nového přetížení do metody [SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions). <sup>25.4</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words pro Python via .NET 25.1 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 25.2 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 25.3 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 25.4 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words pro Python přes .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 zavádí group shape vkládání a StructuredDocumentTag vkládání pomocí DocumentBuilder, vylepšuje Vykreslování radiálního grafu s odstupňováním, vylepšuje digitální podpisy s podporou XAdES-EPES, přidává Markdown rozpoznávání podtržení a poskytuje přístup k oddělovačům poznámek pod čarou/vysvětlivek.

Aspose.Words 24.10 zavádí vylepšenou podporu řízení ActiveX s vytvářením CommandButton, novým ovládáním viditelnosti tvarů, schopností group shapes, vylepšeným exportem Markdown pro tabulky, formátováním grafů pro grafy Pie a Doughnut, lepší manipulací s kódováním Big5 a podporou zastaralých tchajwanských písem.

Aspose.Words 24.11 představuje souhrn dokumentů poháněný AI, vylepšené možnosti Vykreslování, vylepšený přístup k vlastnostem dokumentu a ActiveX Ovládání titulků.

Aspose.Words 24.12 zavádí přizpůsobitelné umístění datových štítků, překlad textu pomocí Google AI a vylepšené nové třídy zpracování LowCode.

### AI - poháněné funkce

#### Shrnutí dokumentu pomocí OpenAI a Google <sup>24.11</sup>

Podpora sumarizace dokumentů pomocí generativních jazykových modelů **OpenAI** a **Google** byla integrována přidáním jmenného prostoru [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) s jeho veřejnými členy.

#### Překlad textu pomocí generativních jazykových modelů Google <sup>24.12</sup>

Schopnost překládat text pomocí generativních jazykových modelů Google byla implementována v Aspose.Words přidáním metody [translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/) a výčtu [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) do oboru názvů [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Nové LowCode třídy jako [Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) atd. byl představen a nabízí sadu metod, které vytvářejí dokonalou rovnováhu mezi jednoduchostí a flexibilitou pro zpracování dokumentů.

### Vykreslování a tisk

#### Promoce na radiálních grafech <sup>24.9</sup>

Bylo implementováno Vykreslování promocí na radiálních grafech.

#### CommandButton ActiveX ovládací prvky <sup>24.10</sup>

Schopnost vytvářet ovládací prvky CommandButton ActiveX byla zavedena přidáním nové veřejné metody [insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/) a nové veřejné třídy [Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/).

#### Kontrola Viditelnosti Tvaru <sup>24.10</sup>

Byla přidána nová veřejná vlastnost [hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/) pro řízení viditelnosti obrazců.

#### Změny v grafech Pie a Doughnut <sup>24.10</sup>

Do grafů format Pie a Doughnut bylo přidáno několik nových veřejných vlastností.

#### Řízení Vykreslování PDF výběrový formulář ohraničení polí <sup>24.11</sup>

Byla implementována nová možnost pro řízení Vykreslování okrajů polí PDF výběrového formuláře přidáním nové veřejné volby [render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/).

#### Získejte a nastavte kódy formátu pro data grafu <sup>24.11</sup>

Schopnost získat a nastavit kódy formátu pro data grafu byla přidána implementací vlastnosti [format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/) do tříd [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/) a [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/).

#### Vykreslení Histogramových grafů s přihrádkami a štítky <sup>24.11</sup>

Vykreslování grafu histogramu bylo vylepšeno umožněním zadaného počtu přihrádek a štítků.

#### Přizpůsobení umístění datových štítků <sup>24.12</sup>

Možnost přizpůsobit umístění popisků dat byla přidána zavedením nových vlastností tříd TH [ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/) a [ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Převod, načítání a ukládání dokumentů

#### Při načítání souborů Markdown podtrhněte formátování <sup>24.9</sup>

Možnost rozpoznat formátování podtržení při načítání dokumentů Markdown byla začleněna přidáním nové veřejné vlastnosti [import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/).

#### Export tabulek jako HTML při ukládání do Markdown <sup>24.10</sup>

Možnost exportovat tabulky jako HTML při ukládání dokumentů do formátu Markdown byla implementována přidáním nové veřejné vlastnosti [export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/) a výčtu [MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/).

#### Export PDF s aktualizovanou logickou strukturou <sup>24.11</sup>

Export PDF byl vylepšen zahrnutím vlastností názvu tabulky jako názvů prvků logické struktury PDF.

### Digitální Podpisy

#### Podepisujte dokumenty XAdES-EPES <sup>24.9</sup>

Schopnost podepisovat dokumenty s podpisy XAdES-EPES úrovně XML-DSig byla zavedena přidáním nového veřejného majetku [xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/) a nového veřejného výčtu [XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/).

### Jiný

* Do group shapes byla přidána nová veřejná metoda [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/). <sup>24.9</sup>
* Byla přidána nová veřejná metoda [insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/) pro vložení **StructuredDocumentTags** do dokumentu. <sup>24.9</sup>
* Veřejný přístup k oddělovačům poznámek pod čarou/vysvětlivek byl poskytnut přidáním několika veřejných tříd a vlastností. <sup>24.9</sup>
* Schopnost seskupovat jednotlivé tvary group shapes dohromady a přímo seskupovat oba tvary a group shapes byla zavedena přidáním metody [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist). <sup>24.10</sup>
* Zpracování kódování Big5 pro TrueType CMAP tabulky bylo vylepšeno. <sup>24.10</sup>
* Byla rozšířena podpora zastaralých tchajwanských písem. <sup>24.10</sup>
* Pro přístup k rozšířeným vlastnostem dokumentu byly do třídy [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/) přidány vlastnosti pouze pro čtení. <sup>24.11</sup>
* Nastavení titulků pro ovládací prvky ActiveX bylo povoleno přidáním nového veřejného nastavovače do vlastnosti [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words pro Python via .NET 24.9 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 24.10 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 24.11 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 24.12 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words pro Python přes .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 rozšiřuje možnosti sestav, zlepšuje možnosti Vykreslování a rozšiřuje některé další možnosti.

Aspose.Words 24.6 vylepšuje možnosti Vykreslování, vylepšuje funkce vyhledávání a porovnávání a rozšiřuje několik dalších funkcí.

Aspose.Words 24.7 mění způsob práce s ActiveX, rozšiřuje možnosti Vykreslování a exportuje do formátů Markdown a XLSX.

Aspose.Words 24.8 vylepšuje přizpůsobení grafu s přesnou kontrolou nad popisky os, rozšiřuje správu písem, zlepšuje manipulaci se strukturou dokumentů a přidává nové možnosti pro export HTML/XAML, funkčnost PDF, převod dokumentů a digitální podpisy.

### Podporované Formáty

Počínaje verzí 24.7 je podporován export do PDF/UA-2, aby byla zajištěna dostupnost pro uživatele se zdravotním postižením.

### Vykreslování a tisk

#### Změny v grafech, tvarech a DrawingML <sup>24.5</sup>

* DrawingML Vykreslování efektů pro grafiku SVG, Rozšíření předchozí funkce omezené na obrázky, bylo implementováno.
* Podpora pro vytváření kombinovaných grafů a úpravy vlastností, jako je šířka mezery, překrytí a stupnice bublin v rámci skupin sérií, byla zavedena přidáním tříd [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/) a [ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/) a vlastnosti [series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/).
* Funkce pro manipulaci s efektem tvarů SoftEdge byla implementována přidáním třídy [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/).
* Možnost upravit upravit hodnoty tvarů byla implementována přidáním veřejných tříd **AdjustmentCollection** a **Adjustment** a vlastnosti [adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/).

#### Změny v grafech, tvarech a kreslení <sup>24.6</sup>

- Byly vylepšeny možnosti mapování. Nyní můžete vytvořit širší škálu grafů, včetně *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* grafy, *Box & Whisker* grafy, *Waterfalls* a *Funnels*. To vám umožní vizualizovat vaše data rozmanitějším a informativnějším způsobem.
- Ovládání barev pro formátování stínů bylo vylepšeno. Přesnější kontrolu nad vzhledem dokumentů můžete získat přístupem k barvám stínů.
- Zvýšení výkonu pro vykreslování pozadí bylo vylepšeno. Díky nativní technologii obkladů můžete výrazně urychlit vykreslování pozadí obsahujících malé prvky.
- Byly přidány realistické přechody pro tvary. Nyní můžete vytvářet DML tvary s nelineárními přechody, napodobující vizuální styl Microsoft Word pro vyleštěnější vzhled.

#### Přizpůsobení Štítku Dat Grafu <sup>24.7</sup>

Byla přidána možnost přizpůsobit štítky dat grafu, jako jsou **Orientation** a **Rotation**.

#### Vlastní styl čísel pro úrovně seznamu <sup>24.7</sup>

Byl přidán setr pro veřejný majetek [custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/). Nyní můžete definovat vlastní styl čísel pro úrovně seznamu.

#### Změny v práci s ActiveX <sup>24.7</sup>

- Vlastnosti objektů ActiveX lze nyní upravit, což vám dává větší kontrolu nad jejich chováním.
- Byla přidána možnost upravit hodnotu ovládacího prvku přepínače ActiveX, aby byla povolena dynamická interakce.
- Byla přidána možnost přepnout ActiveX checkbox na "zaškrtnuto" nebo "nezaškrtnuto".

#### Kontrola nad osou grafu klíště popisky orientace a rotace <sup>24.8</sup>

Pro pohodlnější přizpůsobení grafu byla přidána přesná kontrola nad orientací a rotací štítků klíštěte osy grafu – třída [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) byla rozšířena o nové vlastnosti [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) a [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/).

#### Nahrazení zpětného lomítka znakem jenu <sup>24.8</sup>

Zpětně kompatibilní HTML a XAML export pro nahrazení znaku zpětného lomítka znakem jenu byl vylepšen. K dosažení tohoto cíle byla vlastnost **replace_backslash_with_yen_sign** přidána do tříd [HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/) a [XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/).

#### Použití značek SDT jako názvů polí formuláře při exportu do PDF <sup>24.8</sup>

PDF export s podporou použití značek SDT jako názvů polí formuláře byl vylepšen přidáním nové vlastnosti [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) do třídy [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/).

### Převod, načítání a ukládání dokumentů

#### Export odkazů do formátu Markdown <sup>24.7</sup>

Schopnost řídit export odkazů ve formátu Markdown byla přidána implementací vlastnosti [link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/).

#### LowCode 24.8 <sup>24.8</sup>

Byla zavedena nová třída [LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/), navržená tak, aby poskytovala sadu metod pro převod různých typů dokumentů pomocí jediného řádku kódu.

### Hledat a porovnávat

#### Pokročilé Možnosti Porovnání <sup>24.6</sup>

Byla přidána možnost zefektivnit pracovní postupy analýzy dat s vylepšenou funkcí porovnávání. To zahrnuje novou možnost [ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/) a přepracované rozhraní pro pokročilá srovnání.

### Jiný

* Funkce pro odstranění prázdných stránek z dokumentu byla implementována přidáním metody [remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/). <sup>24.5</sup>
* Možnost zkontrolovat přítomnost Maker VBA bez načtení dokumentu byla poskytnuta přidáním vlastnosti [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/). <sup>24.5</sup>
* Nyní je podporováno udržování číslování zdrojů při vkládání dokumentu pomocí LINQ Reporting Engine. <sup>24.5</sup>
* Byla přidána nová vlastnost [date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/) - poskytuje přesnější časové razítko pro Komentáře, zlepšuje organizaci a sledovatelnost. <sup>24.6</sup>
* Formát datetime je nyní automaticky detekován pro bezproblémový export do formátu XLSX. <sup>24.7</sup>
* Byla přidána veřejná vlastnost [is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/), která umožňuje ověřit, zda je projekt VBA chráněn. <sup>24.7</sup>
* Informace o Písmu byly rozšířeny o vlastnost **embedding_licensing_rights** přidanou do tříd [FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/) a [PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* Pro přesnější práci se strukturou dokumentu byl přidán způsob, jak efektivně vymazat záhlaví a zápatí sekcí při zachování vodoznaků. Chcete-li vymazat záhlaví a zápatí oddílů, použijte novou veřejnou metodu [clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default). <sup>24.8</sup>
* Bylo povoleno digitální podepisování dokumentů XPS pomocí [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/) – pro tento účel byla přidána nová vlastnost [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/). <sup>24.8</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words pro Python via .NET 24.5 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

Další informace o [Aspose.Words Pro Python via .NET 24.6 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 24.7 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 24.8 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words pro Python přes .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 zlepšuje zážitek ze správy barev tahů, vylepšuje objekty OLE a zavádí nový `Bibliography Sources` veřejný API.

Aspose.Words 24.2 rozšířené grafy API a Správa stylů. Tato verze Aspose.Words také zavedla schopnost specifikovat SvgSaveOptions během Vykreslování, flexibilnější ovládání načítání souborů Markdown a práci s referenčním textem pro poznámky pod čarou a vysvětlivky.

Aspose.Words 24.3 zavádí nový TIFF Reader / Writer a emulaci binárních rastrových operací pro WMF metasoubory. Aspose.Words 24.3 také pokračuje v rozšiřování grafů API.

Aspose.Words 24.4 vylepšuje ukládání formátů, některé možnosti Vykreslování a zlepšuje práci s digitálními podpisy.

### Podporované Formáty <sup>24.4</sup>

Moderní formát obrázku **WebP** je nyní podporován v Aspose.Words pro .NET Framework 4.6.2 vysoký. Nyní můžete číst a vkládat obrázky WebP do dokumentů a také ukládat obrázky ve formátu WebP.

Vezměte prosím na vědomí, že WebP je v současné době k dispozici pouze v .NET Standard a .NET Framework v4.6.2 a výše.

### Vykreslování a tisk

#### Ovládání Barev Tahu <sup>24.1</sup>

Třída [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) byla rozšířena o sadu nových veřejných vlastností souvisejících se správou barev tahů: [fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/) a [back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/), [fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/) a [back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### DrawingML Grafy API Rozšíření <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** se stále rozšiřuje.

#### Vložit písma deklarovaná v pravidlech @font-face <sup>24.4</sup>

Přidána možnost vkládat písma deklarovaná v pravidlech @font-face do definic písem výsledného dokumentu byla zavedena přidáním nové vlastnosti [support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/).

#### Práce s formátováním záře a odrazu <sup>24.4</sup>

Byla implementována schopnost pracovat s formátováním záře a odrazu pro kreslící objekt.

### Načítání a ukládání dokumentů

#### Zadejte SvgSaveOptions Během Vykreslování <sup>24.2</sup>

Schopnost specifikovat [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) během Vykreslování byla přidána pomocí [ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) a [OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) metody.

#### Při načítání souborů Markdown Zachovejte prázdné řádky <sup>24.2</sup>

Byla přidána možnost zachovat prázdné řádky při načítání souborů Markdown.

#### Nový TIFF Čtenář / Spisovatel <sup>24.3</sup>

Byl vyvinut nový TIFF reader / writer pro Aspose.Words. Aspose.Words pro .NET 24.3 přidána podpora pro čtení TIFF obrázků s JPEG a starými typy komprese JPEG a také výrazně zlepšila kvalitu operací čtení a zápisu.

### Jiný

* Schopnost upravit text ovládacího prvku `TextBox` OLE byla zavedena přidáním nové vlastnosti **Text** do nové třídy **TextBoxControl**. <sup>24.1</sup>
* Bibliografické zdroje veřejné API byly implementovány přidáním nového oboru názvů [Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/) s novými třídami a výčty a přidáním nové vlastnosti [bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/) do třídy [Document](https://reference.aspose.com/words/python-net/aspose.words/document/). <sup>24.1</sup>
* Do třídy [Style](https://reference.aspose.com/words/python-net/aspose.words/style/) byly přidány nové veřejné vlastnosti [priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/), [unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/) a [semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/) pro rozšířenou správu stylů. <sup>24.2</sup>
* Funkce pro načtení skutečného textu referenční značky pro poznámky pod čarou a vysvětlivky byla vylepšena vlastností [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/) a metodou [update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default). <sup>24.2</sup>
* Byla implementována emulace binárních rastrových operací pro metasoubory WMF. <sup>24.3</sup>
* Možnost definovat možnosti podpisu pro dokumenty v rámci **SaveOptions** byla povolena přidáním nové třídy [DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/) s novými veřejnými členy a přidáním nových vlastností do tříd [OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/) a [OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words pro Python via .NET 24.1 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 24.2 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 24.3 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 24.4 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words pro Python přes .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 rozšiřuje možnosti Vykreslování, emulaci Vykreslování metafile a markdown Možnosti uložení.

Aspose.Words 23.10 zlepšuje vykreslování, rozšiřuje možnosti načítání a ukládání dokumentů a umožňuje uživatelům sloučit dokumenty novými způsoby.

Aspose.Words 23.11 vylepšuje práci s revizemi, formátem XLSX a fonty na legendě grafu s dalšími možnostmi.

Aspose.Words 23.12 zavádí nové vlastnosti a výčty pro práci s PDF a OOXML dokumenty, stejně jako podporu pro WebP Obrázky.

### Vykreslování a tisk

#### Přizpůsobení názvů OS v grafech DrawingML <sup>23.9</sup>

Schopnost přizpůsobit názvy os v grafech DrawingML byla zavedena implementací nové veřejné třídy [ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/) a [title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/) vlastnost.

####  Určení svislé polohy písem v odstavci <sup>23.9</sup>

Nyní je možné definovat svislou polohu písem v odstavci pomocí nové veřejné vlastnosti [baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/) a Nového výčtu [BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/).

#### Ovládání Barev Popředí <sup>23.10</sup>

Schopnost načíst barvu popředí bez modifikátorů byla přidána do tříd [Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/) a [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) pomocí Vlastnosti **BaseForeColor**.

#### Rozšíření funkčnosti grafů <sup>23.10</sup>

Funkce tříd [ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/) a [ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/) byla rozšířena o nové metody a vlastnosti.

#### Automatické nastavení a přizpůsobení obrázku do tvaru <sup>23.10</sup>

Jednoduchý způsob, jak automaticky upravit a přizpůsobit obrázek do určitého tvaru, byl poskytnut pomocí nové metody [fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default).

#### Výchozí formátování písma pro DrawingML položky legendy grafu <sup>23.11</sup>

Možnost zadat výchozí formátování písma pro položky legendy DrawingML grafů byla přidána pomocí vlastnosti [font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/). Tato funkce usnadňuje efektivnější a konzistentnější vzhled prvků grafu a zlepšuje celkovou estetiku dokumentu.

#### Určete Rozložení stránky při otevírání PDF v Readeru <sup>23.12</sup>

Schopnost určit rozvržení stránky, které se má použít při otevírání dokumentu ve čtečce PDF, byla přidána zavedením nové vlastnosti [page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/) do třídy [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) a zavedením nového výčtu [PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/).

### Načítání a ukládání dokumentů

#### Zadání názvu složky pro vytvoření obrázku URIs v Markdown <sup>23.9</sup>

Třída [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) byla rozšířena o vlastnost [images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/), která umožňuje určit název složky použité ke konstrukci obrazu URIs zapsaného do dokumentu Markdown.

#### Zmenšit Velikost Výstupu PDF <sup>23.10</sup>

Byly implementovány různé optimalizace Vykreslování PDF pro zmenšení velikosti výstupu při použití nastavení [optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/).

#### Rozpoznání hypertextových odkazů při načítání dokumentů TXT <sup>23.10</sup>

Funkce rozpoznání hypertextových odkazů při načítání dokumentů TXT byla implementována přidáním nové vlastnosti [detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/).

### Jiný

- Byla implementována emulace Metafile rendering pro určení velikosti rasterizace, konkrétně pro WMF šířku pera a EMF šířku kosmetického pera. K dosažení tohoto cíle byla vlastnost **ScaleWmfFontsToMetafileSize** nahrazena vlastností [emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/) a byla přidána vlastnost [emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/). <sup>23.9</sup>
- Byla zavedena zjednodušená metoda pro vložení jednoho dokumentu do jiného dokumentu na aktuální pozici kurzoru pomocí metody [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions). <sup>23.10</sup>
- Možnost přístupu a úpravy vlastností stylu byla přidána zavedením nové vlastnosti [locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/). <sup>23.10</sup>
- K metodám třídy [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/) byl přidán obecný parametr typu. <sup>23.10</sup>
- Možnost zapsat všechny části dokumentu do stejného listu XLSX byla poskytnuta prostřednictvím nového typu výčtu [XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/) a nové vlastnosti [section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/). <sup>23.11</sup>
* Způsob, jak řídit, jak budou rozšíření formátu ZIP64 použita pro dokumenty OOXML, byl implementován prostřednictvím nové vlastnosti Zip64Mode třídy `OoxmlSaveOptions` a Nového výčtu Zip64Mode. <sup>23.12</sup>
* Byla zavedena podpora pro WebP image. Upozorňujeme, že tato funkce je k dispozici pouze pro .NetStandart a .NET6+ verze. <sup>23.12</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words pro Python via .NET 23.9 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 23.10 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 23.11 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

Další informace o [Aspose.Words Pro .NET 23.12 Poznámka](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words pro Python přes .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 zvyšuje schopnost pracovat s daty řady grafů a schopnost pracovat s ODT dokumenty, stejně jako zlepšit záhlaví/zápatí a jejich obtékání textu.

Aspose.Words 23.6 rozšiřuje možnosti Vykreslování, přidává nový formát exportu, vylepšuje LINQ reporting a LowCode nástroje.

Aspose.Words 23.7 vylepšuje možnosti vykazování, přidává nový formát exportu a zavádí změny v práci s tabulkami a digitálními podpisy.

Aspose.Words 23.8 rozšiřuje možnosti různých formátů, zlepšuje vykreslování a přidává nové možnosti pro práci s poli.

### Podporované Formáty

* Počínaje verzí 23.6 je možné uložit dokument ve formátu XLSX. Nyní můžete své dokumenty převést do formátu Excel. <sup>23.6</sup>

* Počínaje verzí 23.7 je možné uložit stránku dokumentu nebo tvar ve formátu EPS. <sup>23.7</sup>

### Nové Funkce Formátu

- Byla zavedena funkce automatického generování obsahu (TOC) Pro MOBI dokumenty. <sup>23.8</sup>
- Konstruktor [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) byl rozšířen o [PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions). <sup>23.8</sup>
- Bylo implementováno tvarování vertikálního textu pro metasoubory EMF. <sup>23.8</sup>

### Vykreslování

#### Získejte A Upravte Data řady grafů <sup>23.5</sup>

Funkce pro získání a úpravu dat řady grafů byla poskytnuta přidáním:

- nové třídy: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- nové typy výčtu: [ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### Podpora pokročilé typografie <sup>23.6</sup>

Byla přidána podpora pokročilé typografie v WMF, EMF a EMF+ Vykreslování.

#### Barevný obsah na stránce <sup>23.6</sup>

Byla přidána veřejná vlastnost [PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/) označující, zda je stránka barevná nebo ne.

#### Formátování popisků dat grafu <sup>23.6</sup>

Byla implementována možnost nastavit formátování výplně, tahu a popisku pro popisky dat grafu.

### Mail Merge a podávání zpráv

#### Dynamic HTML vložení pro LINQ Reporting Engine <sup>23.6</sup>

Byl přidán nový způsob dynamického vkládání HTML pro LINQ Reporting Engine.

#### Mustache Podpora Značek <sup>23.7</sup>

Značky Mustache jsou nyní podporovány v metodách [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/) a [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/).

#### Určení velikosti vykreslených obrázků <sup>23.8</sup>

Byla zavedena nová veřejná vlastnost [image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/) pro určení velikosti vykreslených obrázků v pixelu.

#### Zachovat mezery pro hodnoty řetězce JSON - LINQ <sup>23.8</sup>

Do LINQ Reporting Engine byla přidána možnost pro zachování mezer pro hodnoty řetězce JSON.

### LowCode <sup>23.6</sup>

Byly přidány nové metody LowCode určené ke sloučení různých typů dokumentů do jednoho výstupního dokumentu.

### Jiný

- Byla implementována podpora zalamování textu v záhlaví/zápatí. <sup>23.5</sup>
- Schopnost odstranit digitální podpisy z dokumentů ODT byla přidána metodou [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str). <sup>23.5</sup>
- Byla přidána veřejná vlastnost [phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/) pro získání základního a rubínového textu fonetického průvodce [Run](https://reference.aspose.com/words/python-net/aspose.words/run/). <sup>23.5</sup>
- Schopnost načíst hodnotu digitálního podpisu z digitálně podepsaného dokumentu jako bajtové pole byla přidána zavedením nové vlastnosti [signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/). <sup>23.7</sup>
- Třídy [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/) a [Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/) byly rozšířeny o nové veřejné členy– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), a [Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/). <sup>23.7</sup>

{{% alert color="primary" %}}

Další informace o [Aspose.Words pro Python via .NET 23.5 Poznámky K Vydání](/words/python-net/aspose-words-for-python-via-dotnet-23-5-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 23.6 Poznámky K Vydání](/words/python-net/aspose-words-for-python-via-dotnet-23-6-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 23.7 Poznámky K Vydání](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

Další informace o [Aspose.Words pro Python via .NET 23.8 Poznámky K Vydání](/words/python-net/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## Vidět

{{% alert color="primary" %}}

Tato stránka obsahuje nejnovější zprávy o vydání za poslední 2 let. Podrobnosti o dřívějších verzích najdete v [Poznámky K Vydání"](https://releases.aspose.com/words/python/release-notes/) stránky v příslušných sekcích.

{{% /alert %}}
