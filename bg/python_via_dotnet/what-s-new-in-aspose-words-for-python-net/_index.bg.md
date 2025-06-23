---
title: Какво ново
second_title: Aspose.Words за Python via .NET
articleTitle: Какво е новото в Aspose.Words за Python via .NET
linktitle: Какво е новото в Aspose.Words за Python via .NET
type: docs
description: "Aspose.Words за Python via .NET разширява и подобрява всеки ден. На тази страница можете да научите за огромните и най-интересните характеристики на продукта."
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /bg/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-06-23-21-02-49
---

Тази страница описва най-интересните нови Aspose.Words функции, въведени в последните издания.

## Aspose.Words за Python via .NET 25.5, 25.6

Aspose.Words 25.5 подобрява персонализирането на диаграмите с нови опции за стилизиране и подобрява Markdown експорта, като предлага контрол върху това как се обработват празните параграфи.

Aspose.Words 25.6 подобрява прецизността и визуализацията чрез въвеждане на разширени опции за експортиране на изображения, подобрена обработка MathML и по-добро представяне на диаграмите.

### Конвертиране, зареждане и запазване на документи

#### Експортиране на празни параграфи до Markdown <sup>25.5</sup>

Възможността да се контролира как празните параграфи се експортират в Markdown е въведена чрез добавяне на **MarkdownEmptyParagraphExportMode** изброяване и **empty_paragraph_export_mode** свойство.

#### Експортиране на документи от няколко страници в растерни формати на изображения <sup>25.6</sup>

Възможността за експортиране на документи от няколко страници в растерни формати на изображения (като PNG и JPEG) с [customizable layouts](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) – хоризонтални, вертикални или мрежови – е въведена чрез разширяване на функционалността за експортиране на изображения.

### Рендериране

#### Задаване на стила на диаграмата <sup>25.5</sup>

Възможността за задаване на стила на диаграмата е въведена чрез добавяне на **ChartStyle** изброяване и **style** свойството.

#### Рендиране на съединителни линии в MathML изрази <sup>25.6</sup>

Рендирането на съединителните линии в MathML изрази е внедрено, за да се осигури по-точно и визуално последователно показване на математическите формули.

#### Създаване на Легенди за Водопадни диаграми <sup>25.6</sup>

Привеждането на легенди за ["Waterfall" charts](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriestype/) е въведена, увеличаване на прозрачността на данните и подобряване на интерпретацията на тези диаграми.

### Друго

* Възможността за обвиване на математически формули, съдържащи множество наклонени черти, е подобрена, подобрявайки яснотата на оформлението и четливостта на формулата. <sup>25.6</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Python via .NET 25.5 бележки по изданието](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-5-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 25.6 бележки по изданието](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words за Python чрез .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 въвежда AI - захранва проверката на граматиката и подобрява записването на документи с разширени опции за формати HTML, SVG и Markdown.

Aspose.Words 25.2 въвежда обобщаване на текст с Anthropic AI модели, добавя MsWorks поддръжка на формат, подобрява типографския контрол и подобрява PDF структурата и обработката на списъци.

Aspose.Words 25.3 подобрява AI - захранва граматика Проверка и избор на шрифт със свойството UpdateAmbiguousTextFont, както и подобрява PDF прикачени файлове износ.

Aspose.Words 25.4 въвежда поддръжка за нови размери на хартията, позволява разширен HTML контрол на износа и подобрява обработката с водни знаци.

### AI - захранващи функции

#### Документ AI Проверка На Граматиката

* Възможността за проверка на граматиката на предоставения документ, използвайки OpenAI генеративни модели е въведена чрез добавяне на нов [check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/) метод. <sup>25.1</sup>
* Функцията за проверка на граматиката AI е актуализирана, за да поддържа всички модели, налични в списъка [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Обобщаване Чрез Използване На Anthropic Генеративни Езикови Модели <sup>25.2</sup>

Обобщаването на текст с помощта на Anthropic генеративните езикови модели е разрешено чрез въвеждане на нов публичен клас [AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/).

### Поддържани Формати <sup>25.2</sup>

От версия 25.2 е добавена съвместимост с новия формат MsWorks за зареждане на Microsoft работни документи.

### Конвертиране, зареждане и запазване на документи

#### Подобрено записване до HTML и SVG формати <sup>25.1</sup>

Записването във формати HTML и SVG е подобрено чрез добавяне на **id_prefix** и **remove_java_script_from_links** свойства както към класовете [HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/), така и към класовете [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/).

#### Задайте разделителна способност на изображението и режим OfficeMath изход, когато записвате до Markdown <sup>25.1</sup>

* Към класа [image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/) е добавена нова опция [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/), За да зададете разделителната способност на изображението.
* Нова опция [office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/) и [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/) изброяване са добавени към класа [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/), за да се зададе OfficeMath изходен режим.

### Рендериране

#### Подобрен Типографски Контрол <sup>25.2</sup>

[number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/) свойството е добавено за подобрен типографски контрол.

#### Контролиране на избора на шрифт за двусмислени знаци <sup>25.3</sup>

В класа [update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/) е добавена нова публична собственост [SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/), За да се контролира изборът на шрифт според използвания код на знака.

#### Опции За Размер На Хартията <sup>25.4</sup>

Възможността за използване на JIS B4 и JIS B5 е въведена чрез добавяне на нови стойности към изброяването [PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/).

#### HTML Контрол На Изхода <sup>25.4</sup>

Възможността за премахване на JavaScript от хипервръзка URLs по време на HTML износ е въведена чрез добавяне на свойство [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/).

### Друго

* PDF логическата структура е подобрена с поддръжка на TOA, BIBLIOGRAPHY и INDEX полета. <sup>25.2</sup>
* [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate) методът е въведен за по-добро боравене със списъка. <sup>25.2</sup>
* Добавено е ново свойство [attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/), за да замени **EmbedAttachments**, за да подобри експортирането на PDF прикачени файлове. Също така към списъка [PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/) са добавени нови стойности, за да се поддържат PDF/A прикачени файлове към версии. Освен това прикачените файлове вече се поддържат с криптиране. <sup>25.3</sup>
* Възможността за задаване на воден знак за изображение от поток е въведена чрез добавяне на ново претоварване към метода [SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions). <sup>25.4</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Python via .NET 25.1 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 25.2 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 25.3 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 25.4 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words за Python чрез .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 въвежда group shape Вмъкване и StructuredDocumentTag Вмъкване чрез DocumentBuilder, подобрява рендирането на радиалната диаграма с градуации, подобрява цифровите подписи с поддръжка XAdES-EPES, добавя Markdown подчертаване и осигурява достъп до разделители на бележки под линия/бележка в края.

Aspose.Words 24.10 въвежда подобрена ActiveX поддръжка за контрол с CommandButton Създаване, нов контрол на видимостта на формата, възможност за group shapes, подобрен Markdown износ за таблици, форматиране на диаграми за Pie и Doughnut, по-добра работа с кодиране на големи 5 и поддръжка за остарели тайвански шрифтове.

Aspose.Words 24.11 въвежда AI - захранвано обобщаване на документи, подобрени опции за рендиране, подобрен достъп до свойствата на документа и ActiveX контрол на надписите.

Aspose.Words 24.12 въвежда Персонализируемо поставяне на етикети на данни, Гугъл AI-захранван превод на текст и подобрени нови LowCode класове за обработка.

### AI - захранващи функции

#### Обобщаване на документи чрез OpenAI и Гугъл <sup>24.11</sup>

Поддръжката за обобщаване на документи, използвайки **OpenAI** и **Google** генеративни езикови модели, е интегрирана чрез добавяне на пространство [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) с неговите публични членове.

#### Превод на текст с помощта на генеративните езикови модели на Гугъл <sup>24.12</sup>

Възможността за превод на текст с помощта на генеративните езикови модели на Гугъл е внедрена в Aspose.Words чрез добавяне на метода [translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/) и [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) изброяване към пространството [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Ново LowCode класове като [Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) и т.н. е въведена, предлагайки набор от методи, които постигат перфектния баланс между простота и гъвкавост за обработка на документи.

### Рендериране и печат

#### Градуации по радиални карти <sup>24.9</sup>

Реализирано е рендиране на градуации по радиални карти.

#### CommandButton ActiveX контроли <sup>24.10</sup>

Възможността за създаване на CommandButton ActiveX контроли е въведена чрез добавяне на нов публичен метод [insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/) и нов публичен клас [Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/).

#### Контрол На Видимостта На Формата <sup>24.10</sup>

Добавена е нова обществена собственост [hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/), за да се контролира видимостта на фигурите.

#### Промени в Pie и Doughnut диаграми <sup>24.10</sup>

Няколко нови публични свойства са добавени към формат Pie и Doughnut диаграми.

#### Контролирайте рендирането на PDF граници на поле за избор на формуляр <sup>24.11</sup>

Въведена е нова опция за контрол на рендирането на PDF граници на полета на формуляр за избор чрез добавяне на нова публична опция [render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/).

#### Получаване и задаване на кодове за форматиране на данни от диаграми <sup>24.11</sup>

Възможността за получаване и задаване на кодове за форматиране на данни от диаграми е добавена чрез внедряване на свойството [format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/) в класовете [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/) и [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/).

#### Рендиране на хистограма диаграми с кошчета и етикети <sup>24.11</sup>

Рендирането на хистограмата е подобрено, като позволява определен брой кошчета и етикети.

#### Персонализиране на поставянето на етикети на данни <sup>24.12</sup>

Възможността за персонализиране на поставянето на етикети на данни е добавена чрез въвеждане на нови свойства на тези класове [ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/) и [ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Конвертиране, зареждане и запазване на документи

#### Подчертаване на форматирането при зареждане Markdown файлове <sup>24.9</sup>

Опцията за разпознаване на форматирането на подчертаването при зареждане на документи Markdown е включена чрез добавяне на нова публична собственост [import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/).

#### Експортиране на таблици като HTML при запис до Markdown <sup>24.10</sup>

Възможност за експортиране на таблици като HTML при записване на документи във формат Markdown е реализирана чрез добавяне на нова публична собственост [export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/) и изброяване [MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/).

#### Експортиране PDF с актуализирана логическа структура <sup>24.11</sup>

PDF експортът е подобрен чрез включване на свойствата на заглавието на таблицата като PDF заглавия на елементите на логическата структура.

### Цифрови Подписи

#### Подписвайте документи с XAdES-EPES <sup>24.9</sup>

Възможността за подписване на документи с XAdES-EPES Ниво XML-DSig е въведена чрез добавяне на нова обществена собственост [xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/) и ново публично изброяване [XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/).

### Друго

* Добавен е нов публичен метод [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/) към group shapes. <sup>24.9</sup>
* Добавен е нов публичен метод [insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/), за да вмъкнете **StructuredDocumentTags** в документ. <sup>24.9</sup>
* Публичен достъп до разделители на бележки под линия/бележка в края е осигурен чрез добавяне на няколко публични класове и свойства. <sup>24.9</sup>
* Възможността за групиране на отделни фигури, group shapes заедно и директно групиране на фигури и group shapes е въведена чрез добавяне на [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist) Метод. <sup>24.10</sup>
* Биг5 обработка на кодиране за TrueType таблица с изображения е подобрена. <sup>24.10</sup>
* Подкрепата за остарели тайвански шрифтове е подобрена. <sup>24.10</sup>
* За достъп до свойствата на разширения документ, свойствата само за четене са добавени към класа [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/). <sup>24.11</sup>
* Задаването на надписи за контроли ActiveX е разрешено чрез добавяне на нов публичен сетер към свойството [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Python via .NET 24.9 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 24.10 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 24.11 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 24.12 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words за Python чрез .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 разширява опциите за сглобки, подобрява възможностите за рендиране и разширява някои други опции.

Aspose.Words 24.6 подобрява опциите за рендиране, подобрява функционалността за търсене и сравняване и разширява няколко други функции.

Aspose.Words 24.7 променя начина, по който работите с ActiveX, разширява възможностите за рендиране, както и експортирането към Markdown и XLSX формати.

Aspose.Words 24.8 подобрява персонализирането на диаграмите с прецизен контрол върху етикетите на осите, разширява управлението на шрифта, подобрява обработката на структурата на документите и добавя нови възможности за HTML/XAML износ, PDF функционалност, конвертиране на документи и цифрови подписи.

### Поддържани Формати

Като се започне от версия 24.7, Експортиране до PDF/UA-2 се поддържа, за да се осигури достъпност за потребители с увреждания.

### Рендериране и печат

#### Промени в диаграми, форми и DrawingML <sup>24.5</sup>

* DrawingML ефекти рендиране за SVG графики, разширяване на предишната функционалност, ограничена до изображения, е изпълнено.
* Поддръжка за създаване на комбо диаграми и коригиране на свойства като ширина на празнината, припокриване и мехурчеста скала в групи от серии е въведена чрез добавяне на класове [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/) и [ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/) и свойство [series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/).
* Функционалността за манипулиране на SoftEdge ефекта на фигурите е реализирана чрез добавяне на [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/) класа.
* Възможността за промяна на коригираните стойности на фигури е реализирана чрез добавяне на **AdjustmentCollection** и **Adjustment** публични класове и [adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/) собственост.

#### Промени в диаграми, форми и чертеж <sup>24.6</sup>

- Възможностите за картографиране са подобрени. Сега можете да създадете по-голямо разнообразие от диаграми, включително *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* диаграми, *Box & Whisker* диаграми, *Waterfalls* и *Funnels*. Това ви позволява да визуализирате данните си по по-разнообразен и информативен начин.
- Контролът на цветовете за форматиране на сенки е подобрен. Можете да получите по-прецизен контрол върху външния вид на вашите документи чрез достъп до цветове в сянка.
- Подобрението на производителността за фоново рендиране е подобрено. Можете значително да ускорите рендирането на фонове, съдържащи малки елементи, благодарение на естествената технология за облицоване.
- Добавени са реалистични градиенти за форми. Вече можете да създавате DML форми с нелинейни градиенти, имитирайки визуалния стил на Microsoft Word за по-полиран вид.

#### Персонализиране На Етикети За Данни На Диаграми <sup>24.7</sup>

Възможността за персонализиране на етикети на данни на диаграма, като **Orientation** и **Rotation** е добавена.

#### Потребителски номер стайлинг за списък нива <sup>24.7</sup>

Добавен е сетер за обществена собственост [custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/). Сега можете да дефинирате персонализиран номер за списъчни нива.

#### Промени в работата с ActiveX <sup>24.7</sup>

- Свойствата на ActiveX обектите вече могат да бъдат променяни, което ви дава по-голям контрол върху тяхното поведение.
- Добавена е възможността за промяна на стойността на контролата на радио бутона ActiveX, за да се даде възможност за динамично взаимодействие.
- Възможността да превключвате ActiveX checkbox на "проверено " или" неотбелязано " е добавена.

#### Контрол върху оста на диаграмата тик Етикети ориентация и въртене <sup>24.8</sup>

Прецизен контрол върху ориентацията и въртенето на етикетите на осите на диаграмата е добавен за по – удобно персонализиране на диаграмата-класът [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) е разширен с нови [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) и [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/) свойства.

#### Замяна на наклонената черта със знака на йената <sup>24.8</sup>

Обратната съвместима HTML и XAML износ за замяна на обратно наклонената черта със знака на йената е подобрена. За да се постигне това, имотът **replace_backslash_with_yen_sign** е добавен към класовете [HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/) и [XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/).

#### Използване на SDT етикети като имена на полета на формуляри при експортиране към PDF <sup>24.8</sup>

PDF експортирането с поддръжка за използване на SDT тагове като имена на полета на формуляри е подобрено чрез добавяне на ново свойство [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) към класа [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/).

### Конвертиране, зареждане и запазване на документи

#### Експортиране на връзки към Markdown формат <sup>24.7</sup>

Възможността да се контролира експортирането на връзки във формат Markdown е добавена чрез имплементацията на [link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/) свойството.

#### LowCode 24.8 <sup>24.8</sup>

Въведен е нов [LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/) клас, предназначен да осигури набор от методи за конвертиране на различни типове документи с един ред код.

### Търсене и сравняване

#### Разширени Опции За Сравнение <sup>24.6</sup>

Добавена е възможността за рационализиране на работните потоци за анализ на данни с подобрена функционалност за сравнение. Това включва нова опция [ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/) и преработен интерфейс за напреднали сравнения.

### Друго

* Функцията за премахване на празни страници от документ е реализирана чрез добавяне на метода [remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/). <sup>24.5</sup>
* Възможността да се провери за наличие на VBA макроси без зареждане на документ е осигурена чрез добавяне на свойство [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/). <sup>24.5</sup>
* Поддържането на номериране на източника при вмъкване на документ с помощта на LINQ двигател за докладване вече се поддържа. <sup>24.5</sup>
* Добавено е ново [date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/) свойство-това осигурява по-точен времеви печат за коментари, подобряване на организацията и проследимостта. <sup>24.6</sup>
* Форматът за дата и час сега автоматично се открива за безпроблемно експортиране във формат XLSX. <sup>24.7</sup>
* Добавена е обществена собственост [is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/), която ви позволява да проверите дали даден проект VBA е защитен. <sup>24.7</sup>
* Информацията за шрифта е разширена със свойството **embedding_licensing_rights**, добавено към класовете [FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/) и [PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* Начин за ефективно изчистване на горни и долни колонтитули на секции при запазване на водните знаци е добавен за по-точно работа със структурата на документа. За да изчистите горни и долни колонтитули на секции, използвайте новия публичен метод [clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default). <sup>24.8</sup>
* Цифровото подписване на XPS документи с [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/) е активирано – за тази цел е добавено ново свойство [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/). <sup>24.8</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Python via .NET 24.5 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 24.6 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 24.7 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 24.8 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words за Python чрез .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 подобрява опита около управлението на цветовете на хода, подобрява OLE обекти, както и въвежда ново `Bibliography Sources` публично API.

Aspose.Words 24.2 разширени графики API и управление на стила. Тази версия на Aspose.Words също така въведе възможността за задаване на SvgSaveOptions по време на рендиране, по-гъвкав контрол за зареждане Markdown файлове и работа с референтен текст за бележки под линия и бележки в края.

Aspose.Words 24.3 въвежда нов TIFF четец / писател и емулация на бинарни растерни операции за WMF метафили. Aspose.Words 24.3 също продължава да разширява класациите API.

Aspose.Words 24.4 подобрява записващите формати, някои опции за рендиране, както и подобрява работата с цифрови подписи.

### Поддържани Формати <sup>24.4</sup>

Модерният **WebP** формат на изображението вече се поддържа в Aspose.Words за .NET Framework 4.6.2 и по-високо. Вече можете да четете и вмъквате WebP изображения в документи, както и да запазвате изображения във формат WebP.

Моля, обърнете внимание, че WebP в момента е наличен само в .NET Standard и .NET Framework в4.6.2 и по-горе.

### Рендериране и печат

#### Контрол На Цвета На Хода <sup>24.1</sup>

Класът [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) е разширен с набор от нови публични свойства, свързани с управлението на цветовете на ходовете: [fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/) и [back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/), [fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/) и [back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### DrawingML Диаграми API Разширение <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** продължава да се разширява.

#### Вграждане на шрифтове, обявени в @font-face правила <sup>24.4</sup>

Добавена е възможност за вграждане на шрифтове, декларирани в @font-face Правила в получените дефиниции на шрифта на документа, чрез добавяне на ново свойство [support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/).

#### Работа с форматиране на отблясъци и отражения <sup>24.4</sup>

Способността да се работи с блясък и отражение форматиране за чертеж обект е реализирана.

### Зареждане и съхранение на документи

#### Посочете SvgSaveOptions По Време На Рендирането <sup>24.2</sup>

Възможността за задаване на [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) по време на рендирането е добавена с помощта на [ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) и [OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) методи.

#### Запазване на празните редове при зареждане Markdown файлове <sup>24.2</sup>

Възможността за запазване на празни линии при зареждане Markdown файлове е добавена.

#### Ново TIFF Читател / Писател <sup>24.3</sup>

Създаден е нов TIFF читател / писател за Aspose.Words. Aspose.Words за .NET 24.3 Добавена е поддръжка за четене TIFF изображения с JPEG и стари JPEG компресионни типове, а също така значително подобрява качеството на операциите за четене и запис.

### Друго

* Възможността за промяна на текста на `TextBox` OLE контролата е въведена чрез добавяне на ново свойство **Text** към новия **TextBoxControl** клас. <sup>24.1</sup>
* Библиографията източници публичен API е реализирана чрез добавяне на ново пространство от имена [Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/) с неговите нови класове и изброявания и чрез добавяне на ново свойство [bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/) към [Document](https://reference.aspose.com/words/python-net/aspose.words/document/) клас. <sup>24.1</sup>
* Нови публични свойства [priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/), [unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/) и [semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/) за подобрено управление на стила са добавени към [Style](https://reference.aspose.com/words/python-net/aspose.words/style/) класа. <sup>24.2</sup>
* Функционалността за извличане на действителния текст на референтния знак за бележки под линия и бележки в края е подобрена със свойството [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/) и метода [update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default). <sup>24.2</sup>
* Въведена е емулация на бинарни растерни операции за WMF метафили. <sup>24.3</sup>
* Възможността за дефиниране на опции за подпис за документи в рамките на **SaveOptions** е разрешена чрез добавяне на нов клас [DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/) с нови публични членове, както и добавяне на нови свойства към класовете [OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/) и [OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Python via .NET 24.1 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 24.2 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 24.3 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 24.4 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words за Python чрез .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 разширява опциите за рендиране, емулацията на рендиране на метаданни и markdown Опции за записване.

Aspose.Words 23.10 подобрява рендирането, разширява опциите за зареждане и записване на документи и позволява на потребителите да обединяват документи по нови начини.

Aspose.Words 23.11 подобрява работата с ревизии, XLSX формат и шрифтове на легендата на диаграмата с допълнителни опции.

Aspose.Words 23.12 въвежда нови свойства и изброявания за работа с PDF и OOXML документи, както и поддръжка на WebP изображения.

### Рендериране и печат

#### Персонализиране на заглавията на осите в DrawingML диаграми <sup>23.9</sup>

Възможността за персонализиране на заглавията на осите в DrawingML диаграми е въведена чрез внедряването на нов публичен клас [ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/) и [title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/) собственост.

####  Определяне на вертикалната позиция на шрифтовете в абзац <sup>23.9</sup>

Сега е възможно да се определи вертикалната позиция на шрифтовете в рамките на абзац, като се използва новото публично свойство [baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/) и новото изброяване [BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/).

#### Контрол На Цветовете На Преден План <sup>23.10</sup>

Възможността за извличане на цвета на преден план без модификатори е добавена към класовете [Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/) и [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) чрез свойството **BaseForeColor**.

#### Разширяване на функционалността на графиките <sup>23.10</sup>

Функционалността на класовете [ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/) и [ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/) е разширена с нови методи и свойства.

#### Автоматично регулиране и поставяне на изображение във фигура <sup>23.10</sup>

Лесен начин за автоматично регулиране и поставяне на изображение в определена форма е предоставен чрез новия метод [fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default).

#### Форматиране на шрифта по подразбиране за записи в Легендата на диаграмата DrawingML <sup>23.11</sup>

Възможността за задаване на форматиране на шрифта по подразбиране за записи в легендата на DrawingML диаграми е добавена чрез свойството [font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/). Тази функция улеснява по-опростен и последователен външен вид за елементите на диаграмата, подобрявайки цялостната естетика на документа.

#### Посочете оформлението на страницата при отваряне PDF в четец <sup>23.12</sup>

Възможността да се определи оформлението на страницата, което да се използва при отваряне на документ в четец PDF, е добавена чрез въвеждането на ново свойство [page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/) в класа [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) и въвеждането на ново изброяване [PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/).

### Зареждане и съхранение на документи

#### Задаване на име на папка за изграждане на изображение URIs в Markdown <sup>23.9</sup>

Класът [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) е разширен чрез включване на свойството [images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/), което позволява да се зададе името на папката, използвана за конструиране на изображение URIs, написано в документа Markdown.

#### Намаляване PDF Изходния Размер <sup>23.10</sup>

Изпълнени са различни PDF оптимизации за рендиране, за да се намали размерът на изхода при използване на [optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/) настройки.

#### Разпознаване на хипервръзки при зареждане TXT документи <sup>23.10</sup>

Функцията за разпознаване на хипервръзки при зареждане на документи TXT е внедрена чрез добавяне на ново свойство [detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/).

### Друго

- Въведена е емулация на метафил за определяне на размера на растеризацията, по-специално за ширина на писалката WMF и ширина на козметичната писалка EMF. За да се постигне това, собствеността **ScaleWmfFontsToMetafileSize** е заменена с собственост [emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/) и собствеността [emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/) е добавена. <sup>23.9</sup>
- Чрез метода [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions) е въведен опростен метод за вмъкване на един документ в друг документ в текущата позиция на курсора. <sup>23.10</sup>
- Възможността за достъп и промяна на свойствата на стила е добавена чрез въвеждането на новата [locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/) собственост. <sup>23.10</sup>
- Към методите от класа [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/) е добавен общ тип параметър. <sup>23.10</sup>
- Възможността да се напишат всички раздели на документ върху един и същ работен лист XLSX е предоставена чрез новото свойство [XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/) изброяване и новото [section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/). <sup>23.11</sup>
* Начин да се контролира как ще се използват разширенията за формат ZIP64 за документи OOXML е внедрен чрез новото свойство на Зип64мода от класа `OoxmlSaveOptions` и новото номериране на Зип64мода. <sup>23.12</sup>
* Въведена е поддръжка за WebP изображение. Моля, имайте предвид, че тази функция е достъпна само за .NetStandart и .NET6+ версии. <sup>23.12</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Python via .NET 23.9 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 23.10 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 23.11 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

Научете повече за [Aspose.Words за .NET 23.12 Бележки По Изданието](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words за Python чрез .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 подобрява способността за работа с данни от серия диаграми и способността за работа с ODT документи, както и подобрява горни/долни колонтитули и тяхното обтичане на текст.

Aspose.Words 23.6 разширява опциите за рендиране, добавя нов формат за експортиране, подобрява инструментите LINQ за отчитане и LowCode.

Aspose.Words 23.7 подобрява възможностите за отчитане, добавя нов формат за експортиране и въвежда промени в работата с таблици и цифрови подписи.

Aspose.Words 23.8 разширява възможностите на различните формати, подобрява рендерирането и добавя нови опции за работа с полета.

### Поддържани Формати

* Започвайки с версия 23.6, е възможно да запишете документ във формат XLSX. Сега можете да конвертирате вашите документи да ексел формат. <sup>23.6</sup>

* Започвайки с версия 23.7, е възможно да запишете страница или фигура на документ във формат EPS. <sup>23.7</sup>

### Нови Функции Формат

- Въведена е функцията за автоматично генериране на съдържание (TOC) за MOBI документи. <sup>23.8</sup>
- [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) конструкторът е разширен с [PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions). <sup>23.8</sup>
- Оформянето на вертикален текст за EMF метафили е изпълнено. <sup>23.8</sup>

### Рендериране

#### Получаване и промяна на данни от серия диаграми <sup>23.5</sup>

Функцията за получаване и промяна на данни от серия диаграми е предоставена чрез добавяне на:

- нови класове: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- нови типове: [ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### Поддръжка за разширена Типография <sup>23.6</sup>

Добавена е поддръжка за разширена Типография в WMF, EMF и EMF + рендиране.

#### Цветно съдържание на страницата <sup>23.6</sup>

Добавена е обществена собственост [PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/), показваща дали страницата е оцветена или не.

#### Форматиране за етикети на данни на диаграма <sup>23.6</sup>

Възможността за задаване на запълване, щрихиране и форматиране на изнесено означение за етикети на данни на диаграма е изпълнена.

### Mail Merge и докладване

#### Динамичен HTML Вмъкване за LINQ докладващ двигател <sup>23.6</sup>

Добавен е нов начин за динамично вмъкване на HTML за LINQ отчетен двигател.

#### Mustache Етикети Поддръжка <sup>23.7</sup>

Mustache таговете вече се поддържат в методите [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/) и [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/).

#### Определяне на размера на Рендираните изображения <sup>23.8</sup>

Въведена е нова обществена собственост [image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/) за определяне на размера на изобразените изображения в пиксел.

#### Запазване на интервали за JSON низови стойности - LINQ <sup>23.8</sup>

Добавена е опция за отчитане на LINQ, за да се запазят празните пространства за JSON низови стойности.

### LowCode <sup>23.6</sup>

Добавени са нови LowCode методи, предназначени за обединяване на различни видове документи в един изходен документ.

### Друго

- Реализирана е поддръжка за обтичане на текст в горни/долни колонтитули. <sup>23.5</sup>
- Възможността за премахване на цифрови подписи от документи ODT е добавена чрез метода [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str). <sup>23.5</sup>
- Добавена е обществена собственост [phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/) за получаване на базов и рубинен текст на фонетичното ръководство [Run](https://reference.aspose.com/words/python-net/aspose.words/run/). <sup>23.5</sup>
- Възможността за извличане на стойност на цифров подпис от цифрово подписан документ като байтов масив е добавена чрез въвеждане на ново свойство [signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/). <sup>23.7</sup>
- Класовете [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/) и [Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/) бяха разширени с нови членове– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), и [Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/). <sup>23.7</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Python via .NET 23.5 Бележки За Издаване](/words/python-net/aspose-words-for-python-via-dotnet-23-5-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 23.6 Бележки За Издаване](/words/python-net/aspose-words-for-python-via-dotnet-23-6-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 23.7 Бележки За Издаване](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

Научете повече за [Aspose.Words за Python via .NET 23.8 Бележки За Издаване](/words/python-net/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## Вижте Също

{{% alert color="primary" %}}

Тази страница съдържа последните новини за последните 2 години. За подробности относно предишните издания вижте [Бележки](https://releases.aspose.com/words/python/release-notes/) страници в съответните раздели.

{{% /alert %}}
