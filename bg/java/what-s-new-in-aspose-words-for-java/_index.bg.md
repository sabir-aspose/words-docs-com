---
title: Какво ново
second_title: Aspose.Words за Java
articleTitle: Какво е новото в Aspose.Words за Java
linktitle: Какво е новото в Aspose.Words за Java
type: docs
description: "Aspose.Words за Java разширява и подобрява всеки ден. На тази страница можете да научите за огромните и най-интересните характеристики на продукта."
weight: 2
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/java/what-s-new-in-aspose-words-for-java/
timestamp: 2025-06-23-21-02-49
---

Тази страница описва най-интересните нови Aspose.Words функции, въведени в последните издания.

## Aspose.Words за Java 25.5, 25.6

Aspose.Words 25.5 подобрява персонализирането на диаграмите с нови опции за стилизиране и подобрява Markdown експорта, като предлага контрол върху това как се обработват празните параграфи.

Aspose.Words 25.6 подобрява прецизността и визуализацията чрез въвеждане на разширени опции за експортиране на изображения, подобрена обработка MathML и по-добро представяне на диаграмите.

### Конвертиране, зареждане и запазване на документи

#### Експортиране на празни параграфи до Markdown <sup>25.5</sup>

Възможността да се контролира как празните параграфи се експортират в Markdown е въведена чрез добавяне на [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownemptyparagraphexportmode/) изброяване и [EmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getEmptyParagraphExportMode) свойство.

#### Експортиране на документи от няколко страници в растерни формати на изображения <sup>25.6</sup>

Възможността за експортиране на документи от няколко страници в растерни формати на изображения (като PNG и JPEG) с [customizable layouts](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) – хоризонтални, вертикални или мрежови – е въведена чрез разширяване на функционалността за експортиране на изображения.

### Рендериране

#### Задаване на стила на диаграмата <sup>25.5</sup>

Възможността за задаване на стила на диаграмата е въведена чрез добавяне на [ChartStyle](https://reference.aspose.com/words/java/com.aspose.words/chartstyle/) изброяване и [Style](https://reference.aspose.com/words/java/com.aspose.words/chart/#getStyle) свойството.

#### Рендиране на съединителни линии в MathML изрази <sup>25.6</sup>

Рендирането на съединителните линии в MathML изрази е внедрено, за да се осигури по-точно и визуално последователно показване на математическите формули.

#### Създаване на Легенди за Водопадни диаграми <sup>25.6</sup>

Привеждането на легенди за ["Waterfall" charts](https://reference.aspose.com/words/java/com.aspose.words/chartseriestype/) е въведена, увеличаване на прозрачността на данните и подобряване на интерпретацията на тези диаграми.

### Друго

* Възможността за обвиване на математически формули, съдържащи множество наклонени черти, е подобрена, подобрявайки яснотата на оформлението и четливостта на формулата. <sup>25.6</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Java 25.5 бележки по изданието](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-5-release-notes/).

Научете повече за [Aspose.Words за Java 25.6 бележки по изданието](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words за Java 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 въвежда AI - захранва проверката на граматиката и подобрява записването на документи с разширени опции за формати HTML, SVG и Markdown.

Aspose.Words 25.2 въвежда обобщаване на текст с Anthropic AI модели, добавя MsWorks поддръжка на формат, подобрява типографския контрол и подобрява PDF структурата и обработката на списъци.

Aspose.Words 25.3 подобрява AI - захранва граматика Проверка и избор на шрифт със свойството UpdateAmbiguousTextFont, както и подобрява PDF прикачени файлове износ.

Aspose.Words 25.4 въвежда поддръжка за нови размери на хартията, позволява усъвършенстван HTML контрол на износа, подобрява обработката с водни знаци и подобрява използваемостта на LowCode API.

### AI - захранващи функции

#### Документ AI Проверка На Граматиката

* Възможността за проверка на граматиката на предоставения документ, използвайки OpenAI генеративни модели е въведена чрез добавяне на нов [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) метод. <sup>25.1</sup>
* Функцията за проверка на граматиката AI е актуализирана, за да поддържа всички модели, налични в списъка [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). <sup>25.3</sup>

#### Обобщаване Чрез Използване На Anthropic Генеративни Езикови Модели <sup>25.2</sup>

Обобщаването на текст с помощта на Anthropic генеративните езикови модели е разрешено чрез въвеждане на нов публичен клас [AnthropicAiModel](https://reference.aspose.com/words/java/com.aspose.words/anthropicaimodel/).

### Low Code

#### Low Code API ползваемост <sup>25.4</sup>

Въведени са значителни подобрения в използваемостта на **LowCode API**, опростяване на обработката на документи и намаляване на необходимостта от повтарящ се Код.

### Поддържани Формати <sup>25.2</sup>

От версия 25.2 е добавена съвместимост с новия формат MsWorks за зареждане на Microsoft работни документи.

### Конвертиране, зареждане и запазване на документи

#### Подобрено записване до HTML и SVG формати <sup>25.1</sup>

Записването във формати HTML и SVG е подобрено чрез добавяне на **IdPrefix** и **RemoveJavaScriptFromLinks** свойства както към класовете [HtmlFixedSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlfixedsaveoptions/), така и към класовете [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/).

#### Задайте разделителна способност на изображението и режим OfficeMath изход, когато записвате до Markdown <sup>25.1</sup>

* Към класа [ImageResolution](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImageResolution) е добавена нова опция [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/), За да зададете разделителната способност на изображението.
* Нова опция [OfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getOfficeMathExportMode) и [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownofficemathexportmode/) изброяване са добавени към класа [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/), за да се зададе OfficeMath изходен режим.
* Възможността за задаване на воден знак за изображение от поток е въведена чрез добавяне на ново претоварване към метода [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.io.InputStream-com.aspose.words.ImageWatermarkOptions). <sup>25.4</sup>

### Рендериране

#### Подобрен Типографски Контрол <sup>25.2</sup>

[NumberSpacing](https://reference.aspose.com/words/java/com.aspose.words/font/#getNumberSpacing) свойството е добавено за подобрен типографски контрол.

#### Контролиране на избора на шрифт за двусмислени знаци <sup>25.3</sup>

В класа [UpdateAmbiguousTextFont](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/#getUpdateAmbiguousTextFont) е добавена нова публична собственост [SaveOptions](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/), За да се контролира изборът на шрифт според използвания код на знака.

#### Опции За Размер На Хартията <sup>25.4</sup>

Възможността за използване на JIS B4 и JIS B5 е въведена чрез добавяне на нови стойности към изброяването [PaperSize](https://reference.aspose.com/words/java/com.aspose.words/papersize/).

#### HTML Контрол На Изхода <sup>25.4</sup>

Възможността за премахване на JavaScript от хипервръзка URLs по време на HTML износ е въведена чрез добавяне на свойство [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/#getRemoveJavaScriptFromLinks).

### Друго

* PDF логическата структура е подобрена с поддръжка на TOA, BIBLIOGRAPHY и INDEX полета. <sup>25.2</sup>
* [AddSingleLevelList](https://reference.aspose.com/words/java/com.aspose.words/listcollection/#addSingleLevelList-int) методът е въведен за по-добро боравене със списъка. <sup>25.2</sup>
* Добавено е ново свойство [AttachmentsEmbeddingMode](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getAttachmentsEmbeddingMode), за да замени **EmbedAttachments**, за да подобри експортирането на PDF прикачени файлове. Също така към списъка [PdfCompliance](https://reference.aspose.com/words/java/com.aspose.words/pdfcompliance/) са добавени нови стойности, за да се поддържат PDF/A прикачени файлове към версии. Освен това прикачените файлове вече се поддържат с криптиране. <sup>25.3</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Java 25.1 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-1-release-notes/).

Научете повече за [Aspose.Words за Java 25.2 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-2-release-notes/).

Научете повече за [Aspose.Words за Java 25.3 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-3-release-notes/).

Научете повече за [Aspose.Words за Java 25.4 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words за Java 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 въвежда group shape Вмъкване и StructuredDocumentTag Вмъкване чрез DocumentBuilder, подобрява рендирането на радиалната диаграма с градуации, подобрява цифровите подписи с поддръжка XAdES-EPES, добавя Markdown подчертаване и осигурява достъп до разделители на бележки под линия/бележка в края.

Aspose.Words 24.10 въвежда подобрена ActiveX поддръжка за контрол с CommandButton Създаване, нов контрол на видимостта на формата, възможност за group shapes, подобрен Markdown износ за таблици, форматиране на диаграми за Pie и Doughnut, по-добра работа с кодиране на големи 5 и поддръжка за остарели тайвански шрифтове.

Aspose.Words 24.11 въвежда AI - захранвано обобщаване на документи, подобрени опции за рендиране, подобрен достъп до свойствата на документа и ActiveX контрол на надписите.

Aspose.Words 24.12 въвежда Персонализируемо поставяне на етикети на данни, Гугъл AI-захранван превод на текст, подобрени опции за почистване Mail Merge и нови LowCode класове за обработка.

### AI - захранващи функции

#### Обобщаване на документи чрез OpenAI и Гугъл <sup>24.11</sup>

Интегрирана е поддръжка за обобщаване на документи, използвайки **OpenAI** и **Google** генеративни езикови модели.

#### Превод на текст с помощта на генеративните езикови модели на Гугъл <sup>24.12</sup>

Възможността за превод на текст с помощта на генеративните езикови модели на Гугъл е внедрена в Aspose.Words чрез добавяне на [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) метода и [Language](https://reference.aspose.com/words/java/com.aspose.words/language/) изброяването.

### Low Code <sup>24.12</sup>

Ново LowCode класове като [Comparer](https://reference.aspose.com/words/java/com.aspose.words/comparer/), [MailMerger](https://reference.aspose.com/words/java/com.aspose.words/mailmerger/), [Replacer](https://reference.aspose.com/words/java/com.aspose.words/replacer/), [Splitter](https://reference.aspose.com/words/java/com.aspose.words/splitter/) и т.н. е въведена, предлагайки набор от методи, които постигат перфектния баланс между простота и гъвкавост за обработка на документи.

### Рендериране и печат

#### Градуации по радиални карти <sup>24.9</sup>

Реализирано е рендиране на градуации по радиални карти.

#### CommandButton ActiveX контроли <sup>24.10</sup>

Възможността за създаване на CommandButton ActiveX контроли е въведена чрез добавяне на нов публичен метод [InsertForms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertForms2OleControl-com.aspose.words.Forms2OleControl) и нов публичен клас [Forms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/).

#### Контрол На Видимостта На Формата <sup>24.10</sup>

Добавена е нова обществена собственост [Hidden](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#getHidden), за да се контролира видимостта на фигурите.

#### Промени в Pie и Doughnut диаграми <sup>24.10</sup>

Няколко нови публични свойства са добавени към формат Pie и Doughnut диаграми.

#### Контролирайте рендирането на PDF граници на поле за избор на формуляр <sup>24.11</sup>

Въведена е нова опция за контрол на рендирането на PDF граници на полета на формуляр за избор чрез добавяне на нова публична опция [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getRenderChoiceFormFieldBorder).

#### Получаване и задаване на кодове за форматиране на данни от диаграми <sup>24.11</sup>

Възможността за получаване и задаване на кодове за форматиране на данни от диаграми е добавена чрез внедряване на свойството [FormatCode](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/#getFormatCode) в класовете [ChartXValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartyvaluecollection/) и [BubbleSizeCollection](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/).

#### Рендиране на хистограма диаграми с кошчета и етикети <sup>24.11</sup>

Рендирането на хистограмата е подобрено, като позволява определен брой кошчета и етикети.

### Конвертиране, зареждане и запазване на документи

#### Подчертаване на форматирането при зареждане Markdown файлове <sup>24.9</sup>

Опцията за разпознаване на форматирането на подчертаването при зареждане на документи Markdown е включена чрез добавяне на нова публична собственост [ImportUnderlineFormatting](https://reference.aspose.com/words/java/com.aspose.words/markdownloadoptions/#getImportUnderlineFormatting).

#### Експортиране на таблици като HTML при запис до Markdown <sup>24.10</sup>

Възможност за експортиране на таблици като HTML при записване на документи във формат Markdown е реализирана чрез добавяне на нова публична собственост [ExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getExportAsHtml) и изброяване [MarkdownExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownexportashtml/).

#### Експортиране PDF с актуализирана логическа структура <sup>24.11</sup>

PDF експортът е подобрен чрез включване на свойствата на заглавието на таблицата като PDF заглавия на елементите на логическата структура.

### Mail Merge и докладване

#### Премахване на празните маси по време на Mail Merge <sup>24.12</sup>

Към списъка **RemoveEmptyTables** е добавена нова опция [MailMergeCleanupOptions](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/), за да се прецизира Mail Merge изхода.

### Цифрови Подписи

#### Подписвайте документи с XAdES-EPES <sup>24.9</sup>

Възможността за подписване на документи с XAdES-EPES Ниво XML-DSig е въведена чрез добавяне на нова обществена собственост [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/signoptions/#getXmlDsigLevel) и ново публично изброяване [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/xmldsiglevel/)

### Друго

* Добавен е нов публичен метод [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-com.aspose.words.Shape...) към group shapes. <sup>24.9</sup>
* Добавен е нов публичен метод [InsertStructuredDocumentTag](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertStructuredDocumentTag-int), за да вмъкнете **StructuredDocumentTags** в документ. <sup>24.9</sup>
* Публичен достъп до разделители на бележки под линия/бележка в края е осигурен чрез добавяне на няколко публични класове и свойства. <sup>24.9</sup>
* Възможността за групиране на отделни фигури, group shapes заедно и директно групиране на фигури и group shapes е въведена чрез добавяне на [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-double-double-double-double-com.aspose.words.ShapeBase...) Метод. <sup>24.10</sup>
* Биг5 обработка на кодиране за TrueType таблица с изображения е подобрена. <sup>24.10</sup>
* Подкрепата за остарели тайвански шрифтове е подобрена. <sup>24.10</sup>
* За достъп до свойствата на разширения документ, свойствата само за четене са добавени към класа [BuiltInDocumentProperties](https://reference.aspose.com/words/java/com.aspose.words/builtindocumentproperties/). <sup>24.11</sup>
* Задаването на надписи за контроли ActiveX е разрешено чрез добавяне на нов публичен сетер към свойството [Forms2OleControl.Caption](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/#getCaption). <sup>24.11</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Java 24.9 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-9-release-notes/).

Научете повече за [Aspose.Words за Java 24.10 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-10-release-notes/).

Научете повече за [Aspose.Words за Java 24.11 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-11-release-notes/).

Научете повече за [Aspose.Words за Java 24.12 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words за Java 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 разширява опциите за сглобки, подобрява възможностите за рендиране и разширява някои други опции.

Aspose.Words 24.6 подобрява опциите за рендиране, подобрява функционалността за търсене и сравняване и разширява няколко други функции.

Aspose.Words 24.7 променя начина, по който работите с ActiveX, разширява възможностите за рендиране, както и експортирането към Markdown и XLSX формати.

Aspose.Words 24.8 подобрява персонализирането на диаграмите с прецизен контрол върху етикетите на осите, разширява управлението на шрифта, подобрява обработката на структурата на документите и добавя нови възможности за HTML/XAML износ, PDF функционалност, конвертиране на документи и цифрови подписи.

### Поддържани Формати

Като се започне от версия 24.7, Експортиране до PDF/UA-2 се поддържа, за да се осигури достъпност за потребители с увреждания.

### Рендериране и печат

#### Промени в диаграми, форми и DrawingML <sup>24.5</sup>

- DrawingML ефекти рендиране за SVG графики, разширяване на предишната функционалност, ограничена до изображения, е изпълнено.
- Поддръжка за създаване на комбо диаграми и коригиране на свойства като ширина на празнината, припокриване и мехурчеста скала в групи от серии е въведена чрез добавяне на класове [ChartSeriesGroup](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroup/) и [ChartSeriesGroupCollection](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroupcollection/) и свойство [SeriesGroups](https://reference.aspose.com/words/java/com.aspose.words/chart/#getSeriesGroups).
- Функционалността за манипулиране на SoftEdge ефекта на фигурите е реализирана чрез добавяне на [SoftEdgeFormat](https://reference.aspose.com/words/java/com.aspose.words/softedgeformat/) класа.
- Възможността за промяна на коригираните стойности на фигури е реализирана чрез добавяне на [AdjustmentCollection](https://reference.aspose.com/words/java/com.aspose.words/adjustmentcollection/) и [Adjustment](https://reference.aspose.com/words/java/com.aspose.words/adjustment/) публични класове и [Adjustments](https://reference.aspose.com/words/java/com.aspose.words/shape/#getAdjustments) собственост.

#### Промени в диаграми, форми и чертеж <sup>24.6</sup>

- Възможностите за картографиране са подобрени. Сега можете да създадете по-голямо разнообразие от диаграми, включително *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* диаграми, *Box & Whisker* диаграми, *Waterfalls* и *Funnels*. Това ви позволява да визуализирате данните си по по-разнообразен и информативен начин.
- Контролът на цветовете за форматиране на сенки е подобрен. Можете да получите по-прецизен контрол върху външния вид на вашите документи чрез достъп до цветове в сянка.
- Подобрението на производителността за фоново рендиране е подобрено. Можете значително да ускорите рендирането на фонове, съдържащи малки елементи, благодарение на естествената технология за облицоване.
- Добавени са реалистични градиенти за форми. Вече можете да създавате DML форми с нелинейни градиенти, имитирайки визуалния стил на Microsoft Word за по-полиран вид.

#### Персонализиране На Етикети За Данни На Диаграми <sup>24.7</sup>

Възможността за персонализиране на етикети на данни на диаграма, като **Orientation** и **Rotation** е добавена.

#### Потребителски номер стайлинг за списък нива <sup>24.7</sup>

Добавен е сетер за обществена собственост [CustomNumberStyleFormat](https://reference.aspose.com/words/java/com.aspose.words/listlevel/#getCustomNumberStyleFormat). Сега можете да дефинирате персонализиран номер за списъчни нива.

#### Промени в работата с ActiveX <sup>24.7</sup>

* Свойствата на ActiveX обектите вече могат да бъдат променяни, което ви дава по-голям контрол върху тяхното поведение.
* Добавена е възможността за промяна на стойността на контролата на радио бутона ActiveX, за да се даде възможност за динамично взаимодействие.
* Възможността да превключвате ActiveX checkbox на "проверено " или" неотбелязано " е добавена.

#### Контрол върху оста на диаграмата тик Етикети ориентация и въртене <sup>24.8</sup>

Прецизен контрол върху ориентацията и въртенето на етикетите на осите на диаграмата е добавен за по – удобно персонализиране на диаграмата-класът [AxisTickLabels](https://reference.aspose.com/words/java/com.aspose.words/axisticklabels/) е разширен с нови **Orientation** и **Rotation** свойства.

#### Замяна на наклонената черта със знака на йената <sup>24.8</sup>

Обратната съвместима HTML и XAML износ за замяна на обратно наклонената черта със знака на йената е подобрена. За да се постигне това, имотът **ReplaceBackslashWithYenSign** е добавен към класовете [HtmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/) и [XamlFlowSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/).

#### Използване на SDT етикети като имена на полета на формуляри при експортиране към PDF <sup>24.8</sup>

PDF експортирането с поддръжка за използване на SDT тагове като имена на полета на формуляри е подобрено чрез добавяне на ново свойство **UseSdtTagAsFormFieldName** към класа [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/).

### Конвертиране, зареждане и запазване на документи

#### Експортиране на връзки към Markdown формат <sup>24.7</sup>

Възможността да се контролира експортирането на връзки във формат Markdown е добавена чрез имплементацията на [LinkExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getLinkExportMode) свойството.

#### LowCode 24.8 <sup>24.8</sup>

Въведен е нов **LowCode.Converter** клас, предназначен да осигури набор от методи за конвертиране на различни типове документи с един ред код.

### Търсене и сравняване

#### Разширени Опции За Сравнение <sup>24.6</sup>

Добавена е възможността за рационализиране на работните потоци за анализ на данни с подобрена функционалност за сравнение. Това включва нова опция [IgnoreStoreItemId](https://reference.aspose.com/words/java/com.aspose.words/advancedcompareoptions/#getIgnoreStoreItemId) и преработен интерфейс за напреднали сравнения.

### Друго

* Функцията за премахване на празни страници от документ е реализирана чрез добавяне на метода [RemoveBlankPages](https://reference.aspose.com/words/java/com.aspose.words/document/#removeBlankPages). <sup>24.5</sup>
* Възможността да се провери за наличие на VBA макроси без зареждане на документ е осигурена чрез добавяне на свойство [HasMacros](https://reference.aspose.com/words/java/com.aspose.words/fileformatinfo/#hasMacros). <sup>24.5</sup>
* Поддържането на номериране на източника при вмъкване на документ с помощта на LINQ двигател за докладване вече се поддържа. <sup>24.5</sup>
* Добавено е ново [DateTimeUtc](https://reference.aspose.com/words/java/com.aspose.words/comment/#getDateTimeUtc) свойство-това осигурява по-точен времеви печат за коментари, подобряване на организацията и проследимостта. <sup>24.6</sup>
* Двигателят LINQ е подобрен. Селективно премахване на празни параграфи и дефиниране на персонализирани съобщения за липсващите членове на обекта са направени, което води до по-чисти и по-информативни отчети. <sup>24.6</sup>
* Форматът за дата и час сега автоматично се открива за безпроблемно експортиране във формат XLSX. <sup>24.7</sup>
* Добавена е обществена собственост [IsProtected](https://reference.aspose.com/words/java/com.aspose.words/vbaproject/#isProtected), която ви позволява да проверите дали даден проект VBA е защитен. <sup>24.7</sup>
* Информацията за шрифта е разширена със свойството **EmbeddingLicensingRights**, добавено към класовете [FontInfo](https://reference.aspose.com/words/java/com.aspose.words/fontinfo/) и [PhysicalFontInfo](https://reference.aspose.com/words/java/com.aspose.words/physicalfontinfo/). <sup>24.8</sup>
* Начин за ефективно изчистване на горни и долни колонтитули на секции при запазване на водните знаци е добавен за по-точно работа със структурата на документа. За да изчистите горни и долни колонтитули на секции, използвайте новия публичен метод **ClearHeadersFooters**. <sup>24.8</sup>
* Цифровото подписване на XPS документи с [XpsSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xpssaveoptions/) е активирано – за целта е добавено ново свойство **DigitalSignatureDetails**. <sup>24.8</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Java 24.5 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-5-release-notes/).

Научете повече за [Aspose.Words за Java 24.6 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-6-release-notes/).

Научете повече за [Aspose.Words за Java 24.7 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-7-release-notes/).

Научете повече за [Aspose.Words за Java 24.8 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words за Java 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 подобрява опита около управлението на цветовете на инсулт, подобрява OLE обекти и LINQ отчитане, както и въвежда нова библиография източници публично API.

Aspose.Words 24.2 разширени графики API, управление на стила и LINQ опции. Тази версия на Aspose.Words също така въведе възможността за задаване на SvgSaveOptions по време на рендиране, по-гъвкав контрол за зареждане Markdown файлове и работа с референтен текст за бележки под линия и бележки в края.

Aspose.Words 24.3 въвежда нов TIFF четец / писател и емулация на бинарни растерни операции за WMF метафили. Aspose.Words 24.3 също продължава да разширява класациите API.

Aspose.Words 24.4 подобрява записващите формати, някои опции за рендиране, както и подобрява работата с цифрови подписи.

### Поддържани Формати <sup>24.4</sup>

Модерният формат на изображението **WebP** сега се поддържа в Aspose.Words. Сега можете да четете и вмъквате WebP изображения в документи, както и да запазвате изображения във формат WebP.

### Рендериране и печат

#### Контрол На Цвета На Хода <sup>24.1</sup>

Класът [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) е разширен с набор от нови публични свойства, свързани с управлението на цветовете на ходовете: [ForeThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeThemeColor) и [BackThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackThemeColor), [ForeTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeTintAndShade) и [BackTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackTintAndShade).

#### DrawingML Диаграми API Разширение <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** продължава да се разширява.

#### Вграждане на шрифтове, обявени в @font-face правила <sup>24.4</sup>

Добавена е възможност за вграждане на шрифтове, декларирани в @font-face Правила в получените дефиниции на шрифта на документа, чрез добавяне на ново свойство [SupportFontFaceRules](https://reference.aspose.com/words/java/com.aspose.words/htmlloadoptions/#getSupportFontFaceRules).

#### Работа с форматиране на отблясъци и отражения <sup>24.4</sup>

Способността да се работи с блясък и отражение форматиране за чертеж обект е реализирана.

### Зареждане и съхранение на документи

#### Посочете SvgSaveOptions По Време На Рендирането <sup>24.2</sup>

Възможността за задаване на [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/) по време на рендирането е добавена с помощта на [ShapeRenderer](https://reference.aspose.com/words/java/com.aspose.words/shaperenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) и [OfficeMathRenderer](https://reference.aspose.com/words/java/com.aspose.words/officemathrenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) методи.

#### Запазване на празните редове при зареждане Markdown файлове <sup>24.2</sup>

Възможността за запазване на празни линии при зареждане Markdown файлове е добавена.

#### Ново TIFF Читател / Писател <sup>24.3</sup>

Създаден е нов TIFF читател/писател за Aspose.Words за .NET Standard, .NET 6 и по-късно. Aspose.Words за .NET 24.3 Добавена е поддръжка за четене TIFF изображения с JPEG и стари JPEG компресионни типове, а също така значително подобрява качеството на операциите за четене и запис.

### Друго

* Възможността за промяна на текста на `TextBox` OLE контролата е въведена чрез добавяне на ново свойство [Text](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/#getText) към новия клас [TextBoxControl](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/). 24.1 <sup>24.1</sup>
* Библиографията публични източници API е реализирана чрез добавяне на няколко нови [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/bibliography/), [Source](https://reference.aspose.com/words/java/com.aspose.words/source/), [ContributorCollection](https://reference.aspose.com/words/java/com.aspose.words/contributorcollection/), [Contributor](https://reference.aspose.com/words/java/com.aspose.words/contributor/), [Corporate](https://reference.aspose.com/words/java/com.aspose.words/corporate/), [PersonCollection](https://reference.aspose.com/words/java/com.aspose.words/personcollection/) и [Person](https://reference.aspose.com/words/java/com.aspose.words/person/) класове и [SourceType](https://reference.aspose.com/words/java/com.aspose.words/sourcetype/) изброяване, както и чрез добавяне на ново [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/document/#getBibliography) свойство към [Document](https://reference.aspose.com/words/java/com.aspose.words/document/) клас. <sup>24.1</sup>
* Предоставен е API за ограничаване на достъпа до членовете на типа, използвайки синтаксиса на шаблона за двигателя за докладване LINQ. <sup>24.1</sup>
* Нови публични свойства [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) и [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) за подобрено управление на стила са добавени към [Style](https://reference.aspose.com/words/net/aspose.words/style/) класа. <sup>24.2</sup>
* Функционалността за извличане на действителния текст на референтния знак за бележки под линия и бележки в края е подобрена със свойството [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) и метода [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* Съвместимостта с `Word 2016` диаграми за `LINQ Reporting Engine` е разрешена. <sup>24.2</sup>
* Въведена е емулация на бинарни растерни операции за WMF метафили. <sup>24.3</sup>
* Възможността за дефиниране на опции за подпис за документи в рамките на **SaveOptions** е разрешена чрез добавяне на нов клас [DigitalSignatureDetails](https://reference.aspose.com/words/java/com.aspose.words/digitalsignaturedetails/) с нови публични членове, както и добавяне на нови свойства към класовете [OoxmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/docsaveoptions/) и [OdtSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Java 24.1 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-1-release-notes/).

Научете повече за [Aspose.Words за Java 24.2 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-2-release-notes/).

Научете повече за [Aspose.Words за Java 24.3 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-3-release-notes/).

Научете повече за [Aspose.Words за Java 24.4 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words за Java 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 разширява опциите за рендиране, емулацията на рендиране на метаданни и markdown Опции за записване.

Aspose.Words 23.10 подобрява рендирането, разширява опциите за зареждане и записване на документи и позволява на потребителите да обединяват документи по нови начини.

Aspose.Words 23.11 подобрява работата с ревизии, XLSX формат и шрифтове на легендата на диаграмата с допълнителни опции.

Aspose.Words 23.12 въвежда нови свойства и изброявания за работа с PDF документи, поддръжка на WebP изображения и актуализирана библиотека на замъка.

### Рендериране и печат

#### Персонализиране на заглавията на осите в DrawingML диаграми <sup>23.9</sup>

Възможността за персонализиране на заглавията на осите в DrawingML диаграми е въведена чрез внедряването на нов публичен клас [ChartAxisTitle](https://reference.aspose.com/words/java/com.aspose.words/chartaxistitle/) и [Title](https://reference.aspose.com/words/java/com.aspose.words/chartaxis/#getTitle) собственост.

#### Определяне на вертикалната позиция на шрифтовете в абзац <sup>23.9</sup>

Сега е възможно да се определи вертикалната позиция на шрифтовете в рамките на абзац, като се използва новото публично свойство [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getBaselineAlignment) и новото изброяване [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/baselinealignment/).

#### Контрол На Цветовете На Преден План <sup>23.10</sup>

Възможността за извличане на цвета на преден план без модификатори е добавена към класовете [Fill](https://reference.aspose.com/words/java/com.aspose.words/fill/) и [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) чрез свойството **BaseForeColor**.

#### Разширяване на функционалността на графиките <sup>23.10</sup>

Функционалността на класовете [ChartDataPointCollection](https://reference.aspose.com/words/java/com.aspose.words/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/java/com.aspose.words/chartseries/) и [ChartFormat](https://reference.aspose.com/words/java/com.aspose.words/chartformat/) е разширена с нови методи и свойства.

#### Автоматично регулиране и поставяне на изображение във фигура <sup>23.10</sup>

Лесен начин за автоматично регулиране и поставяне на изображение в определена форма е предоставен чрез новия метод [FitImageToShape](https://reference.aspose.com/words/java/com.aspose.words/imagedata/#fitImageToShape).

#### Форматиране на шрифта по подразбиране за записи в Легендата на диаграмата DrawingML <sup>23.11</sup>

Възможността за задаване на форматиране на шрифта по подразбиране за записи в легендата на DrawingML диаграми е добавена чрез свойството **Font**. Тази функция улеснява по-опростен и последователен външен вид за елементите на диаграмата, подобрявайки цялостната естетика на документа.

#### Посочете оформлението на страницата при отваряне PDF в четец <sup>23.12</sup>

Възможността да се определи оформлението на страницата, което да се използва при отваряне на документ в четец PDF, е добавена чрез въвеждането на ново свойство [PageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getPageLayout) в класа [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/) и въвеждането на ново изброяване [PdfPageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfpagelayout/).

### Зареждане и съхранение на документи

#### Задаване на име на папка за изграждане на изображение URIs в Markdown <sup>23.9</sup>

Класът [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) е разширен чрез включване на свойството [ImagesFolderAlias](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImagesFolderAlias), което позволява да се зададе името на папката, използвана за конструиране на изображение URIs, написано в документа Markdown.

#### Намаляване PDF Изходния Размер <sup>23.10</sup>

Изпълнени са различни PDF оптимизации за рендиране, за да се намали размерът на изхода при използване на [OptimizeOutput](https://reference.aspose.com/words/java/com.aspose.words/fixedpagesaveoptions/#getOptimizeOutput) настройки.

#### Разпознаване на хипервръзки при зареждане TXT документи <sup>23.10</sup>

Функцията за разпознаване на хипервръзки при зареждане на документи TXT е внедрена чрез добавяне на ново свойство [DetectHyperlinks](https://reference.aspose.com/words/java/com.aspose.words/txtloadoptions/#getDetectHyperlinks).

### Друго

- Въведена е емулация на метафил за определяне на размера на растеризацията, по-специално за ширина на писалката WMF и ширина на козметичната писалка EMF. За да се постигне това, собствеността **ScaleWmfFontsToMetafileSize** е заменена с собственост [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPage) и собствеността [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPageResolution) е добавена. <sup>23.9</sup>
- Чрез метода [InsertDocumentInline](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertDocumentInline-com.aspose.words.Document-int-com.aspose.words.ImportFormatOptions) е въведен опростен метод за вмъкване на един документ в друг документ в текущата позиция на курсора. <sup>23.10</sup>
- Възможността за достъп и промяна на свойствата на стила е добавена чрез въвеждането на новата [Locked](https://reference.aspose.com/words/java/com.aspose.words/style/#getLocked) собственост. <sup>23.10</sup>
- Към методите от класа [CompositeNode](https://reference.aspose.com/words/java/com.aspose.words/compositenode/) е добавен общ тип параметър. <sup>23.10</sup>
- Начин да се контролира кога дадена ревизия трябва да бъде приета/отхвърлена или не, е бил приложен чрез използване на методите [Accept](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#accept-com.aspose.words.IRevisionCriteria) и [Reject](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#reject-com.aspose.words.IRevisionCriteria). Това подобрение дава на потребителите по-фин контрол върху процеса на преразглеждане. <sup>23.11</sup>
- Възможността да се напишат всички раздели на документ върху един и същ работен лист XLSX е предоставена чрез новото свойство [XlsxSectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsectionmode/) изброяване и новото [SectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/#getSectionMode). <sup>23.11</sup>
- Въведена е поддръжка за WebP изображение. Моля, имайте предвид, че тази функция е достъпна само за .NetStandart и .NET6+ версии. <sup>23.12</sup>

{{% alert color="primary" %}}

Научете повече за [Aspose.Words за Java 23.9 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-9-release-notes/).

Научете повече за [Aspose.Words за Java 23.10 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-10-release-notes/).

Научете повече за [Aspose.Words за Java 23.11 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-11-release-notes/).

Научете повече за [Aspose.Words за Java 23.12 Бележки За Издаване](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-12-release-notes/).

{{% /alert %}}

## Вижте Също

{{% alert color="primary" %}}

Тази страница съдържа последните новини за последните 2 години. За подробности относно предишните издания вижте [Бележки](https://releases.aspose.com/words/java/release-notes/) страници в съответните раздели.

{{% /alert %}}
