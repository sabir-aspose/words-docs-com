---
title: Що нового
second_title: Aspose.Words для .NET
articleTitle: Що нового в Aspose.Words для .NET
linktitle: Що нового в Aspose.Words для .NET
type: docs
description: "Aspose.Words для .NET з кожним днем розширюється і поліпшується сервіс. На цій сторінці ви можете дізнатися про найважливіші та найцікавіші можливості продукту."
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /uk/net/what-s-new-in-aspose-words-for-net/
timestamp: 2025-06-23-21-02-49
---

На цій сторінці описані найцікавіші нові функції Aspose.Words, що з'явилися в останніх версіях.

## Aspose.Words для .NET 25.5, 25.6

Aspose.Words 25.5 розширює можливості налаштування діаграм за допомогою нових варіантів оформлення і покращує Markdown експорт, надаючи можливість управляти обробкою порожніх абзаців.

Aspose.Words 25.6 покращує точність візуалізації та можливості візуалізації завдяки розширеним можливостям експорту зображень, покращеній обробці MathML та кращому представленню діаграм.

### Перетворення, завантаження та збереження документів

#### Експортуйте порожні абзаци в Markdown <sup>25.5</sup>

Можливість керувати тим, як порожні абзаци експортуються в Markdown, з'явилася завдяки додаванню перерахування [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownemptyparagraphexportmode/) і властивості [EmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/emptyparagraphexportmode/).

#### Експорт багатосторінкових документів у формати растрових зображень <sup>25.6</sup>

Можливість експорту багатосторінкових документів у формати растрових зображень (наприклад, PNG і JPEG) з [customizable layouts](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) - по горизонталі, вертикалі або сітці – з'явилася завдяки розширенню функціональності експорту зображень.

### Візуалізація

#### Налаштування стилю діаграми <sup>25.5</sup>

Можливість задавати стиль діаграми була реалізована шляхом додавання перерахування [ChartStyle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartstyle/) і властивості [Style](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/style/).

#### Відображення сполучних ліній у виразах MathML <sup>25.6</sup>

Для забезпечення більш точного і візуально несуперечливого відображення математичних формул був реалізований рендеринг сполучних ліній у виразах MathML.

#### Візуалізація умовних позначень для каскадних діаграм <sup>25.6</sup>

Була введена візуалізація умовних позначень для ["Waterfall" charts](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriestype/), що підвищує прозорість даних і покращує інтерпретованість цих діаграм.

### Інший

* Покращено можливість перенесення математичних формул, що містять кілька косих рис, що підвищує чіткість компонування і розбірливість формул. <sup>25.6</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для .NET 25.5 приміток до випуску](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-5-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 25.6 приміток до випуску](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words для .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 реалізована перевірка граматики на основі AI та покращено збереження документів завдяки розширеним параметрам для форматів HTML, SVG та Markdown.

Aspose.Words 25.2 введено Узагальнення тексту за допомогою Anthropic AI моделей, додана підтримка MsWorks форматів, поліпшений контроль типографіки і поліпшена структура PDF і обробка списків.

Aspose.Words 25.3 розширює можливості перевірки граматики на основі AI та вибору шрифту за допомогою властивості UpdateAmbiguousTextFont, а також покращує експорт вкладень на основі PDF.

Aspose.Words 25.4 реалізована підтримка нових форматів паперу, розширений експортний контроль HTML, поліпшена обробка водяних знаків і зручність використання LowCode API.

### AI - функціональні можливості

#### Перевірка граматики документа AI

* Можливість перевірки граматики наданого документа з використанням OpenAI генеруючих моделей була реалізована шляхом додавання нового методу [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/). <sup>25.1</sup>
* Функція перевірки граматики на основі AI була оновлена для підтримки всіх моделей, доступних у списку [AiModelType](https://reference.aspose.com/words/net/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Узагальнення з використанням Anthropic генеруючих мовних моделей <sup>25.2</sup>

Узагальнення тексту за допомогою моделей генеративної мови Anthropic стало можливим завдяки введенню нового загальнодоступного класу [AnthropicAiModel](https://reference.aspose.com/words/net/aspose.words.ai/anthropicaimodel/).

### Low Code

#### Low Code API зручність використання <sup>25.4</sup>

Були внесені значні поліпшення в зручність використання **LowCode API**, що спростило обробку документів і зменшило необхідність в повторюваному коді.

### Підтримувані формати <sup>25.2</sup>

Починаючи з версії 25.2, Додана сумісність з новим форматом завантаження MsWorks для робочих документів Microsoft.

### Перетворення, завантаження та збереження документів

#### Покращено збереження у форматах HTML та SVG <sup>25.1</sup>

Збереження у форматах HTML та SVG було покращено додаванням властивостей **IdPrefix** та **RemoveJavaScriptFromLinks** Як до класів [HtmlFixedSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlfixedsaveoptions/), так і [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/).

#### Встановіть роздільну здатність зображення та режим виводу OfficeMath при збереженні в Markdown <sup>25.1</sup>

* До класу [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) додано нову опцію [ImageResolution](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imageresolution/) для налаштування роздільної здатності зображення.
* У клас [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) були додані нова опція [OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/officemathexportmode/) і перерахування [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownofficemathexportmode/), щоб задати режим виведення OfficeMath.
* Можливість встановлення водяного знака на зображення з потоку була введена шляхом додавання нового перевантаження до методу [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage_2). <sup>25.4</sup>

### Візуалізація

#### Покращений типографський контроль <sup>25.2</sup>

Властивість [NumberSpacing](https://reference.aspose.com/words/net/aspose.words/font/numberspacing/) було додано для покращення управління типографікою.

#### Управління вибором шрифту для неоднозначних символів <sup>25.3</sup>

До класу [SaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/) додано нову загальнодоступну властивість [UpdateAmbiguousTextFont](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/updateambiguoustextfont/), що дозволяє керувати вибором шрифту відповідно до використовуваного коду символу.

#### Параметри формату паперу <sup>25.4</sup>

Можливість використання форматів паперу JIS B4 та JIS B5 була реалізована шляхом додавання нових значень до списку [PaperSize](https://reference.aspose.com/words/net/aspose.words/papersize/).

#### HTML управління виходом <sup>25.4</sup>

Можливість видалення JavaScript з гіперпосилання URLs під час експорту HTML була реалізована шляхом додавання властивості [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/removejavascriptfromlinks/).

### Інший

* PDF логічна структура була вдосконалена завдяки підтримці полів TOA, BIBLIOGRAPHY та INDEX. <sup>25.2</sup>
* Метод [AddSingleLevelList](https://reference.aspose.com/words/net/aspose.words.lists/listcollection/addsinglelevellist/) був введений для поліпшення роботи зі списками. <sup>25.2</sup>
* Додано нову властивість [AttachmentsEmbeddingMode](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/attachmentsembeddingmode/) замість **EmbedAttachments** для покращення експорту вкладень PDF. Крім того, до Списку [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) були додані нові значення для підтримки вкладень версії PDF/A. Крім того, вкладення тепер підтримуються за допомогою шифрування. <sup>25.3</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для .NET 25.1 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-1-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 25.2 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-2-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 25.3 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-3-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 25.4 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words для .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 додає вставку group shape і вставку StructuredDocumentTag за допомогою DocumentBuilder, покращує відображення радіальних діаграм за допомогою градуювань, покращує цифрові підписи з підтримкою XAdES-EPES, додає розпізнавання підкреслення Markdown і надає доступ до роздільників виносок/кінцевих приміток.

Aspose.Words 24.10 представлена розширена підтримка ActiveX елементів керування зі створенням CommandButton, новий елемент керування видимістю фігур, можливість group shapes, покращений експорт Markdown для таблиць, форматування діаграм для Pie та Doughnut діаграм, Покращена обробка кодувань Big5 та Підтримка застарілих Тайванські шрифти.

Aspose.Words 24.11 реалізована функція Узагальнення документів на основі AI, розширені можливості візуалізації, покращений доступ до властивостей документа і ActiveX Управління субтитрами.

Aspose.Words 24.12 представлені настроюється розміщення міток даних, переклад тексту за допомогою Google AI, розширені Mail Merge можливості очищення і нові LowCode класи обробки.

### AI - функціональні можливості

#### Узагальнення документів за допомогою OpenAI та Google <sup>24.11</sup>

Підтримка Узагальнення документів за допомогою моделей генеративної мови **OpenAI** та **Google** була інтегрована шляхом додавання простору імен [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) з його загальнодоступними членами.

#### Переклад тексту за допомогою генеративних мовних моделей Google <sup>24.12</sup>

Можливість перекладу тексту за допомогою моделей генеративної мови Google була реалізована в Aspose.Words шляхом додавання методу [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) та перерахування [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) у простір імен [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Були введені нові класи LowCode, такі як [Comparer](https://reference.aspose.com/words/net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/net/aspose.words.lowcode/splitter/) і т.д., які пропонують набір методів, що забезпечують ідеальний баланс між простотою і гнучкістю обробки документів.

### Рендеринг та друк

#### Градуювання на радіальних графіках <sup>24.9</sup>

Реалізовано рендеринг градацій на радіальних діаграмах.

#### CommandButton ActiveX елементи керування <sup>24.10</sup>

Можливість створення CommandButton ActiveX елементів керування була реалізована шляхом додавання нового загальнодоступного методу [InsertForms2OleControl](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertforms2olecontrol/) та нового загальнодоступного класу [Forms2OleControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/).

#### Контролюйте видимість фігури <sup>24.10</sup>

Додано нову загальнодоступну властивість [Hidden](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/hidden/) для контролю видимості фігур.

#### Зміни на графіках Pie і Doughnut <sup>24.10</sup>

До діаграм формату Pie та Doughnut було додано кілька нових загальнодоступних властивостей.

#### Керувати відображенням меж поля форми вибору PDF <sup>24.11</sup>

Нова опція для управління відображенням меж полів форми вибору PDF була реалізована шляхом додавання нової загальнодоступної опції [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/renderchoiceformfieldborder/).

#### Отримання та встановлення кодів формату для даних діаграми <sup>24.11</sup>

Можливість отримання та встановлення кодів формату для даних діаграми була додана шляхом реалізації властивості [FormatCode](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/formatcode/) у класах [ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/) та [BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/).

#### Візуалізація гістограмних графіків з осередками і написами <sup>24.11</sup>

Покращено рендеринг гістограмних діаграм за рахунок використання заданої кількості осередків і міток.

#### Налаштування розміщення міток даних <sup>24.12</sup>

Додана можливість налаштування розміщення міток даних шляхом додавання нових властивостей до класів [ChartDataLabel](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabel/) і [ChartDataLabelCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Перетворення, завантаження та збереження документів

#### Підкреслення форматування при завантаженні Markdown файлів <sup>24.9</sup>

Можливість розпізнавати форматування підкреслення під час завантаження документів Markdown була реалізована шляхом додавання нової загальнодоступної властивості [ImportUnderlineFormatting](https://reference.aspose.com/words/net/aspose.words.loading/markdownloadoptions/importunderlineformatting/).

#### Експорт таблиць як HTML при збереженні в Markdown <sup>24.10</sup>

Можливість експортувати таблиці у форматі HTML при збереженні документів у форматі Markdown була реалізована шляхом додавання нової загальнодоступної властивості [ExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/exportashtml/) та перерахування [MarkdownExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownexportashtml/).

#### Експорт PDF з оновленою логічною структурою <sup>24.11</sup>

PDF експорт було покращено, включивши властивості заголовка таблиці як заголовки елементів логічної структури PDF.

### Mail Merge та звітність

#### Видалити порожні таблиці протягом Mail Merge <sup>24.12</sup>

У перерахування [MailMergeCleanupOptions](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmergecleanupoptions/) був доданий новий параметр **RemoveEmptyTables** для уточнення вихідних даних Mail Merge.

### Цифрові підписи

#### Підписуйте документи за допомогою XAdES-EPES <sup>24.9</sup>

Можливість підписувати документи підписами рівня XAdES-EPES XML-DSig була введена шляхом додавання нової публічної властивості [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/signoptions/xmldsiglevel/) та нового публічного переліку [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/xmldsiglevel/).

### Інший

* До group shapes було додано новий загальнодоступний метод [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/). <sup>24.9</sup>
* Додано новий загальнодоступний метод [InsertStructuredDocumentTag](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertstructureddocumenttag/) для вставки **StructuredDocumentTags** у документ. <sup>24.9</sup>
* Відкритий доступ до розділювачів виносок і кінцевих приміток був забезпечений шляхом додавання декількох загальнодоступних класів і властивостей. <sup>24.9</sup>
* Можливість групувати окремі фігури, group shapes разом, а також безпосередньо групувати обидві фігури і group shapes з'явилася завдяки додаванню методу [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/#insertgroupshape_1). <sup>24.10</sup>
* Покращена обробка кодування Big5 для TrueType таблиць cmap. <sup>24.10</sup>
* Була покращена підтримка застарілих тайванських шрифтів. <sup>24.10</sup>
* Для доступу до розширених властивостей документа в клас [BuiltInDocumentProperties](https://reference.aspose.com/words/net/aspose.words.properties/builtindocumentproperties/) були додані властивості, доступні тільки для читання. <sup>24.11</sup>
* Налаштування підписів для елементів керування ActiveX було ввімкнено шляхом додавання нового загальнодоступного параметра Налаштування до властивості [Forms2OleControl.Caption](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для .NET 24.9 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-9-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 24.10 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-10-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 24.11 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-11-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 24.12 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words для .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 розширює можливості для збірок, покращує можливості рендеринга і розширює деякі інші можливості.

Aspose.Words 24.6 покращено параметри рендеринга, розширені можливості пошуку та порівняння, а також розширено ряд інших функцій.

Aspose.Words 24.7 змінює спосіб роботи з ActiveX, розширює можливості рендеринга, а також експорту в формати Markdown і XLSX.

Aspose.Words 24.8 розширює можливості налаштування діаграм за рахунок точного управління мітками осей, розширює можливості управління шрифтами, покращує роботу зі структурою документа і додає нові можливості для експорту HTML/XAML, функціональності PDF, перетворення документів і цифрових підписів.

### Підтримувані формати

Починаючи з версії 24.7, підтримується експорт в PDF/UA-2 для забезпечення доступності для користувачів з обмеженими можливостями.

### Платформа <sup>24.5</sup>

.NET 7.0/8.0 збірки були включені в пакет Aspose.Words NuGet.

### Рендеринг та друк

#### Зміни в графіках, фігурах і DrawingML <sup>24.5</sup>

* DrawingML реалізовано рендеринг ефектів для SVG графіки, що розширює попередню функціональність, обмежену зображеннями.
* Підтримка створення комбінованих діаграм та налаштування таких властивостей, як ширина проміжку, перекриття та бульбашковий масштаб у групах рядів була реалізована шляхом додавання класів [ChartSeriesGroup](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroup/) та [ChartSeriesGroupCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroupcollection/) та властивості [SeriesGroups](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/seriesgroups/).
* Функціональність для управління ефектом SoftEdge фігур була реалізована шляхом додавання класу [SoftEdgeFormat](https://reference.aspose.com/words/net/aspose.words.drawing/softedgeformat/).
* Можливість змінювати коригувальні значення фігур була реалізована шляхом додавання загальнодоступних класів [AdjustmentCollection](https://reference.aspose.com/words/net/aspose.words.drawing/adjustmentcollection/) і [Adjustment](https://reference.aspose.com/words/net/aspose.words.drawing/adjustment/) і властивості [Adjustments](https://reference.aspose.com/words/net/aspose.words.drawing/shape/adjustments/).

#### Зміни в діаграмах, фігурах і кресленнях <sup>24.6</sup>

* Можливості побудови графіків були розширені. Тепер ви можете створювати більш широкий спектр діаграм, включаючи *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* графіки, *Box & Whisker* діаграми, *Waterfalls* і *Funnels*. Це дозволяє візуалізувати ваші дані більш різноманітним та інформативним способом.
* Покращено управління кольором для форматування тіней. Ви можете отримати більш точний контроль над зовнішнім виглядом ваших документів, отримавши доступ до кольорів тіней.
* Покращена продуктивність при рендерингу фону. Ви можете значно прискорити рендеринг фону, що містить невеликі елементи, завдяки вбудованій технології тайлінгу.
* Додані реалістичні градієнти для фігур. Тепер ви можете створювати фігури DML з нелінійними градієнтами, імітуючи візуальний стиль Microsoft Word для надання їм більш досконалого вигляду.

#### Налаштування міток даних діаграми <sup>24.7</sup>

Додано Можливість налаштування міток даних діаграми, таких як **Orientation** та **Rotation**.

#### Користувальницький стиль нумерації для рівнів списку <sup>24.7</sup>

Додано параметр налаштування для властивості public [CustomNumberStyleFormat](https://reference.aspose.com/words/net/aspose.words.lists/listlevel/customnumberstyleformat/). Тепер ви можете задати користувальницький стиль нумерації для рівнів списку.

#### Зміни в роботі з ActiveX <sup>24.7</sup>

* Властивості об'єктів ActiveX тепер можна змінювати, що дає вам більше контролю над їх поведінкою.
* Додана можливість змінювати значення перемикача ActiveX для включення динамічної взаємодії.
* Додана можливість перемикати значення ActiveX checkbox на "перевірено" або "знято".

#### Управління орієнтацією і поворотом міток на осі графіка <sup>24.8</sup>

Для більш зручного налаштування графіка був доданий точний контроль над орієнтацією і поворотом міток відміток на осі графіка – клас [AxisTickLabels](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/) був розширений новими властивостями [Orientation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/orientation/) і [Rotation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/rotation/).

#### Заміна зворотної косої риси знаком ієни <sup>24.8</sup>

Покращено експорт із зворотною сумісністю HTML і XAML для заміни символу зворотної косої риски знаком ієни. Для досягнення цієї мети до класів [HtmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/) та [XamlFlowSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xamlflowsaveoptions/) було додано властивість **ReplaceBackslashWithYenSign**.

#### Використання тегів SDT Як імен полів форми при експорті в PDF <sup>24.8</sup>

PDF експорт із підтримкою Використання тегів SDT Як імен полів форми було розширено додаванням нової властивості [UseSdtTagAsFormFieldName](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/usesdttagasformfieldname/) до класу [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/).

### Перетворення, завантаження та збереження документів

#### Експорт посилань у формат Markdown <sup>24.7</sup>

Можливість керувати експортом посилань у форматі Markdown була додана завдяки реалізації властивості [LinkExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/linkexportmode/).

#### LowCode 24.8 <sup>24.8</sup>

Був представлений новий клас [LowCode.Converter](https://reference.aspose.com/words/net/aspose.words.lowcode/converter/), призначений для надання набору методів перетворення різних типів документів за допомогою одного рядка коду.

### Пошук та порівняння

#### Розширені параметри порівняння <sup>24.6</sup>
Додана можливість оптимізації робочих процесів аналізу даних з поліпшеною функціональністю порівняння. Це включає нову опцію [IgnoreStoreItemId](https://reference.aspose.com/words/net/aspose.words.comparing/advancedcompareoptions/ignorestoreitemid/) та перероблений інтерфейс для розширених порівнянь.

### Інший

* Функція видалення порожніх сторінок з документа була реалізована шляхом додавання методу [RemoveBlankPages](https://reference.aspose.com/words/net/aspose.words/document/removeblankpages/). <sup>24.5</sup>
* Можливість перевірки наявності макросів VBA без завантаження документа була надана шляхом додавання властивості [HasMacros](https://reference.aspose.com/words/net/aspose.words/fileformatinfo/hasmacros/). <sup>24.5</sup>
* Тепер підтримується збереження нумерації джерел при вставці документа за допомогою механізму створення звітів LINQ. <sup>24.5</sup>
* Додано нову властивість [DateTimeUtc](https://reference.aspose.com/words/net/aspose.words/comment/datetimeutc/) – вона забезпечує більш точну позначку часу для коментарів, покращуючи організацію та відстеження. <sup>24.6</sup>
* Покращено механізм створення звітів LINQ. Вибірково видалені порожні абзаци та визначені користувацькі повідомлення для відсутніх елементів об'єкта, що призвело до створення більш чистих та інформативних звітів. <sup>24.6</sup>
* Формат дати та часу тепер автоматично визначається для безперешкодного експорту у формат XLSX. <sup>24.7</sup>
* Додано загальнодоступну властивість [IsProtected](https://reference.aspose.com/words/net/aspose.words.vba/vbaproject/isprotected/), яка дозволяє перевірити, чи захищений проект VBA. <sup>24.7</sup>
* Інформація про Шрифт була розширена шляхом додавання властивості **EmbeddingLicensingRights** до класів [FontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/fontinfo/) та [PhysicalFontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* Для більш точної роботи зі структурою документа був доданий спосіб ефективного очищення верхніх і нижніх колонтитулів розділів зі збереженням водяних знаків. Щоб очистити верхні та нижні колонтитули розділів, використовуйте новий загальнодоступний метод [ClearHeadersFooters](https://reference.aspose.com/words/net/aspose.words/section/clearheadersfooters/). <sup>24.8</sup>
* Включено цифровий підпис XPS документів з використанням [XpsSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/) – для цієї мети додано нову властивість [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/digitalsignaturedetails/). <sup>24.8</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для .NET 24.5 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-5-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 24.6 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-6-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 24.7 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-7-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 24.8 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words для .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 покращено управління кольорами обведення, покращено OLE об'єкти та LINQ звіти, а також введено новий `Bibliography Sources` загальнодоступний API Інтерфейс.

Aspose.Words 24.2 розширені діаграми API, управління стилем і LINQ опції. У цій версії Aspose.Words також з'явилася можливість вказувати SvgSaveOptions під час рендеринга, більш гнучке управління завантаженням Markdown файлів і робота з посилальним текстом для виносок і кінцевих приміток.

Aspose.Words 24.3 представлений новий TIFF Режим читання/запису та емуляція бінарних растрових операцій для WMF метафайлів. Aspose.Words 24.3 також продовжує розширювати діаграми API.

Aspose.Words 24.4 розширені формати збереження, деякі параметри рендеринга, а також поліпшена робота з цифровими підписами.

### Підтримувані формати <sup>24.4</sup>

Сучасний формат зображення **WebP** тепер підтримується в Aspose.Words для .NET Framework 4.6.2 і вище. Тепер ви можете читати та вставляти WebP зображення в документи, а також зберігати зображення у форматі WebP.

Зверніть увагу, що WebP наразі доступний лише у версіях .NET Standard та .NET Framework v4.6.2 та вище.

### Рендеринг та друк

#### Управління кольором обведення <sup>24.1</sup>

Клас [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) був розширений набором нових загальнодоступних властивостей, пов'язаних з Керуванням кольорами обведення: [ForeThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/forethemecolor/) і [BackThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/foretintandshade/) і [BackTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backtintandshade/).

#### DrawingML розширення графіків API <sup>24.2 / 24.3 / 24.4</sup>

Параметр **DrawingML Charts API** продовжує розширюватися.

#### Вставити шрифти, оголошені в правилах @font-face <sup>24.4</sup>

Додана можливість вбудовувати шрифти, оголошені в правилах @font-face, в визначення шрифтів результуючого документа була введена шляхом додавання нової властивості [SupportFontFaceRules](https://reference.aspose.com/words/net/aspose.words.loading/htmlloadoptions/supportfontfacerules/).

#### Робота з форматуванням світіння і відображення <sup>24.4</sup>

Реалізована можливість роботи з форматуванням світіння і відображення для об'єкта малювання.

### Завантаження та збереження документів

#### Вкажіть SvgSaveOptions під час рендеринга <sup>24.2</sup>

Додана можливість вказувати [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/) під час рендеринга з використанням методів [ShapeRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) і [OfficeMathRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/).

#### Зберігати порожні рядки при завантаженні Markdown файлів <sup>24.2</sup>

Додана можливість зберігати порожні рядки при завантаженні файлів Markdown.

#### Новий користувач TIFF для читання / запису <sup>24.3</sup>

Розроблено новий TIFF модуль читання / запису для Aspose.Words .NET Standard, .NET 6 і пізніших версій. Aspose.Words для .NET 24.3 додана підтримка читання TIFF зображень з JPEG і старими типами стиснення JPEG, а також значно покращено якість операцій читання і запису.

### Інший

* Можливість змінювати текст елемента керування `TextBox` OLE була реалізована шляхом додавання нової властивості [Text](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/text/) до нового класу [TextBoxControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/). <sup>24.1</sup>
* Загальнодоступні джерела бібліографії API були реалізовані шляхом додавання нового простору імен [Aspose.Words.Bibliography](https://reference.aspose.com/words/net/aspose.words.bibliography/) з його новими класами та перерахуваннями, а також шляхом додавання нової властивості [Bibliography](https://reference.aspose.com/words/net/aspose.words/document/bibliography/) до класу [Document](https://reference.aspose.com/words/net/aspose.words/document/). <sup>24.1</sup>
* Було надано API для обмеження доступу до елементів типу за допомогою синтаксису шаблону для `LINQ Reporting Engine`. <sup>24.1</sup>
* Клас [Style](https://reference.aspose.com/words/net/aspose.words/style/) додав нові загальнодоступні властивості [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) та [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) для вдосконаленого управління стилем. <sup>24.2</sup>
* Функціональність для отримання фактичного тексту опорного знака для виносок і кінцевих виносок була розширена за допомогою властивості [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) і методу [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* Включена сумісність з графіками `Word 2016` для `LINQ Reporting Engine`. <sup>24.2</sup>
* Реалізована емуляція бінарних растрових операцій для метафайлів WMF. <sup>24.3</sup>
* Можливість визначення параметрів підпису для документів у межах **SaveOptions** була включена шляхом додавання нового класу [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/digitalsignaturedetails/) з новими відкритими членами, а також додавання нових властивостей до класів [OoxmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/docsaveoptions/) та [OdtSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для .NET 24.1 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-1-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 24.2 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-2-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 24.3 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-3-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 24.4 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words для .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 розширює можливості рендеринга, емуляції рендеринга метафайлів і markdown збереження.

Aspose.Words 23.10 покращено рендеринг, розширені можливості завантаження і збереження документів, а також користувачі можуть по-новому об'єднувати документи.

Aspose.Words 23.11 розширює можливості роботи зі змінами, XLSX форматуванням і шрифтами в легенді діаграми за допомогою додаткових опцій.

Aspose.Words 23.12 додані нові властивості і перерахування для роботи з PDF і OOXML документами, а також підтримка WebP зображень.

### Рендеринг та друк

#### Налаштування назв осей в DrawingML діаграмах <sup>23.9</sup>

Можливість налаштовувати назви осей на діаграмах DrawingML з'явилася завдяки впровадженню нової властивості public class [ChartAxisTitle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxistitle/) і [Title](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxis/title/).

#### Визначення вертикального розташування шрифтів в абзаці <sup>23.9</sup>

Тепер можна визначати вертикальне розташування шрифтів в абзаці, використовуючи нову властивість public [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/paragraphformat/baselinealignment/) і нове перерахування [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/baselinealignment/).

#### Управління кольором переднього плану <sup>23.10</sup>

Можливість витягувати колір переднього плану без модифікаторів була додана до класів [Fill](https://reference.aspose.com/words/net/aspose.words.drawing/fill/) та [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) за допомогою властивості **BaseForeColor**.

#### Розширення функціональності графіків <sup>23.10</sup>

Функціональність класів [ChartDataPointCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseries/) та [ChartFormat](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartformat/) була розширена новими методами та властивостями.

#### Автоматична настройка і підгонка зображення під форму <sup>23.10</sup>

Новий метод [FitImageToShape](https://reference.aspose.com/words/net/aspose.words.drawing/imagedata/fitimagetoshape/) надає простий спосіб автоматичної настройки і підгонки зображення під певну форму.

#### Форматування шрифту за замовчуванням для DrawingML записів в умовних позначеннях діаграми <sup>23.11</sup>

Додана можливість задавати форматування шрифту за замовчуванням для записів умовних позначень діаграм DrawingML за допомогою властивості [Font](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartlegend/font/). Ця функція забезпечує більш впорядкований і однаковий зовнішній вигляд елементів діаграми, покращуючи загальну естетику документа.

#### Вкажіть макет сторінки під час відкриття PDF у Reader <sup>23.12</sup>

Можливість вказувати макет сторінки, який буде використовуватися при відкритті документа в PDF рідері, була додана завдяки введенню нового властивості [PageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/pagelayout/) для класу [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) і нового перерахування [PdfPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfpagelayout/).

### Завантаження та збереження документів

#### Вказівка імені папки для створення зображення URIs в Markdown <sup>23.9</sup>

Клас [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) було розширено додаванням властивості [ImagesFolderAlias](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imagesfolderalias/), що дозволяє вказати назву папки, яка використовується для створення зображення URIs, записаного в документ Markdown.

#### Зменшити PDF Розмір вихідних даних <sup>23.10</sup>

Були реалізовані різні оптимізації PDF рендеринга для зменшення розміру вихідних даних при використанні налаштувань [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/).

#### Розпізнавати гіперпосилання при завантаженні TXT документів <sup>23.10</sup>

Функція розпізнавання гіперпосилань при завантаженні документів TXT була реалізована шляхом додавання нової властивості [DetectHyperlinks](https://reference.aspose.com/words/net/aspose.words.loading/txtloadoptions/detecthyperlinks/).

### Інший

* Реалізована емуляція рендеринга метафайлів для визначення розміру растеризації, зокрема, для WMF ширини пера і EMF косметичної ширини пера. Для досягнення цієї мети властивість **ScaleWmfFontsToMetafileSize** було замінено властивістю [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpage/) і додано властивість [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpageresolution/). <sup>23.9</sup>
* З використанням методу [InsertDocumentInline](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertdocumentinline/) був представлений спрощений метод вставки одного документа в інший в поточному положенні курсору. <sup>23.10</sup>
* Можливість доступу до властивостей стилю і їх зміни була додана завдяки введенню нового властивості [Locked](https://reference.aspose.com/words/net/aspose.words/style/locked/). <sup>23.10</sup>
* До методів класу [CompositeNode](https://reference.aspose.com/words/net/aspose.words/compositenode/) був доданий параметр універсального типу. <sup>23.10</sup>
* За допомогою методів [Accept](https://reference.aspose.com/words/net/aspose.words/revisioncollection/accept/) і [Reject](https://reference.aspose.com/words/net/aspose.words/revisioncollection/reject/) був реалізований спосіб контролю того, коли певна редакція повинна бути прийнята/відхилена чи ні. Це вдосконалення надає користувачам більш точний контроль над процесом внесення змін. <sup>23.11</sup>
* Можливість записувати всі розділи документа на один і той же робочий лист XLSX була надана завдяки новому типу перерахування [XlsxSectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsectionmode/) і Новій властивості [SectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsaveoptions/sectionmode/). <sup>23.11</sup>
* Спосіб управління тим, як розширення формату ZIP64 будуть використовуватися для документів OOXML, був реалізований за допомогою нової властивості Zip64Mode класу `OoxmlSaveOptions` та нового переліку Zip64Mode. <sup>23.12</sup>
* Додана підтримка зображень WebP. Будь ласка, зверніть увагу, що ця функція доступна тільки для версій .NetStandart і .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для .NET 23.9 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-9-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 23.10 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-10-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 23.11 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-11-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 23.12 примітки до випуску](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-12-release-notes/).

{{% /alert %}}

## Дивіться також

{{% alert color="primary" %}}

На цій сторінці представлені останні новини про релізи за останні 2 роки. Більш детальну інформацію про попередні випуски дивіться в [Примітки до випуску'](https://releases.aspose.com/words/net/release-notes/) сторінки у відповідних розділах.

{{% /alert %}}
