---
title: Co nowego
second_title: Aspose.Words dla .NET
articleTitle: Co nowego w Aspose.Words dla .NET
linktitle: Co nowego w Aspose.Words dla .NET
type: docs
description: "Aspose.Words dla .NET rozszerza się i zwiększa codziennie. Na tej stronie możesz dowiedzieć się o ogromnych i najciekawszych funkcjach produktu."
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pl/net/what-s-new-in-aspose-words-for-net/
timestamp: 2025-06-23-21-02-49
---

Ta strona opisuje najciekawsze nowe funkcje Aspose.Words wprowadzone w ostatnich wydaniach.

## Aspose.Words dla .NET 25.5, 25.6

Aspose.Words 25.5 poprawia dostosowywanie Wykresów za pomocą nowych opcji stylizacji i poprawia eksport Markdown, oferując kontrolę nad sposobem obsługi pustych akapitów.

Aspose.Words 25.6 zwiększa precyzję renderowania i funkcje wizualizacji, wprowadzając zaawansowane opcje eksportu obrazu, ulepszoną obsługę MathML i lepszą reprezentację Wykresów.

### Konwertowanie, ładowanie i zapisywanie dokumentów

#### Eksportuj puste akapity do Markdown <sup>25.5</sup>

Możliwość kontrolowania sposobu eksportowania pustych akapitów do Markdown została wprowadzona przez dodanie wyliczenia [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownemptyparagraphexportmode/) i właściwości [EmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/emptyparagraphexportmode/).

#### Eksportuj wielostronicowe dokumenty do formatów obrazów rastrowych <sup>25.6</sup>

Możliwość eksportowania dokumentów wielostronicowych do formatów obrazów rastrowych (takich jak PNG i JPEG) za pomocą [customizable layouts](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) – poziomych, pionowych lub siatkowych – została wprowadzona poprzez rozszerzenie funkcji eksportu obrazów.

### Rendering

#### Ustawianie stylu wykresu <sup>25.5</sup>

Możliwość ustawienia stylu wykresu została wprowadzona przez dodanie wyliczenia [ChartStyle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartstyle/) i właściwości [Style](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/style/).

#### Renderowanie linii łączników w wyrażeniach MathML  <sup>25.6</sup>

Renderowanie linii łączących w wyrażeniach MathML zostało zaimplementowane, aby zapewnić dokładniejsze i spójne wizualnie wyświetlanie wzorów matematycznych.

#### Renderowanie Legend dla Wykresów wodospadów <sup>25.6</sup>

Wprowadzono renderowanie Legend dla ["Waterfall" charts](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriestype/), zwiększając przejrzystość danych i poprawiając interpretację tych wykresów.

### Inne

* Poprawiono możliwość zawijania formuł matematycznych zawierających wiele ukośników, poprawiając przejrzystość układu i czytelność formuł. <sup>25.6</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla .NET 25.5 Informacje o wydaniu](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-5-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 25.6 Informacje o wydaniu](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words dla .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 wprowadza sprawdzanie gramatyki z napędem AI i ulepsza zapisywanie dokumentów dzięki zaawansowanym opcjom formatów HTML, SVG i Markdown.

Aspose.Words 25.2 wprowadza podsumowanie tekstu za pomocą modeli Anthropic AI, dodaje obsługę formatu MsWorks, poprawia kontrolę typograficzną oraz poprawia strukturę i obsługę list PDF.

Aspose.Words 25.3 ulepsza sprawdzanie gramatyki i wybór czcionek z AI za pomocą właściwości UpdateAmbiguousTextFont, a także ulepsza eksport załączników PDF.

Aspose.Words 25.4 wprowadza obsługę nowych rozmiarów papieru, umożliwia zaawansowaną kontrolę eksportu HTML, poprawia obsługę znaków wodnych i zwiększa użyteczność LowCode API.

### AI - funkcje zasilane

#### Sprawdzanie Gramatyki Dokumentu AI

* Możliwość sprawdzenia gramatyki dostarczonego dokumentu przy użyciu OpenAI modeli generatywnych została wprowadzona poprzez dodanie nowej metody [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/). <sup>25.1</sup>
* Funkcja sprawdzania gramatyki obsługiwana przez AI została zaktualizowana, aby obsługiwać wszystkie modele dostępne w wyliczeniu [AiModelType](https://reference.aspose.com/words/net/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Podsumowanie Przy Użyciu Generatywnych Modeli Językowych Anthropic <sup>25.2</sup>

Podsumowanie tekstu przy użyciu generatywnych modeli języka Anthropic zostało włączone poprzez wprowadzenie nowej klasy publicznej [AnthropicAiModel](https://reference.aspose.com/words/net/aspose.words.ai/anthropicaimodel/).

### Low Code

#### Low Code API użyteczność <sup>25.4</sup>

Wprowadzono znaczące ulepszenia użyteczności **LowCode API**, upraszczając przetwarzanie dokumentów i zmniejszając potrzebę powtarzalnego kodu.

### Obsługiwane Formaty <sup>25.2</sup>

Począwszy od wersji 25.2, dodano zgodność z nowym formatem ładowania MsWorks dla Microsoft works documents.

### Konwertowanie, ładowanie i zapisywanie dokumentów

#### Ulepszone zapisywanie w formatach HTML i SVG <sup>25.1</sup>

Zapisywanie w formatach HTML i SVG zostało ulepszone poprzez dodanie właściwości **IdPrefix** i **RemoveJavaScriptFromLinks** do klas [HtmlFixedSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlfixedsaveoptions/) i [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/).

#### Ustaw rozdzielczość obrazu i tryb wyjścia OfficeMath podczas zapisywania do Markdown <sup>25.1</sup>

* Nowa opcja [ImageResolution](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imageresolution/) została dodana do klasy [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/), aby ustawić rozdzielczość obrazu.
* Nowa opcja [OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/officemathexportmode/) i [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownofficemathexportmode/) wyliczenie zostały dodane do klasy [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/), aby ustawić OfficeMath Tryb wyjściowy.
* Możliwość ustawienia znaku wodnego obrazu ze strumienia została wprowadzona przez dodanie nowego przeciążenia do metody [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage_2). <sup>25.4</sup>

### Rendering

#### Ulepszona Kontrola Typograficzna <sup>25.2</sup>

Właściwość [NumberSpacing](https://reference.aspose.com/words/net/aspose.words/font/numberspacing/) została dodana w celu poprawy kontroli typograficznej.

#### Kontrolowanie wyboru czcionki dla znaków niejednoznacznych <sup>25.3</sup>

Nowa właściwość publiczna [UpdateAmbiguousTextFont](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/updateambiguoustextfont/) została dodana do klasy [SaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/), aby kontrolować wybór czcionki zgodnie z użytym kodem znaku.

#### Opcje Rozmiaru Papieru <sup>25.4</sup>

Możliwość użycia JIS B4 i JIS B5 rozmiarów papieru została wprowadzona poprzez dodanie nowych wartości do wyliczenia [PaperSize](https://reference.aspose.com/words/net/aspose.words/papersize/).

#### HTML Kontrola Wyjścia <sup>25.4</sup>

Możliwość usunięcia JavaScript z hiperłącza URLs podczas eksportu HTML została wprowadzona przez dodanie właściwości [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/removejavascriptfromlinks/).

### Inne

* PDF struktura logiczna została ulepszona dzięki obsłudze pól TOA, BIBLIOGRAPHY i INDEX. <sup>25.2</sup>
* Metoda [AddSingleLevelList](https://reference.aspose.com/words/net/aspose.words.lists/listcollection/addsinglelevellist/) została wprowadzona w celu poprawy obsługi listy. <sup>25.2</sup>
* Dodano nową właściwość [AttachmentsEmbeddingMode](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/attachmentsembeddingmode/) w celu zastąpienia **EmbedAttachments** w celu ulepszenia eksportu PDF załączników. Ponadto do wyliczenia [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) Dodano nowe wartości, aby obsługiwać załączniki wersji PDF/A. Ponadto załączniki są teraz obsługiwane za pomocą szyfrowania. <sup>25.3</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla .NET 25.1 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-1-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 25.2 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-2-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 25.3 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-3-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 25.4 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words dla .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 wprowadza group shape wstawianie i StructuredDocumentTag wstawianie przez DocumentBuilder, poprawia renderowanie Wykresów promieniowych z podziałką, poprawia podpisy cyfrowe z obsługą XAdES-EPES, dodaje rozpoznawanie podkreśleń Markdown i zapewnia dostęp do separatorów przypisów/przypisów końcowych.

Aspose.Words 24.10 wprowadza ulepszoną obsługę sterowania ActiveX z tworzeniem CommandButton, nową kontrolę widoczności kształtu, możliwość group shapes, ulepszony eksport Markdown dla tabel, formatowanie wykresów dla Wykresów Pie i Doughnut, lepszą obsługę kodowania Big5 i obsługę przestarzałych czcionek tajwańskich.

Aspose.Words 24.11 wprowadza AI-powered podsumowania dokumentu, ulepszone opcje renderowania, lepszy dostęp do Właściwości dokumentu i ActiveX napisów sterowania.

Aspose.Words 24.12 wprowadza konfigurowalne umieszczanie etykiet danych, tłumaczenie tekstu oparte na Google AI, ulepszone opcje czyszczenia Mail Merge i nowe klasy przetwarzania LowCode.

### AI - funkcje zasilane

#### Podsumowanie dokumentów za pomocą OpenAI i Google <sup>24.11</sup>

Obsługa podsumowania dokumentów przy użyciu generatywnych modeli językowych **OpenAI** i **Google** została zintegrowana poprzez dodanie przestrzeni nazw [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) wraz z jej publicznymi członkami.

#### Tłumaczenie tekstu przy użyciu generatywnych modeli językowych Google <sup>24.12</sup>

Możliwość tłumaczenia tekstu za pomocą generatywnych modeli językowych Google została zaimplementowana w Aspose.Words poprzez dodanie metody [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) i wyliczenia [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) do przestrzeni nazw [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Nowe LowCode klasy, takie jak[Comparer](https://reference.aspose.com/words/net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/net/aspose.words.lowcode/splitter/) itp. został wprowadzony, oferując zestaw metod, które zapewniają idealną równowagę między prostotą a elastycznością przetwarzania dokumentów.

### Renderowanie i drukowanie

#### Podziałka na wykresach promieniowych <sup>24.9</sup>

Zaimplementowano renderowanie podziałek na wykresach promieniowych.

#### CommandButton ActiveX sterowanie <sup>24.10</sup>

Możliwość tworzenia kontrolek CommandButton ActiveX została wprowadzona przez dodanie nowej metody publicznej [InsertForms2OleControl](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertforms2olecontrol/) i nowej klasy publicznej [Forms2OleControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/).

#### Kontrola Widoczności Kształtu <sup>24.10</sup>

Dodano nową właściwość publiczną [Hidden](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/hidden/), aby kontrolować widoczność kształtów.

#### Zmiany na wykresach Pie i Doughnut <sup>24.10</sup>

Dodano kilka nowych właściwości publicznych do Wykresów format Pie i Doughnut.

#### Kontroluj renderowanie granic pól formularza wyboru PDF <sup>24.11</sup>

Nowa opcja kontrolowania renderowania granic pól formularza wyboru PDF została zaimplementowana przez dodanie nowej opcji publicznej [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/renderchoiceformfieldborder/).

#### Pobierz i ustaw kody formatu dla danych wykresu <sup>24.11</sup>

Możliwość pobierania i ustawiania kodów formatu dla danych wykresu została dodana poprzez implementację właściwości [FormatCode](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/formatcode/) w klasach [ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/) i [BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/).

#### Renderuj wykresy histogramu z pojemnikami i etykietami <sup>24.11</sup>

Renderowanie wykresu histogramu zostało ulepszone, umożliwiając określoną liczbę pojemników i etykiet.

#### Dostosuj rozmieszczenie etykiet danych <sup>24.12</sup>

Dodano możliwość dostosowania rozmieszczenia etykiet danych poprzez wprowadzenie nowych właściwości do klas [ChartDataLabel](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabel/) i [ChartDataLabelCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Konwertowanie, ładowanie i zapisywanie dokumentów

#### Podkreśl formatowanie podczas ładowania plików Markdown <sup>24.9</sup>

Opcja rozpoznawania formatowania podkreślenia podczas ładowania dokumentów Markdown została włączona przez dodanie nowej własności publicznej [ImportUnderlineFormatting](https://reference.aspose.com/words/net/aspose.words.loading/markdownloadoptions/importunderlineformatting/).

#### Eksportowanie tabel jako HTML podczas zapisywania do Markdown <sup>24.10</sup>

Opcja eksportu tabel jako HTML podczas zapisywania dokumentów do formatu Markdown została zaimplementowana przez dodanie nowej własności publicznej [ExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/exportashtml/) i wyliczenia [MarkdownExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownexportashtml/).

#### Eksportuj PDF ze zaktualizowaną strukturą logiczną <sup>24.11</sup>

PDF eksport został wzmocniony przez włączenie właściwości tytułu tabeli jako PDF tytułów elementów struktury logicznej.

### Mail Merge i raportowanie

#### Usuń puste tabele podczas Mail Merge <sup>24.12</sup>

Nowa opcja **RemoveEmptyTables** została dodana do wyliczenia [MailMergeCleanupOptions](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmergecleanupoptions/), aby udoskonalić Mail Merge wyjście.

### Podpisy Cyfrowe

#### Podpisuj dokumenty za pomocą XAdES-EPES <sup>24.9</sup>

Możliwość podpisywania dokumentów z podpisami XAdES-EPES poziomu XML-DSig została wprowadzona przez dodanie nowej własności publicznej [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/signoptions/xmldsiglevel/) i nowego wyliczenia publicznego [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/xmldsiglevel/).

### Inne

* Nowa metoda publiczna [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/) została dodana do group shapes. <sup>24.9</sup>
* Dodano nową metodę publiczną [InsertStructuredDocumentTag](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertstructureddocumenttag/), aby wstawić **StructuredDocumentTags** do dokumentu. <sup>24.9</sup>
* Publiczny dostęp do separatorów przypisów / przypisów końcowych został zapewniony przez dodanie kilku publicznych klas i właściwości. <sup>24.9</sup>
* Możliwość grupowania poszczególnych kształtów, group shapes Razem i bezpośredniego grupowania zarówno kształtów, jak i group shapes została wprowadzona przez dodanie metody [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/#insertgroupshape_1). <sup>24.10</sup>
* Poprawiono obsługę kodowania Big5 dla tabel CMAP TrueType. <sup>24.10</sup>
* Ulepszono obsługę przestarzałych czcionek tajwańskich. <sup>24.10</sup>
* Aby uzyskać dostęp do rozszerzonych właściwości dokumentu, właściwości tylko do odczytu zostały dodane do klasy [BuiltInDocumentProperties](https://reference.aspose.com/words/net/aspose.words.properties/builtindocumentproperties/). <sup>24.11</sup>
* Ustawianie napisów dla kontrolek ActiveX zostało włączone przez dodanie nowego setera publicznego do właściwości [Forms2OleControl.Caption](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla .NET 24.9 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-9-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 24.10 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-10-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 24.11 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-11-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 24.12 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words dla .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 rozszerza opcje zestawów, poprawia możliwości renderowania i rozszerza niektóre inne opcje.

Aspose.Words 24.6 poprawia opcje renderowania, poprawia funkcje wyszukiwania i porównywania oraz rozszerza kilka innych funkcji.

Aspose.Words 24.7 zmienia sposób pracy z ActiveX, rozszerza możliwości renderowania, a także eksportuje do formatów Markdown i XLSX.

Aspose.Words 24.8 usprawnia dostosowywanie wykresów dzięki precyzyjnej kontroli nad etykietami osi, rozszerza zarządzanie czcionkami, poprawia obsługę struktury dokumentu i dodaje nowe możliwości eksportu HTML/XAML, funkcjonalności PDF, konwersji dokumentów i podpisów cyfrowych.

### Obsługiwane Formaty

Począwszy od wersji 24.7, eksport do PDF/UA-2 jest obsługiwany w celu zapewnienia dostępności dla użytkowników niepełnosprawnych.

### Platformy <sup>24.5</sup>

.NET 7.0/8.0 zespoły zostały zawarte w pakiecie Aspose.Words NuGet.

### Renderowanie i drukowanie

#### Zmiany w wykresach, kształtach i DrawingML <sup>24.5</sup>

* Zaimplementowano renderowanie efektów DrawingML dla Grafiki SVG, rozszerzając poprzednią funkcjonalność ograniczoną do obrazów.
* Obsługa tworzenia wykresów kombi i dostosowywania właściwości, takich jak szerokość szczeliny, nakładanie się i skala bąbelków w grupach serii, została wprowadzona przez dodanie klas [ChartSeriesGroup](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroup/) i [ChartSeriesGroupCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroupcollection/) oraz właściwości [SeriesGroups](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/seriesgroups/).
* Funkcjonalność manipulowania efektem SoftEdge kształtów została zaimplementowana przez dodanie klasy [SoftEdgeFormat](https://reference.aspose.com/words/net/aspose.words.drawing/softedgeformat/).
* Możliwość modyfikowania dostosowywania wartości kształtów została zaimplementowana przez dodanie klas publicznych [AdjustmentCollection](https://reference.aspose.com/words/net/aspose.words.drawing/adjustmentcollection/) i [Adjustment](https://reference.aspose.com/words/net/aspose.words.drawing/adjustment/) oraz właściwości [Adjustments](https://reference.aspose.com/words/net/aspose.words.drawing/shape/adjustments/).

#### Zmiany w wykresach, kształtach i rysunkach <sup>24.6</sup>

* Zwiększono możliwości tworzenia wykresów. Możesz teraz tworzyć szerszą gamę Wykresów, w tym*Treemaps*, *Sunbursts*, *Histograms*, *Pareto* wykresy, *Box & Whisker* wykresy, *Waterfalls* i *Funnels*. Pozwala to na wizualizację danych w bardziej zróżnicowany i informacyjny sposób.
* Poprawiono kontrolę koloru dla formatowania cienia. Możesz uzyskać bardziej precyzyjną kontrolę nad wyglądem dokumentów, uzyskując dostęp do kolorów cieni.
* Poprawiono zwiększenie wydajności renderowania w tle. Możesz znacznie przyspieszyć renderowanie tła zawierającego małe elementy dzięki natywnej technologii układania płytek.
* Dodano realistyczne gradienty kształtów. Możesz teraz tworzyć DML kształty z nieliniowymi gradientami, naśladując styl wizualny Microsoft Word, aby uzyskać bardziej dopracowany wygląd.

#### Dostosowanie Etykiety Danych Wykresu <sup>24.7</sup>

Dodano możliwość dostosowywania etykiet danych wykresów, takich jak **Orientation** i **Rotation**.

#### Niestandardowa Stylizacja numerów dla poziomów listy <sup>24.7</sup>

Dodano seter dla własności publicznej [CustomNumberStyleFormat](https://reference.aspose.com/words/net/aspose.words.lists/listlevel/customnumberstyleformat/). Możesz teraz zdefiniować niestandardową stylizację numerów dla poziomów listy.

#### Zmiany w pracy z ActiveX <sup>24.7</sup>

* Właściwości obiektów ActiveX można teraz modyfikować, co daje większą kontrolę nad ich zachowaniem.
* Dodano możliwość modyfikacji wartości przycisku opcji ActiveX w celu włączenia dynamicznej interakcji.
* Dodano możliwość przełączania ActiveX checkbox Na "zaznaczone" lub "odznaczone".

#### Kontrola nad osią wykresu zaznacz etykiety Orientacja i obrót <sup>24.8</sup>

Dodano precyzyjną kontrolę nad orientacją i obrotem etykiet znaczników osi wykresu w celu wygodniejszego dostosowywania wykresu - klasa [AxisTickLabels](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/) została rozszerzona o nowe właściwości [Orientation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/orientation/) i [Rotation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/rotation/).

#### Zastąpienie ukośnika odwrotnego znakiem Jena <sup>24.8</sup>

Wstecznie kompatybilny eksport HTML i XAML do zastąpienia znaku ukośnika odwrotnego znakiem Jena został ulepszony. Aby to osiągnąć, właściwość **ReplaceBackslashWithYenSign** została dodana do klas [HtmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/) i [XamlFlowSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xamlflowsaveoptions/).

#### Używanie znaczników SDT jako nazw pól formularza podczas eksportowania do PDF <sup>24.8</sup>

PDF eksport z obsługą używania znaczników SDT jako nazw pól formularza został ulepszony poprzez dodanie nowej właściwości [UseSdtTagAsFormFieldName](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/usesdttagasformfieldname/) do klasy [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/).

### Konwertowanie, ładowanie i zapisywanie dokumentów

#### Eksportowanie linków do formatu Markdown <sup>24.7</sup>

Możliwość kontrolowania eksportu linków w formacie Markdown została dodana poprzez implementację właściwości [LinkExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/linkexportmode/).

#### LowCode 24.8 <sup>24.8</sup>

Wprowadzono nową klasę [LowCode.Converter](https://reference.aspose.com/words/net/aspose.words.lowcode/converter/), zaprojektowaną w celu zapewnienia zestawu metod konwersji różnych typów dokumentów za pomocą jednego wiersza kodu.

### Wyszukaj i porównaj

#### Zaawansowane Opcje Porównania <sup>24.6</sup>
Dodano możliwość usprawnienia przepływów pracy analizy danych dzięki ulepszonej funkcji porównywania. Obejmuje to nową opcję [IgnoreStoreItemId](https://reference.aspose.com/words/net/aspose.words.comparing/advancedcompareoptions/ignorestoreitemid/) i przeprojektowany interfejs do zaawansowanych porównań.

### Inne

* Funkcja eliminacji pustych stron z dokumentu została zaimplementowana przez dodanie metody [RemoveBlankPages](https://reference.aspose.com/words/net/aspose.words/document/removeblankpages/). <sup>24.5</sup>
* Możliwość sprawdzenia obecności makr VBA bez ładowania dokumentu została zapewniona przez dodanie właściwości [HasMacros](https://reference.aspose.com/words/net/aspose.words/fileformatinfo/hasmacros/). <sup>24.5</sup>
* Utrzymywanie numeracji źródeł podczas wstawiania dokumentu przy użyciu mechanizmu raportowania LINQ jest teraz obsługiwane. <sup>24.5</sup>
* Dodano nową właściwość [DateTimeUtc](https://reference.aspose.com/words/net/aspose.words/comment/datetimeutc/) - zapewnia to dokładniejszy znacznik czasu dla komentarzy, poprawiając organizację i identyfikowalność. <sup>24.6</sup>
* Silnik raportowania LINQ został ulepszony. Dokonano selektywnego usuwania pustych akapitów i definicji niestandardowych komunikatów dla brakujących elementów obiektu, co prowadzi do czystszych i bardziej pouczających raportów. <sup>24.6</sup>
* Format datetime jest teraz automatycznie wykrywany w celu bezproblemowego eksportu do formatu XLSX. <sup>24.7</sup>
* Dodano własność publiczną [IsProtected](https://reference.aspose.com/words/net/aspose.words.vba/vbaproject/isprotected/), która pozwala sprawdzić, czy projekt VBA jest chroniony. <sup>24.7</sup>
* Informacje o czcionkach zostały rozszerzone o Właściwość **EmbeddingLicensingRights** dodaną do klas [FontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/fontinfo/) i [PhysicalFontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* Dodano sposób efektywnego czyszczenia nagłówków i stopek sekcji przy jednoczesnym zachowaniu znaków wodnych, aby dokładniej pracować ze strukturą dokumentu. Aby wyczyścić nagłówki i stopki sekcji, użyj nowej metody publicznej [ClearHeadersFooters](https://reference.aspose.com/words/net/aspose.words/section/clearheadersfooters/). <sup>24.8</sup>
* Włączono cyfrowe podpisywanie dokumentów XPS przy użyciu [XpsSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/) – w tym celu dodano nową właściwość [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/digitalsignaturedetails/). <sup>24.8</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla .NET 24.5 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-5-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 24.6 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-6-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 24.7 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-7-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 24.8 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words dla .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 poprawia wrażenia związane z zarządzaniem kolorami obrysów, poprawia OLE obiekty i LINQ raportowanie, a także wprowadza nowy `Bibliography Sources` public API.

Aspose.Words 24.2 rozszerzone wykresy API, Zarządzanie stylami i LINQ opcje. Ta wersja Aspose.Words wprowadziła również możliwość określania SvgSaveOptions podczas renderowania, bardziej elastycznego sterowania ładowaniem plików Markdown i pracy z tekstem odniesienia dla przypisów dolnych i końcowych.

Aspose.Words 24.3 wprowadza Nowy TIFF Reader / Writer i emulację binarnych operacji rastrowych dla WMF metaplików. Aspose.Words 24.3 kontynuuje również rozszerzanie Wykresów API.

Aspose.Words 24.4 usprawnia zapisywanie formatów, niektóre opcje renderowania, a także usprawnia pracę z podpisami cyfrowymi.

### Obsługiwane Formaty <sup>24.4</sup>

Nowoczesny format obrazu **WebP** jest teraz obsługiwany w Aspose.Words dla .NET Framework 4.6.2 i wyżej. Możesz teraz czytać i wstawiać obrazy WebP do dokumentów, a także zapisywać obrazy w formacie WebP.

Należy pamiętać, że WebP jest obecnie dostępny tylko w .NET Standard i .NET Framework v4.6.2 i nowszych.

### Renderowanie i drukowanie

#### Kontrola Koloru Obrysu <sup>24.1</sup>

Klasa [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) została rozszerzona o zestaw nowych właściwości publicznych związanych z zarządzaniem kolorami obrysu: [ForeThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/forethemecolor/) i [BackThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/foretintandshade/) i [BackTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backtintandshade/).

#### DrawingML Wykresy API Rozszerzenie <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** jest nadal rozwijany.

#### Osadź czcionki zadeklarowane w regułach @font-face <sup>24.4</sup>

Dodano możliwość osadzania czcionek zadeklarowanych w regułach @font-face w definicjach czcionek wynikowego dokumentu została wprowadzona przez dodanie nowej właściwości [SupportFontFaceRules](https://reference.aspose.com/words/net/aspose.words.loading/htmlloadoptions/supportfontfacerules/).

#### Pracuj z formatowaniem blasku i odbicia <sup>24.4</sup>

Zaimplementowano możliwość pracy z formatowaniem blasku i odbicia dla obiektu rysunkowego.

### Ładowanie i zapisywanie dokumentów

#### Określ SvgSaveOptions Podczas Renderowania <sup>24.2</sup>

Możliwość określenia [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/) podczas renderowania została dodana przy użyciu [ShapeRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) i [OfficeMathRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) metody.

#### Zachowaj puste linie podczas ładowania plików Markdown <sup>24.2</sup>

Dodano możliwość zachowania pustych linii podczas ładowania plików Markdown.

#### Nowy TIFF Czytelnik / Pisarz <sup>24.3</sup>

Nowy czytnik / pisarz TIFF dla Aspose.Words dla .NET Standard, .NET 6 i nowszych został opracowany. Aspose.Words dla .NET 24.3 dodano obsługę odczytu obrazów TIFF z JPEG i starymi typami kompresji JPEG, a także znacznie poprawiono jakość operacji odczytu i zapisu.

### Inne

* Możliwość modyfikowania tekstu kontrolki `TextBox` OLE została wprowadzona przez dodanie nowej właściwości [Text](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/text/) do nowej klasy [TextBoxControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/). <sup>24.1</sup>
* Bibliografia Sources public API została zaimplementowana poprzez dodanie nowej przestrzeni nazw [Aspose.Words.Bibliography](https://reference.aspose.com/words/net/aspose.words.bibliography/) z nowymi klasami i wyliczeniami oraz poprzez dodanie nowej właściwości [Bibliography](https://reference.aspose.com/words/net/aspose.words/document/bibliography/) do klasy [Document](https://reference.aspose.com/words/net/aspose.words/document/). <sup>24.1</sup>
* API aby ograniczyć dostęp do członków typu przy użyciu składni szablonu dla `LINQ Reporting Engine` został dostarczony. <sup>24.1</sup>
* Nowe właściwości publiczne [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) i [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) dla ulepszonego zarządzania stylem zostały dodane do klasy [Style](https://reference.aspose.com/words/net/aspose.words/style/). <sup>24.2</sup>
* Funkcjonalność pobierania rzeczywistego tekstu znaku odniesienia dla przypisów dolnych i końcowych została wzbogacona o Właściwość [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) i metodę [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* Kompatybilność z wykresami `Word 2016` dla `LINQ Reporting Engine` została włączona. <sup>24.2</sup>
* Zaimplementowano emulację binarnych operacji rastrowych dla WMF metaplików. <sup>24.3</sup>
* Możliwość definiowania opcji podpisu dla dokumentów w **SaveOptions** została włączona poprzez dodanie nowej klasy [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/digitalsignaturedetails/) z nowymi członkami publicznymi, a także dodanie nowych właściwości do klas [OoxmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/docsaveoptions/) i [OdtSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla .NET 24.1 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-1-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 24.2 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-2-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 24.3 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-3-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 24.4 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words dla .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 rozszerza opcje renderowania, emulację renderowania metapliku i markdown opcje zapisywania.

Aspose.Words 23.10 poprawia renderowanie, rozszerza opcje ładowania i zapisywania dokumentów oraz umożliwia użytkownikom scalanie dokumentów na nowe sposoby.

Aspose.Words 23.11 usprawnia pracę z wersjami, formatem XLSX i czcionkami w legendzie wykresu z dodatkowymi opcjami.

Aspose.Words 23.12 wprowadza nowe właściwości i wyliczenia do pracy z dokumentami PDF i OOXML, a także obsługę obrazów WebP.

### Renderowanie i drukowanie

#### Dostosowywanie tytułów osi na wykresach DrawingML <sup>23.9</sup>

Możliwość dostosowywania tytułów osi na wykresach DrawingML została wprowadzona przez implementację nowej klasy publicznej [ChartAxisTitle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxistitle/) i właściwości [Title](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxis/title/).

#### Określanie pozycji pionowej czcionek w akapicie <sup>23.9</sup>

Teraz Można zdefiniować pionowe położenie czcionek w akapicie przy użyciu nowej właściwości public [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/paragraphformat/baselinealignment/) i nowego wyliczenia [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/baselinealignment/).

#### Kontrola Koloru Pierwszego Planu <sup>23.10</sup>

Możliwość pobierania koloru pierwszego planu bez modyfikatorów została dodana do klas [Fill](https://reference.aspose.com/words/net/aspose.words.drawing/fill/) i [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) za pośrednictwem właściwości **BaseForeColor**.

#### Rozszerzenie funkcjonalności Wykresów <sup>23.10</sup>

Funkcjonalność klas [ChartDataPointCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseries/) i [ChartFormat](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartformat/) została rozszerzona o nowe metody i właściwości.

#### Automatycznie Dopasuj i Dopasuj obraz do kształtu <sup>23.10</sup>

Prosty sposób automatycznego dopasowania i dopasowania obrazu w określonym kształcie został zapewniony za pomocą nowej metody [FitImageToShape](https://reference.aspose.com/words/net/aspose.words.drawing/imagedata/fitimagetoshape/).

#### Domyślne formatowanie czcionek dla wpisów legendy wykresu DrawingML <sup>23.11</sup>

Możliwość określenia domyślnego formatowania czcionek dla wpisów legendy Wykresów DrawingML została dodana za pośrednictwem właściwości [Font](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartlegend/font/). Ta funkcja ułatwia bardziej usprawniony i spójny wygląd elementów wykresu, poprawiając ogólną estetykę dokumentu.

#### Określ układ strony podczas otwierania PDF w czytniku <sup>23.12</sup>

Możliwość określenia układu strony, który ma być używany podczas otwierania dokumentu w czytniku PDF, została dodana poprzez wprowadzenie nowej właściwości [PageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/pagelayout/) do klasy [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) i wprowadzenie nowego wyliczenia [PdfPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfpagelayout/).

### Ładowanie i zapisywanie dokumentów

#### Określanie nazwy folderu do konstruowania obrazu URIs w Markdown <sup>23.9</sup>

Klasa [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) została rozszerzona o Właściwość [ImagesFolderAlias](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imagesfolderalias/), która pozwala określić nazwę folderu użytego do skonstruowania obrazu URIs zapisanego w dokumencie Markdown.

#### Zmniejsz Rozmiar Wyjściowy PDF <sup>23.10</sup>

Zaimplementowano różne optymalizacje renderowania PDF w celu zmniejszenia rozmiaru wyjściowego przy użyciu ustawień [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/).

#### Rozpoznaj hiperłącza podczas ładowania dokumentów TXT <sup>23.10</sup>

Funkcja rozpoznawania hiperłączy podczas ładowania dokumentów TXT została zaimplementowana przez dodanie nowej właściwości [DetectHyperlinks](https://reference.aspose.com/words/net/aspose.words.loading/txtloadoptions/detecthyperlinks/).

### Inne

* Zaimplementowano emulację renderowania metaplików w celu określenia rozmiaru rasteryzacji, szczególnie dla WMF szerokości pióra i EMF szerokości pióra kosmetycznego. Aby to osiągnąć, właściwość **ScaleWmfFontsToMetafileSize** została zastąpiona właściwością [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpage/) i dodano Właściwość [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpageresolution/). <sup>23.9</sup>
* Uproszczona metoda wstawiania jednego dokumentu do innego dokumentu w bieżącej pozycji kursora została wprowadzona przy użyciu metody [InsertDocumentInline](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertdocumentinline/). <sup>23.10</sup>
* Możliwość dostępu i modyfikowania właściwości stylu została dodana poprzez wprowadzenie nowej właściwości [Locked](https://reference.aspose.com/words/net/aspose.words/style/locked/). <sup>23.10</sup>
* Ogólny parametr typu został dodany do metod klasy [CompositeNode](https://reference.aspose.com/words/net/aspose.words/compositenode/). <sup>23.10</sup>
* Sposób kontrolowania, kiedy pewna wersja powinna zostać zaakceptowana/odrzucona lub nie została zaimplementowana przy użyciu metod [Accept](https://reference.aspose.com/words/net/aspose.words/revisioncollection/accept/) i [Reject](https://reference.aspose.com/words/net/aspose.words/revisioncollection/reject/). To ulepszenie zapewnia użytkownikom lepszą kontrolę nad procesem weryfikacji. <sup>23.11</sup>
* Możliwość zapisania wszystkich sekcji dokumentu w tym samym arkuszu XLSX została zapewniona przez nowy typ wyliczenia [XlsxSectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsectionmode/) i właściwość new [SectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsaveoptions/sectionmode/). <sup>23.11</sup>
* Sposób kontrolowania sposobu użycia rozszerzeń formatu ZIP64 dla dokumentów OOXML został zaimplementowany za pomocą nowej właściwości Zip64Mode klasy `OoxmlSaveOptions` i nowego wyliczenia Zip64Mode. <sup>23.12</sup>
* Wprowadzono obsługę obrazu WebP. Należy pamiętać, że ta funkcja jest dostępna tylko dla .NetStandart i .NET6+ wersji. <sup>23.12</sup>

{{% alert color="primary" %}}

Dowiedz się więcej o [Aspose.Words dla .NET 23.9 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-9-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 23.10 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-10-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 23.11 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-11-release-notes/).

Dowiedz się więcej o [Aspose.Words dla .NET 23.12 Informacje O Wydaniu](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-12-release-notes/).

{{% /alert %}}

## Zobacz także

{{% alert color="primary" %}}

Ta strona zawiera najnowsze wiadomości z ostatnich 2 lat. Aby uzyskać szczegółowe informacje na temat wcześniejszych wydań, zobacz [Release Notes"](https://releases.aspose.com/words/net/release-notes/) strony w odpowiednich sekcjach.

{{% /alert %}}
