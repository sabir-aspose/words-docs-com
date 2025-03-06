---
title: Co nowego
second_title: Aspose.Words dla Python via .NET
articleTitle: Co nowego w Aspose.Words dla Python via .NET
linktitle: Co nowego w Aspose.Words dla Python via .NET
type: docs
description: "Aspose.Words dla Python via .NET rozszerza się i zwiększa codziennie. Na tej stronie możesz dowiedzieć się o ogromnych i najciekawszych funkcjach produktu."
weight: 10
url: /pl/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-02-17-18-02-05
---

Ta strona opisuje najciekawsze nowe funkcje Aspose.Words wprowadzone w ostatnich wydaniach.

## Aspose.Words dla Python via .NET 25.1, 25.2

Aspose.Words 25.1 wprowadza sprawdzanie gramatyki z napędem AI i ulepsza zapisywanie dokumentów dzięki zaawansowanym opcjom formatów HTML, SVG i Markdown.

Aspose.Words 25.2 wprowadza podsumowanie tekstu za pomocą modeli antropicznych AI, dodaje obsługę formatu MsWorks, poprawia kontrolę typograficzną oraz poprawia strukturę i obsługę list PDF.

### AI - funkcje zasilane

#### Sprawdzanie Gramatyki Dokumentu AI <sup>25.1</sup>

Możliwość sprawdzenia gramatyki dostarczonego dokumentu przy użyciu OpenAI modeli generatywnych została wprowadzona poprzez dodanie nowej metody [check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/).

#### Podsumowanie Za Pomocą Antropicznych Generatywnych Modeli Językowych <sup>25.2</sup>

Podsumowanie tekstu przy użyciu antropicznych generatywnych modeli językowych zostało włączone poprzez wprowadzenie nowej klasy publicznej [AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/).

### Obsługiwane Formaty <sup>25.2</sup>

Począwszy od wersji 25.2, dodano zgodność z nowym formatem ładowania MsWorks dla Microsoft works documents.

### Konwertowanie, ładowanie i zapisywanie dokumentów

#### Ulepszone zapisywanie w formatach HTML i SVG <sup>25.1</sup>

Zapisywanie w formatach HTML i SVG zostało ulepszone poprzez dodanie właściwości **id_prefix** i **remove_java_script_from_links** do klas [HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/) i [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/).

#### Ustaw rozdzielczość obrazu i tryb wyjścia OfficeMath podczas zapisywania do Markdown <sup>25.1</sup>

* Nowa opcja [image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/) została dodana do klasy [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/), aby ustawić rozdzielczość obrazu.
* Nowa opcja [office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/) i [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/) wyliczenie zostały dodane do klasy [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/), aby ustawić OfficeMath Tryb wyjściowy.

### Rendering

#### Ulepszona Kontrola Typograficzna <sup>25.2</sup>

Właściwość [number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/) została dodana w celu poprawy kontroli typograficznej.

### Inne

* PDF struktura logiczna została ulepszona dzięki obsłudze pól TOA, BIBLIOGRAPHY i INDEX. <sup>25.2</sup>
* Metoda [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate) została wprowadzona w celu poprawy obsługi listy. <sup>25.2</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla Python via .NET 25.1 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-1-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 25.2 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-2-release-notes/).

{{% /alert %}}

## Aspose.Words dla Python przez .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 wprowadza group shape wstawianie i StructuredDocumentTag wstawianie przez DocumentBuilder, poprawia renderowanie Wykresów promieniowych z podziałką, poprawia podpisy cyfrowe z obsługą XAdES-EPES, dodaje rozpoznawanie podkreśleń Markdown i zapewnia dostęp do separatorów przypisów/przypisów końcowych.

Aspose.Words 24.10 wprowadza ulepszoną obsługę kontroli ActiveX z tworzeniem CommandButton, nową kontrolą widoczności kształtu, możliwością group shapes, ulepszonym eksportem Markdown dla tabel, formatowaniem wykresów dla Wykresów Pie i Doughnut, lepszą obsługą kodowania Big5 i obsługą przestarzałych czcionek tajwańskich.

Aspose.Words 24.11 wprowadza AI-powered podsumowania dokumentu, ulepszone opcje renderowania, lepszy dostęp do Właściwości dokumentu i ActiveX napisów kontrolnych.

Aspose.Words 24.12 wprowadza konfigurowalne umieszczanie etykiet danych, tłumaczenie tekstu oparte na Google AI i ulepszone nowe klasy przetwarzania LowCode.

### AI - funkcje zasilane

#### Podsumowanie dokumentów za pomocą OpenAI i Google <sup>24.11</sup>

Obsługa podsumowania dokumentów przy użyciu generatywnych modeli językowych **OpenAI** i **Google** została zintegrowana poprzez dodanie przestrzeni nazw [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) wraz z jej publicznymi członkami.

#### Tłumaczenie tekstu przy użyciu generatywnych modeli językowych Google <sup>24.12</sup>

Możliwość tłumaczenia tekstu za pomocą generatywnych modeli językowych Google została zaimplementowana w Aspose.Words poprzez dodanie metody [translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/) i wyliczenia [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) do przestrzeni nazw [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Nowe LowCode klasy, takie jak[Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) itp. został wprowadzony, oferując zestaw metod, które zapewniają idealną równowagę między prostotą a elastycznością przetwarzania dokumentów.

### Renderowanie i drukowanie

#### Podziałka na wykresach promieniowych <sup>24.9</sup>

Zaimplementowano renderowanie podziałek na wykresach promieniowych.

#### CommandButton Formanty ActiveX <sup>24.10</sup>

Możliwość tworzenia CommandButton formantów ActiveX została wprowadzona przez dodanie nowej metody publicznej [insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/) i nowej klasy publicznej [Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/).

#### Kontrola Widoczności Kształtu <sup>24.10</sup>

Dodano nową właściwość publiczną [hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/), aby kontrolować widoczność kształtów.

#### Zmiany na wykresach Pie i Doughnut <sup>24.10</sup>

Dodano kilka nowych właściwości publicznych do Wykresów format Pie i Doughnut.

#### Kontroluj renderowanie granic pól formularza wyboru PDF <sup>24.11</sup>

Nowa opcja kontrolowania renderowania granic pól formularza wyboru PDF została zaimplementowana przez dodanie nowej opcji publicznej [render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/).

#### Pobierz i ustaw kody formatu dla danych wykresu <sup>24.11</sup>

Możliwość pobierania i ustawiania kodów formatu dla danych wykresu została dodana poprzez implementację właściwości [format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/) w klasach [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/) i [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/).

#### Renderuj wykresy histogramu z pojemnikami i etykietami <sup>24.11</sup>

Renderowanie wykresu histogramu zostało ulepszone, umożliwiając określoną liczbę pojemników i etykiet.

#### Dostosuj rozmieszczenie etykiet danych <sup>24.12</sup>

Dodano możliwość dostosowania rozmieszczenia etykiet danych poprzez wprowadzenie nowych właściwości do klas th [ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/) i [ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Konwertowanie, ładowanie i zapisywanie dokumentów

#### Podkreśl formatowanie podczas ładowania plików Markdown <sup>24.9</sup>

Opcja rozpoznawania formatowania podkreślenia podczas ładowania dokumentów Markdown została włączona przez dodanie nowej własności publicznej [import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/).

#### Eksportowanie tabel jako HTML podczas zapisywania do Markdown <sup>24.10</sup>

Opcja eksportu tabel jako HTML podczas zapisywania dokumentów do formatu Markdown została zaimplementowana przez dodanie nowej własności publicznej [export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/) i wyliczenia [MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/).

#### Eksportuj PDF ze zaktualizowaną strukturą logiczną <sup>24.11</sup>

PDF eksport został wzmocniony przez włączenie właściwości tytułu tabeli jako PDF tytułów elementów struktury logicznej.

### Podpisy Cyfrowe

#### Podpisuj dokumenty za pomocą XAdES-EPES <sup>24.9</sup>

Możliwość podpisywania dokumentów z podpisami XAdES-EPES poziomu XML-DSig została wprowadzona przez dodanie nowej własności publicznej [xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/) i nowego wyliczenia publicznego [XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/).

### Inne

* Nowa metoda publiczna [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/) została dodana do group shapes. <sup>24.9</sup>
* Dodano nową metodę publiczną [insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/), aby wstawić **StructuredDocumentTags** do dokumentu. <sup>24.9</sup>
* Publiczny dostęp do separatorów przypisów / przypisów końcowych został zapewniony przez dodanie kilku publicznych klas i właściwości. <sup>24.9</sup>
* Możliwość grupowania poszczególnych kształtów, group shapes Razem i bezpośredniego grupowania zarówno kształtów, jak i group shapes została wprowadzona przez dodanie metody [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist). <sup>24.10</sup>
* Poprawiono obsługę kodowania Big5 dla tabel CMAP TrueType. <sup>24.10</sup>
* Ulepszono obsługę przestarzałych czcionek tajwańskich. <sup>24.10</sup>
* Aby uzyskać dostęp do rozszerzonych właściwości dokumentu, właściwości tylko do odczytu zostały dodane do klasy [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/). <sup>24.11</sup>
* Ustawianie napisów dla formantów ActiveX zostało włączone przez dodanie nowego publicznego setera do właściwości [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.9 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.10 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.11 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.12 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words dla Python przez .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 rozszerza opcje zestawów, poprawia możliwości renderowania i rozszerza niektóre inne opcje.

Aspose.Words 24.6 poprawia opcje renderowania, poprawia funkcje wyszukiwania i porównywania oraz rozszerza kilka innych funkcji.

Aspose.Words 24.7 zmienia sposób pracy z ActiveX, rozszerza możliwości renderowania, a także eksportuje do formatów Markdown i XLSX.

Aspose.Words 24.8 usprawnia dostosowywanie wykresów dzięki precyzyjnej kontroli nad etykietami osi, rozszerza zarządzanie czcionkami, poprawia obsługę struktury dokumentu i dodaje nowe możliwości eksportu HTML/XAML, funkcjonalności PDF, konwersji dokumentów i podpisów cyfrowych.

### Obsługiwane Formaty

Począwszy od wersji 24.7, eksport do PDF/UA-2 jest obsługiwany w celu zapewnienia dostępności dla użytkowników niepełnosprawnych.

### Renderowanie i drukowanie

#### Zmiany w wykresach, kształtach i DrawingML <sup>24.5</sup>

* Zaimplementowano renderowanie efektów DrawingML dla Grafiki SVG, rozszerzając poprzednią funkcjonalność ograniczoną do obrazów.
* Obsługa tworzenia wykresów kombi i dostosowywania właściwości, takich jak szerokość szczeliny, nakładanie się i skala bąbelków w grupach serii, została wprowadzona przez dodanie klas [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/) i [ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/) oraz właściwości [series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/).
* Funkcjonalność manipulowania efektem SoftEdge kształtów została zaimplementowana przez dodanie klasy [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/).
* Możliwość modyfikowania dostosowywania wartości kształtów została zaimplementowana przez dodanie klas publicznych **AdjustmentCollection** i **Adjustment** oraz właściwości [adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/).

#### Zmiany w wykresach, kształtach i rysunkach <sup>24.6</sup>

- Zwiększono możliwości tworzenia wykresów. Możesz teraz tworzyć szerszą gamę Wykresów, w tym*Treemaps*, *Sunbursts*, *Histograms*, *Pareto* wykresy, *Box & Whisker* wykresy, *Waterfalls* i *Funnels*. Pozwala to na wizualizację danych w bardziej zróżnicowany i informacyjny sposób.
- Poprawiono kontrolę koloru dla formatowania cienia. Możesz uzyskać bardziej precyzyjną kontrolę nad wyglądem dokumentów, uzyskując dostęp do kolorów cieni.
- Poprawiono zwiększenie wydajności renderowania w tle. Możesz znacznie przyspieszyć renderowanie tła zawierającego małe elementy dzięki natywnej technologii układania płytek.
- Dodano realistyczne gradienty kształtów. Możesz teraz tworzyć DML kształty z nieliniowymi gradientami, naśladując styl wizualny Microsoft Word, aby uzyskać bardziej dopracowany wygląd.

#### Dostosowanie Etykiety Danych Wykresu <sup>24.7</sup>

Dodano możliwość dostosowywania etykiet danych wykresów, takich jak **Orientation** i **Rotation**.

#### Niestandardowa Stylizacja numerów dla poziomów listy <sup>24.7</sup>

Dodano seter dla własności publicznej [custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/). Możesz teraz zdefiniować niestandardową stylizację numerów dla poziomów listy.

#### Zmiany w pracy z ActiveX <sup>24.7</sup>

- Właściwości obiektów ActiveX można teraz modyfikować, co daje większą kontrolę nad ich zachowaniem.
- Dodano możliwość modyfikacji wartości kontrolki ActiveX przycisku radiowego w celu umożliwienia dynamicznej interakcji.
- Dodano możliwość przełączania ActiveX checkbox Na "zaznaczone" lub "niezaznaczone".

#### Kontrola nad osią wykresu zaznacz etykiety Orientacja i obrót <sup>24.8</sup>

Dodano precyzyjną kontrolę nad orientacją i obrotem etykiet znaczników osi wykresu w celu wygodniejszego dostosowywania wykresu - klasa [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) została rozszerzona o nowe właściwości [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) i [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/).

#### Zastąpienie ukośnika odwrotnego znakiem Jena <sup>24.8</sup>

Wstecznie kompatybilny eksport HTML i XAML do zastąpienia znaku ukośnika odwrotnego znakiem Jena został ulepszony. Aby to osiągnąć, właściwość **replace_backslash_with_yen_sign** została dodana do klas [HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/) i [XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/).

#### Używanie znaczników SDT jako nazw pól formularza podczas eksportowania do PDF <sup>24.8</sup>

PDF eksport z obsługą używania znaczników SDT jako nazw pól formularza został ulepszony poprzez dodanie nowej właściwości [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) do klasy [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/).

### Konwertowanie, ładowanie i zapisywanie dokumentów

#### Eksportowanie linków do formatu Markdown <sup>24.7</sup>

Możliwość kontrolowania eksportu linków w formacie Markdown została dodana poprzez implementację właściwości [link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/).

#### LowCode 24.8 <sup>24.8</sup>

Wprowadzono nową klasę [LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/), zaprojektowaną w celu zapewnienia zestawu metod konwersji różnych typów dokumentów za pomocą jednego wiersza kodu.

### Wyszukaj i porównaj

#### Zaawansowane Opcje Porównania <sup>24.6</sup>

Dodano możliwość usprawnienia przepływów pracy analizy danych dzięki ulepszonej funkcji porównywania. Obejmuje to nową opcję [ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/) i przeprojektowany interfejs do zaawansowanych porównań.

### Inne

* Funkcja eliminacji pustych stron z dokumentu została zaimplementowana przez dodanie metody [remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/). <sup>24.5</sup>
* Możliwość sprawdzenia obecności makr VBA bez ładowania dokumentu została zapewniona przez dodanie właściwości [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/). <sup>24.5</sup>
* Utrzymywanie numeracji źródeł podczas wstawiania dokumentu przy użyciu mechanizmu raportowania LINQ jest teraz obsługiwane. <sup>24.5</sup>
* Dodano nową właściwość [date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/) - zapewnia to dokładniejszy znacznik czasu dla komentarzy, poprawiając organizację i identyfikowalność. <sup>24.6</sup>
* Format datetime jest teraz automatycznie wykrywany w celu bezproblemowego eksportu do formatu XLSX. <sup>24.7</sup>
* Dodano własność publiczną [is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/), która pozwala sprawdzić, czy projekt VBA jest chroniony. <sup>24.7</sup>
* Informacje o czcionkach zostały rozszerzone o Właściwość **embedding_licensing_rights** dodaną do klas [FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/) i [PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* Dodano sposób efektywnego czyszczenia nagłówków i stopek sekcji przy jednoczesnym zachowaniu znaków wodnych, aby dokładniej pracować ze strukturą dokumentu. Aby wyczyścić nagłówki i stopki sekcji, użyj nowej metody publicznej [clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default). <sup>24.8</sup>
* Włączono cyfrowe podpisywanie dokumentów XPS przy użyciu [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/) – w tym celu dodano nową właściwość [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/). <sup>24.8</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.5 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.6 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.7 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.8 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words dla Python przez .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 poprawia wrażenia związane z zarządzaniem kolorami obrysu, ulepsza OLE obiekty, a także wprowadza nowy `Bibliography Sources` public API.

Aspose.Words 24.2 rozszerzone wykresy API i zarządzanie stylem. Ta wersja Aspose.Words wprowadziła również możliwość określania SvgSaveOptions podczas renderowania, bardziej elastycznego sterowania ładowaniem plików Markdown i pracy z tekstem odniesienia dla przypisów dolnych i końcowych.

Aspose.Words 24.3 wprowadza Nowy TIFF Reader / Writer i emulację binarnych operacji rastrowych dla WMF metaplików. Aspose.Words 24.3 kontynuuje również rozszerzanie Wykresów API.

Aspose.Words 24.4 usprawnia zapisywanie formatów, niektóre opcje renderowania, a także usprawnia pracę z podpisami cyfrowymi.

### Obsługiwane Formaty <sup>24.4</sup>

Nowoczesny format obrazu **WebP** jest teraz obsługiwany w Aspose.Words dla .NET Framework 4.6.2 i wyżej. Możesz teraz czytać i wstawiać obrazy WebP do dokumentów, a także zapisywać obrazy w formacie WebP.

Należy pamiętać, że WebP jest obecnie dostępny tylko w .NET Standard i .NET Framework v4.6.2 i nowszych.

### Renderowanie i drukowanie

#### Kontrola Koloru Obrysu <sup>24.1</sup>

Klasa [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) została rozszerzona o zestaw nowych właściwości publicznych związanych z zarządzaniem kolorami obrysu: [fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/) i [back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/), [fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/) i [back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### DrawingML Wykresy API Rozszerzenie <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** jest nadal rozwijany.

#### Osadź czcionki zadeklarowane w regułach @font-face <sup>24.4</sup>

Dodano możliwość osadzania czcionek zadeklarowanych w regułach @font-face w definicjach czcionek wynikowego dokumentu została wprowadzona przez dodanie nowej właściwości [support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/).

#### Pracuj z formatowaniem blasku i odbicia <sup>24.4</sup>

Zaimplementowano możliwość pracy z formatowaniem blasku i odbicia dla obiektu rysunkowego.

### Ładowanie i zapisywanie dokumentów

#### Określ SvgSaveOptions Podczas Renderowania <sup>24.2</sup>

Możliwość określenia [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) podczas renderowania została dodana przy użyciu [ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) i [OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) metody.

#### Zachowaj puste linie podczas ładowania plików Markdown <sup>24.2</sup>

Dodano możliwość zachowania pustych linii podczas ładowania plików Markdown.

#### Nowy TIFF Czytelnik / Pisarz <sup>24.3</sup>

Opracowano nowy czytnik/pisarz TIFF dla Aspose.Words. Aspose.Words dla .NET 24.3 dodano obsługę odczytu obrazów TIFF z JPEG i starymi typami kompresji JPEG, a także znacznie poprawiono jakość operacji odczytu i zapisu.

### Inne

* Możliwość modyfikowania tekstu kontrolki `TextBox` OLE została wprowadzona przez dodanie nowej właściwości **Text** do nowej klasy **TextBoxControl**. <sup>24.1</sup>
* Bibliografia Sources public API została zaimplementowana poprzez dodanie nowej przestrzeni nazw [Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/) z nowymi klasami i wyliczeniami oraz poprzez dodanie nowej właściwości [bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/) do klasy [Document](https://reference.aspose.com/words/python-net/aspose.words/document/). <sup>24.1</sup>
* Nowe właściwości publiczne [priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/), [unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/) i [semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/) dla ulepszonego zarządzania stylem zostały dodane do klasy [Style](https://reference.aspose.com/words/python-net/aspose.words/style/). <sup>24.2</sup>
* Funkcjonalność pobierania rzeczywistego tekstu znaku odniesienia dla przypisów dolnych i końcowych została wzbogacona o Właściwość [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/) i metodę [update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default). <sup>24.2</sup>
* Zaimplementowano emulację binarnych operacji rastrowych dla WMF metaplików. <sup>24.3</sup>
* Możliwość definiowania opcji podpisu dla dokumentów w **SaveOptions** została włączona poprzez dodanie nowej klasy [DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/) z nowymi członkami publicznymi, a także dodanie nowych właściwości do klas [OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/) i [OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.1 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.2 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.3 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 24.4 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words dla Python przez .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 rozszerza opcje renderowania, emulację renderowania metapliku i markdown opcje zapisywania.

Aspose.Words 23.10 poprawia renderowanie, rozszerza opcje ładowania i zapisywania dokumentów oraz umożliwia użytkownikom scalanie dokumentów na nowe sposoby.

Aspose.Words 23.11 usprawnia pracę z wersjami, formatem XLSX i czcionkami w legendzie wykresu z dodatkowymi opcjami.

Aspose.Words 23.12 wprowadza nowe właściwości i wyliczenia do pracy z dokumentami PDF i OOXML, a także obsługę obrazów WebP.

### Renderowanie i drukowanie

#### Dostosowywanie tytułów osi na wykresach DrawingML <sup>23.9</sup>

Możliwość dostosowywania tytułów osi na wykresach DrawingML została wprowadzona przez implementację nowej klasy publicznej [ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/) i właściwości [title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/).

####  Określanie pozycji pionowej czcionek w akapicie <sup>23.9</sup>

Teraz Można zdefiniować pionowe położenie czcionek w akapicie przy użyciu nowej właściwości public [baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/) i nowego wyliczenia [BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/).

#### Kontrola Koloru Pierwszego Planu <sup>23.10</sup>

Możliwość pobierania koloru pierwszego planu bez modyfikatorów została dodana do klas [Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/) i [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) za pośrednictwem właściwości **BaseForeColor**.

#### Rozszerzenie funkcjonalności Wykresów <sup>23.10</sup>

Funkcjonalność klas [ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/) i [ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/) została rozszerzona o nowe metody i właściwości.

#### Automatycznie Dopasuj i Dopasuj obraz do kształtu <sup>23.10</sup>

Prosty sposób automatycznego dopasowania i dopasowania obrazu w określonym kształcie został zapewniony za pomocą nowej metody [fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default).

#### Domyślne formatowanie czcionek dla wpisów legendy wykresu DrawingML <sup>23.11</sup>

Możliwość określenia domyślnego formatowania czcionek dla wpisów legendy Wykresów DrawingML została dodana za pośrednictwem właściwości [font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/). Ta funkcja ułatwia bardziej usprawniony i spójny wygląd elementów wykresu, poprawiając ogólną estetykę dokumentu.

#### Określ układ strony podczas otwierania PDF w czytniku <sup>23.12</sup>

Możliwość określenia układu strony, który ma być używany podczas otwierania dokumentu w czytniku PDF, została dodana poprzez wprowadzenie nowej właściwości [page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/) do klasy [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) i wprowadzenie nowego wyliczenia [PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/).

### Ładowanie i zapisywanie dokumentów

#### Określanie nazwy folderu do konstruowania obrazu URIs w Markdown <sup>23.9</sup>

Klasa [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) została rozszerzona o Właściwość [images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/), która pozwala określić nazwę folderu użytego do skonstruowania obrazu URIs zapisanego w dokumencie Markdown.

#### Zmniejsz Rozmiar Wyjściowy PDF <sup>23.10</sup>

Zaimplementowano różne optymalizacje renderowania PDF w celu zmniejszenia rozmiaru wyjściowego przy użyciu ustawień [optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/).

#### Rozpoznaj hiperłącza podczas ładowania dokumentów TXT <sup>23.10</sup>

Funkcja rozpoznawania hiperłączy podczas ładowania dokumentów TXT została zaimplementowana przez dodanie nowej właściwości [detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/).

### Inne

- Zaimplementowano emulację renderowania metaplików w celu określenia rozmiaru rasteryzacji, szczególnie dla WMF szerokości pióra i EMF szerokości pióra kosmetycznego. Aby to osiągnąć, właściwość **ScaleWmfFontsToMetafileSize** została zastąpiona właściwością [emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/) i dodano Właściwość [emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/). <sup>23.9</sup>
- Uproszczona metoda wstawiania jednego dokumentu do innego dokumentu w bieżącej pozycji kursora została wprowadzona przy użyciu metody [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions). <sup>23.10</sup>
- Możliwość dostępu i modyfikowania właściwości stylu została dodana poprzez wprowadzenie nowej właściwości [locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/). <sup>23.10</sup>
- Ogólny parametr typu został dodany do metod klasy [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/). <sup>23.10</sup>
- Możliwość zapisania wszystkich sekcji dokumentu w tym samym arkuszu XLSX została zapewniona przez nowy typ wyliczenia [XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/) i właściwość new [section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/). <sup>23.11</sup>
* Sposób kontrolowania sposobu użycia rozszerzeń formatu ZIP64 dla dokumentów OOXML został zaimplementowany za pomocą właściwości new Zip64Mode klasy `OoxmlSaveOptions` i wyliczenia new Zip64Mode. <sup>23.12</sup>
* Wprowadzono obsługę obrazu WebP. Należy pamiętać, że ta funkcja jest dostępna tylko dla .NetStandart i .NET6+ wersji. <sup>23.12</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla Python via .NET 23.9 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 23.10 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 23.11 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 23.12 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words dla Python przez .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 zwiększa możliwość pracy z danymi serii wykresów i możliwość pracy z dokumentami ODT, a także poprawić nagłówki/stopki i ich zawijanie tekstu.

Aspose.Words 23.6 rozszerza opcje renderowania, dodaje nowy format eksportu, poprawia LINQ raportowanie i LowCode narzędzia.

Aspose.Words 23.7 zwiększa możliwości raportowania, dodaje nowy format eksportu i wprowadza zmiany w pracy z tabelami i podpisami cyfrowymi.

Aspose.Words 23.8 rozszerza możliwości różnych formatów, poprawia renderowanie i dodaje nowe opcje pracy z polami.

### Obsługiwane Formaty

* Począwszy od wersji 23.6, możliwe jest zapisanie dokumentu w formacie XLSX. Teraz możesz konwertować swoje dokumenty do formatu Excel. <sup>23.6</sup>

* Począwszy od wersji 23.7, możliwe jest zapisanie strony dokumentu lub kształtu w formacie EPS. <sup>23.7</sup>

### Nowe Funkcje Formatu

- Wprowadzono funkcję automatycznego generowania spisu treści (TOC) dla dokumentów MOBI. <sup>23.8</sup>
- Konstruktor [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) został rozszerzony o [PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions). <sup>23.8</sup>
- Zaimplementowano kształtowanie tekstu pionowego dla metaplików EMF. <sup>23.8</sup>

### Rendering

#### Pobierz i zmodyfikuj dane serii Wykresów <sup>23.5</sup>

Funkcja pobierania i modyfikowania danych serii Wykresów została zapewniona przez dodanie:

- nowe klasy: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- nowe typy wyliczeń: [ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### Wsparcie dla zaawansowanej typografii <sup>23.6</sup>

Dodano obsługę zaawansowanej typografii w renderowaniu WMF, EMF i EMF+.

#### Kolorowe treści na stronie <sup>23.6</sup>

Własność publiczna [PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/), wskazująca, czy strona jest kolorowa, czy nie, została dodana.

#### Formatowanie etykiet danych wykresu <sup>23.6</sup>

Zaimplementowano możliwość ustawienia formatowania wypełnienia, obrysu i objaśnienia dla etykiet danych wykresu.

### Mail Merge i raportowanie

#### Dynamiczne Wstawianie HTML dla LINQ silnika raportowania <sup>23.6</sup>

Dodano nowy sposób dynamicznego wstawiania HTML dla LINQ silnika raportowania.

#### Mustache Obsługa Tagów <sup>23.7</sup>

Znaczniki Mustache są teraz obsługiwane w metodach [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/) i [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/).

#### Określanie rozmiaru renderowanych obrazów <sup>23.8</sup>

Wprowadzono nową właściwość publiczną [image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/) do określania rozmiaru renderowanych obrazów w pikselu.

#### Zachowaj spacje dla wartości ciągów JSON - LINQ <sup>23.8</sup>

Do mechanizmu raportowania LINQ Dodano opcję, aby zachować spacje dla wartości ciągów JSON.

### LowCode <sup>23.6</sup>

Dodano nowe metody LowCode przeznaczone do łączenia różnych typów dokumentów w jeden dokument wyjściowy.

### Inne

- Zaimplementowano obsługę zawijania tekstu w nagłówkach/stopkach. <sup>23.5</sup>
- Możliwość usuwania podpisów cyfrowych z dokumentów ODT została dodana metodą [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str). <sup>23.5</sup>
- Dodano własność publiczną [phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/) w celu uzyskania podstawowego i rubinowego tekstu przewodnika fonetycznego [Run](https://reference.aspose.com/words/python-net/aspose.words/run/). <sup>23.5</sup>
- Możliwość pobierania wartości podpisu cyfrowego z podpisanego cyfrowo dokumentu jako tablicy bajtów została dodana poprzez wprowadzenie nowej właściwości [signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/). <sup>23.7</sup>
- Klasy [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/) i [Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/) zostały rozszerzone o nowych członków publicznych– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), i [Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/). <sup>23.7</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla Python via .NET 23.5 Informacje O Wydaniu](/words/python-net/aspose-words-for-python-via-dotnet-23-5-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 23.6 Informacje O Wydaniu](/words/python-net/aspose-words-for-python-via-dotnet-23-6-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 23.7 Informacje O Wydaniu](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

Dowiedz się więcej o [Aspose.Words dla Python via .NET 23.8 Informacje O Wydaniu](/words/python-net/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## Zobacz także

{{% alert color="primary" %}}

Ta strona zawiera najnowsze wiadomości z ostatnich 2 lat. Aby uzyskać szczegółowe informacje na temat wcześniejszych wydań, zobacz [Release Notes"](https://releases.aspose.com/words/python/release-notes/) strony w odpowiednich sekcjach.

{{% /alert %}}
