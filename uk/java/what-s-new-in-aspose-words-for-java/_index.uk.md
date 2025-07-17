---
title: Що нового
second_title: Aspose.Words для Java
articleTitle: Що нового в Aspose.Words для Java
linktitle: Що нового в Aspose.Words для Java
type: docs
description: "Aspose.Words для Java з кожним днем розширюється і поліпшується сервіс. На цій сторінці ви можете дізнатися про найважливіші та найцікавіші можливості продукту."
weight: 2
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /uk/java/what-s-new-in-aspose-words-for-java/
timestamp: 2025-06-23-21-02-49
---

На цій сторінці описані найцікавіші нові функції Aspose.Words, що з'явилися в останніх версіях.

## Aspose.Words для Java 25.5, 25.6

Aspose.Words 25.5 розширює можливості налаштування діаграм за допомогою нових варіантів оформлення і покращує Markdown експорт, надаючи можливість управляти обробкою порожніх абзаців.

Aspose.Words 25.6 покращує точність візуалізації та можливості візуалізації завдяки розширеним можливостям експорту зображень, покращеній обробці MathML та кращому представленню діаграм.

### Перетворення, завантаження та збереження документів

#### Експортуйте порожні абзаци в Markdown <sup>25.5</sup>

Можливість керувати тим, як порожні абзаци експортуються в Markdown, з'явилася завдяки додаванню перерахування [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownemptyparagraphexportmode/) і властивості [EmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getEmptyParagraphExportMode).

#### Експорт багатосторінкових документів у формати растрових зображень <sup>25.6</sup>

Можливість експорту багатосторінкових документів у формати растрових зображень (наприклад, PNG і JPEG) з [customizable layouts](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) - по горизонталі, вертикалі або сітці – з'явилася завдяки розширенню функціональності експорту зображень.

### Візуалізація

#### Налаштування стилю діаграми <sup>25.5</sup>

Можливість задавати стиль діаграми була реалізована шляхом додавання перерахування [ChartStyle](https://reference.aspose.com/words/java/com.aspose.words/chartstyle/) і властивості [Style](https://reference.aspose.com/words/java/com.aspose.words/chart/#getStyle).

#### Відображення сполучних ліній у виразах MathML <sup>25.6</sup>

Для забезпечення більш точного і візуально несуперечливого відображення математичних формул був реалізований рендеринг сполучних ліній у виразах MathML.

#### Візуалізація умовних позначень для каскадних діаграм <sup>25.6</sup>

Була введена візуалізація умовних позначень для ["Waterfall" charts](https://reference.aspose.com/words/java/com.aspose.words/chartseriestype/), що підвищує прозорість даних і покращує інтерпретованість цих діаграм.

### Інший

* Покращено можливість перенесення математичних формул, що містять кілька косих рис, що підвищує чіткість компонування і розбірливість формул. <sup>25.6</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Java приміток до випуску 25.5](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-5-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java приміток до випуску 25.6](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words для Java 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 реалізована перевірка граматики на основі AI та покращено збереження документів завдяки розширеним параметрам для форматів HTML, SVG та Markdown.

Aspose.Words 25.2 введено Узагальнення тексту за допомогою Anthropic AI моделей, додана підтримка MsWorks форматів, поліпшений контроль типографіки і поліпшена структура PDF і обробка списків.

Aspose.Words 25.3 розширює можливості перевірки граматики на основі AI та вибору шрифту за допомогою властивості UpdateAmbiguousTextFont, а також покращує експорт вкладень на основі PDF.

Aspose.Words 25.4 додана підтримка нових форматів паперу, розширений експортний контроль HTML, Покращена обробка водяних знаків та зручність використання LowCode API.

### AI - функціональні можливості

#### Перевірка граматики документа AI

* Можливість перевірки граматики наданого документа з використанням OpenAI генеруючих моделей була реалізована шляхом додавання нового методу [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions). <sup>25.1</sup>
* Функція перевірки граматики на основі AI була оновлена для підтримки всіх моделей, доступних у списку [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). <sup>25.3</sup>

#### Узагальнення з використанням Anthropic генеруючих мовних моделей <sup>25.2</sup>

Узагальнення тексту за допомогою моделей генеративної мови Anthropic стало можливим завдяки введенню нового загальнодоступного класу [AnthropicAiModel](https://reference.aspose.com/words/java/com.aspose.words/anthropicaimodel/).

### Low Code

#### Low Code API зручність використання <sup>25.4</sup>

Були внесені значні поліпшення в зручність використання **LowCode API**, що спростило обробку документів і зменшило необхідність в повторюваному коді.

### Підтримувані формати <sup>25.2</sup>

Починаючи з версії 25.2, Додана сумісність з новим форматом завантаження MsWorks для робочих документів Microsoft.

### Перетворення, завантаження та збереження документів

#### Покращено збереження у форматах HTML та SVG <sup>25.1</sup>

Збереження у форматах HTML та SVG було покращено додаванням властивостей **IdPrefix** та **RemoveJavaScriptFromLinks** Як до класів [HtmlFixedSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlfixedsaveoptions/), так і [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/).

#### Встановіть роздільну здатність зображення та режим виводу OfficeMath при збереженні в Markdown <sup>25.1</sup>

* До класу [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) додано нову опцію [ImageResolution](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImageResolution) для налаштування роздільної здатності зображення.
* У клас [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) були додані нова опція [OfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getOfficeMathExportMode) і перерахування [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownofficemathexportmode/), щоб задати режим виведення OfficeMath.
* Можливість встановлення водяного знака на зображення з потоку була введена шляхом додавання нового перевантаження до методу [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.io.InputStream-com.aspose.words.ImageWatermarkOptions). <sup>25.4</sup>

### Візуалізація

#### Покращений типографський контроль <sup>25.2</sup>

Властивість [NumberSpacing](https://reference.aspose.com/words/java/com.aspose.words/font/#getNumberSpacing) було додано для покращення управління типографікою.

#### Управління вибором шрифту для неоднозначних символів <sup>25.3</sup>

До класу [SaveOptions](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/) додано нову загальнодоступну властивість [UpdateAmbiguousTextFont](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/#getUpdateAmbiguousTextFont), що дозволяє керувати вибором шрифту відповідно до використовуваного коду символу.

#### Параметри формату паперу <sup>25.4</sup>

Можливість використання форматів паперу JIS B4 та JIS B5 була реалізована шляхом додавання нових значень до списку [PaperSize](https://reference.aspose.com/words/java/com.aspose.words/papersize/).

#### HTML управління виходом <sup>25.4</sup>

Можливість видалення JavaScript з гіперпосилання URLs під час експорту HTML була реалізована шляхом додавання властивості [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/#getRemoveJavaScriptFromLinks).

### Інший

* PDF логічна структура була вдосконалена завдяки підтримці полів TOA, BIBLIOGRAPHY та INDEX. <sup>25.2</sup>
* Метод [AddSingleLevelList](https://reference.aspose.com/words/java/com.aspose.words/listcollection/#addSingleLevelList-int) був введений для поліпшення роботи зі списками. <sup>25.2</sup>
* Додано нову властивість [AttachmentsEmbeddingMode](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getAttachmentsEmbeddingMode) замість **EmbedAttachments** для покращення експорту вкладень PDF. Крім того, до Списку [PdfCompliance](https://reference.aspose.com/words/java/com.aspose.words/pdfcompliance/) були додані нові значення для підтримки вкладень версії PDF/A. Крім того, вкладення тепер підтримуються за допомогою шифрування. <sup>25.3</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Java 25.1 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-1-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 25.2 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-2-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 25.3 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-3-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 25.4 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words для Java 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 додає вставку group shape і вставку StructuredDocumentTag за допомогою DocumentBuilder, покращує відображення радіальних діаграм за допомогою градуювань, покращує цифрові підписи з підтримкою XAdES-EPES, додає розпізнавання підкреслення Markdown і надає доступ до роздільників виносок/кінцевих приміток.

Aspose.Words 24.10 представлена розширена підтримка елементів керування ActiveX зі створенням CommandButton, новий елемент керування видимістю фігур, можливість group shapes, покращений експорт Markdown для таблиць, форматування діаграм для Pie та Doughnut діаграм, Покращена обробка кодувань Big5 та Підтримка застарілих Тайванські шрифти.

Aspose.Words 24.11 реалізована функція Узагальнення документів на основі AI, розширені можливості візуалізації, поліпшений доступ до властивостей документа і ActiveX Управління субтитрами.

Aspose.Words 24.12 представлені настроюється розміщення міток даних, переклад тексту за допомогою Google AI, розширені Mail Merge можливості очищення і нові LowCode класи обробки.

### AI - функціональні можливості

#### Узагальнення документів за допомогою OpenAI та Google <sup>24.11</sup>

Була інтегрована підтримка Узагальнення документів з використанням моделей генеративної мови **OpenAI** та **Google**.

#### Переклад тексту за допомогою генеративних мовних моделей Google <sup>24.12</sup>

Можливість перекладу тексту за допомогою генеративних мовних моделей Google була реалізована в Aspose.Words шляхом додавання методу [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) та перерахування [Language](https://reference.aspose.com/words/java/com.aspose.words/language/).

### Low Code <sup>24.12</sup>

Були введені нові класи LowCode, такі як [Comparer](https://reference.aspose.com/words/java/com.aspose.words/comparer/), [MailMerger](https://reference.aspose.com/words/java/com.aspose.words/mailmerger/), [Replacer](https://reference.aspose.com/words/java/com.aspose.words/replacer/), [Splitter](https://reference.aspose.com/words/java/com.aspose.words/splitter/) і т.д., які пропонують набір методів, що забезпечують ідеальний баланс між простотою і гнучкістю обробки документів.

### Рендеринг та друк

#### Градуювання на радіальних графіках <sup>24.9</sup>

Реалізовано рендеринг градацій на радіальних діаграмах.

#### CommandButton ActiveX елементи керування <sup>24.10</sup>

Можливість створювати CommandButton ActiveX елементів управління з'явилася завдяки додаванню нового загальнодоступного методу [InsertForms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertForms2OleControl-com.aspose.words.Forms2OleControl) і нового загальнодоступного класу [Forms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/).

#### Контролюйте видимість фігури <sup>24.10</sup>

Додано нову загальнодоступну властивість [Hidden](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#getHidden) для контролю видимості фігур.

#### Зміни на графіках Pie і Doughnut <sup>24.10</sup>

До діаграм формату Pie та Doughnut було додано кілька нових загальнодоступних властивостей.

#### Керувати відображенням меж поля форми вибору PDF <sup>24.11</sup>

Нова опція для управління відображенням меж полів форми вибору PDF була реалізована шляхом додавання нової загальнодоступної опції [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getRenderChoiceFormFieldBorder).

#### Отримання та встановлення кодів формату для даних діаграми <sup>24.11</sup>

Можливість отримання та встановлення кодів формату для даних діаграми була додана шляхом реалізації властивості [FormatCode](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/#getFormatCode) у класах [ChartXValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartyvaluecollection/) та [BubbleSizeCollection](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/).

#### Візуалізація гістограмних графіків з осередками і написами <sup>24.11</sup>

Покращено рендеринг гістограмних діаграм за рахунок використання заданої кількості осередків і міток.

### Перетворення, завантаження та збереження документів

#### Підкреслення форматування при завантаженні Markdown файлів <sup>24.9</sup>

Можливість розпізнавати форматування підкреслення під час завантаження документів Markdown була реалізована шляхом додавання нової загальнодоступної властивості [ImportUnderlineFormatting](https://reference.aspose.com/words/java/com.aspose.words/markdownloadoptions/#getImportUnderlineFormatting).

#### Експорт таблиць як HTML при збереженні в Markdown <sup>24.10</sup>

Можливість експортувати таблиці у форматі HTML при збереженні документів у форматі Markdown була реалізована шляхом додавання нової загальнодоступної властивості [ExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getExportAsHtml) та перерахування [MarkdownExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownexportashtml/).

#### Експорт PDF з оновленою логічною структурою <sup>24.11</sup>

PDF експорт було покращено, включивши властивості заголовка таблиці як заголовки елементів логічної структури PDF.

### Mail Merge та звітність

#### Видалити порожні таблиці протягом Mail Merge <sup>24.12</sup>

У перерахування [MailMergeCleanupOptions](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/) був доданий новий параметр **RemoveEmptyTables** для уточнення вихідних даних Mail Merge.

### Цифрові підписи

#### Підписуйте документи за допомогою XAdES-EPES <sup>24.9</sup>

Можливість підписувати документи підписами рівня XAdES-EPES XML-DSig була введена шляхом додавання нової публічної властивості [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/signoptions/#getXmlDsigLevel) та нового публічного переліку [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/xmldsiglevel/)

### Інший

* До group shapes було додано новий загальнодоступний метод [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-com.aspose.words.Shape...). <sup>24.9</sup>
* Додано новий загальнодоступний метод [InsertStructuredDocumentTag](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertStructuredDocumentTag-int) для вставки **StructuredDocumentTags** у документ. <sup>24.9</sup>
* Відкритий доступ до розділювачів виносок і кінцевих приміток був забезпечений шляхом додавання декількох загальнодоступних класів і властивостей. <sup>24.9</sup>
* Можливість групувати окремі фігури, group shapes разом, а також безпосередньо групувати обидві фігури і group shapes з'явилася завдяки додаванню методу [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-double-double-double-double-com.aspose.words.ShapeBase...). <sup>24.10</sup>
* Покращена обробка кодування Big5 для TrueType таблиць cmap. <sup>24.10</sup>
* Була покращена підтримка застарілих тайванських шрифтів. <sup>24.10</sup>
* Для доступу до розширених властивостей документа в клас [BuiltInDocumentProperties](https://reference.aspose.com/words/java/com.aspose.words/builtindocumentproperties/) були додані властивості, доступні тільки для читання. <sup>24.11</sup>
* Налаштування підписів для елементів керування ActiveX було ввімкнено шляхом додавання нового загальнодоступного параметра Налаштування до властивості [Forms2OleControl.Caption](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/#getCaption). <sup>24.11</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Java 24.9 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-9-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 24.10 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-10-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 24.11 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-11-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 24.12 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words для Java 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 розширює можливості для збірок, покращує можливості рендеринга і розширює деякі інші можливості.

Aspose.Words 24.6 покращено параметри рендеринга, розширені можливості пошуку та порівняння, а також розширено ряд інших функцій.

Aspose.Words 24.7 змінює спосіб роботи з ActiveX, розширює можливості рендеринга, а також експорту в формати Markdown і XLSX.

Aspose.Words 24.8 розширює можливості налаштування діаграм за рахунок точного управління мітками осей, розширює можливості управління шрифтами, покращує роботу зі структурою документа і додає нові можливості для експорту HTML/XAML, функціональності PDF, перетворення документів і цифрових підписів.

### Підтримувані формати

Починаючи з версії 24.7, підтримується експорт в PDF/UA-2 для забезпечення доступності для користувачів з обмеженими можливостями.

### Рендеринг та друк

#### Зміни в графіках, фігурах і DrawingML <sup>24.5</sup>

- DrawingML реалізовано рендеринг ефектів для SVG графіки, що розширює попередню функціональність, обмежену зображеннями.
- Підтримка створення комбінованих діаграм і налаштування таких властивостей, як ширина проміжку, перекриття і бульбашковий масштаб, в групах рядів була реалізована шляхом додавання класів [ChartSeriesGroup](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroup/) і [ChartSeriesGroupCollection](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroupcollection/), а також властивості [SeriesGroups](https://reference.aspose.com/words/java/com.aspose.words/chart/#getSeriesGroups).
- Функціональність для управління ефектом SoftEdge фігур була реалізована шляхом додавання класу [SoftEdgeFormat](https://reference.aspose.com/words/java/com.aspose.words/softedgeformat/).
- Можливість змінювати коригувальні значення фігур була реалізована шляхом додавання загальнодоступних класів [AdjustmentCollection](https://reference.aspose.com/words/java/com.aspose.words/adjustmentcollection/) і [Adjustment](https://reference.aspose.com/words/java/com.aspose.words/adjustment/) і властивості [Adjustments](https://reference.aspose.com/words/java/com.aspose.words/shape/#getAdjustments).

#### Зміни в діаграмах, фігурах і кресленнях <sup>24.6</sup>

- Можливості побудови графіків були розширені. Тепер ви можете створювати більш широкий спектр діаграм, включаючи *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* графіки, *Box & Whisker* діаграми, *Waterfalls* і *Funnels*. Це дозволяє візуалізувати ваші дані більш різноманітним та інформативним способом.
- Покращено управління кольором для форматування тіней. Ви можете отримати більш точний контроль над зовнішнім виглядом ваших документів, отримавши доступ до кольорів тіней.
- Покращена продуктивність при рендерингу фону. Ви можете значно прискорити рендеринг фону, що містить невеликі елементи, завдяки вбудованій технології тайлінгу.
- Додані реалістичні градієнти для фігур. Тепер ви можете створювати фігури DML з нелінійними градієнтами, імітуючи візуальний стиль Microsoft Word для надання їм більш досконалого вигляду.

#### Налаштування міток даних діаграми <sup>24.7</sup>

Додано Можливість налаштування міток даних діаграми, таких як **Orientation** та **Rotation**.

#### Користувальницький стиль нумерації для рівнів списку <sup>24.7</sup>

Додано параметр налаштування для властивості public [CustomNumberStyleFormat](https://reference.aspose.com/words/java/com.aspose.words/listlevel/#getCustomNumberStyleFormat). Тепер ви можете задати користувальницький стиль нумерації для рівнів списку.

#### Зміни в роботі з ActiveX <sup>24.7</sup>

* Властивості об'єктів ActiveX тепер можна змінювати, що дає вам більше контролю над їх поведінкою.
* Додана можливість змінювати значення перемикача ActiveX для включення динамічної взаємодії.
* Додана можливість перемикати значення ActiveX checkbox на "перевірено" або "знято".

#### Управління орієнтацією і поворотом міток на осі графіка <sup>24.8</sup>

Для більш зручного налаштування графіка був доданий точний контроль над орієнтацією і поворотом міток відміток на осі графіка – клас [AxisTickLabels](https://reference.aspose.com/words/java/com.aspose.words/axisticklabels/) був розширений новими властивостями **Orientation** і **Rotation**.

#### Заміна зворотної косої риси знаком ієни <sup>24.8</sup>

Покращено експорт із зворотною сумісністю HTML і XAML для заміни символу зворотної косої риски знаком ієни. Для досягнення цієї мети до класів [HtmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/) та [XamlFlowSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/) було додано властивість **ReplaceBackslashWithYenSign**.

#### Використання тегів SDT Як імен полів форми при експорті в PDF <sup>24.8</sup>

PDF експорт із підтримкою Використання тегів SDT Як імен полів форми було розширено додаванням нової властивості **UseSdtTagAsFormFieldName** до класу [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/).

### Перетворення, завантаження та збереження документів

#### Експорт посилань у формат Markdown <sup>24.7</sup>

Можливість керувати експортом посилань у форматі Markdown була додана завдяки реалізації властивості [LinkExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getLinkExportMode).

#### LowCode 24.8 <sup>24.8</sup>

Був представлений новий клас **LowCode.Converter**, призначений для надання набору методів перетворення різних типів документів за допомогою одного рядка коду.

### Пошук та порівняння

#### Розширені параметри порівняння <sup>24.6</sup>

Додана можливість оптимізації робочих процесів аналізу даних з поліпшеною функціональністю порівняння. Це включає нову опцію [IgnoreStoreItemId](https://reference.aspose.com/words/java/com.aspose.words/advancedcompareoptions/#getIgnoreStoreItemId) та перероблений інтерфейс для розширених порівнянь.

### Інший

* Функція видалення порожніх сторінок з документа була реалізована шляхом додавання методу [RemoveBlankPages](https://reference.aspose.com/words/java/com.aspose.words/document/#removeBlankPages). <sup>24.5</sup>
* Можливість перевірки наявності макросів VBA без завантаження документа була надана шляхом додавання властивості [HasMacros](https://reference.aspose.com/words/java/com.aspose.words/fileformatinfo/#hasMacros). <sup>24.5</sup>
* Тепер підтримується збереження нумерації джерел при вставці документа за допомогою механізму створення звітів LINQ. <sup>24.5</sup>
* Додано нову властивість [DateTimeUtc](https://reference.aspose.com/words/java/com.aspose.words/comment/#getDateTimeUtc) – вона забезпечує більш точну позначку часу для коментарів, покращуючи організацію та відстеження. <sup>24.6</sup>
* Покращено механізм створення звітів LINQ. Вибірково видалені порожні абзаци та визначені користувацькі повідомлення для відсутніх елементів об'єкта, що призвело до створення більш чистих та інформативних звітів. <sup>24.6</sup>
* Формат дати та часу тепер автоматично визначається для безперешкодного експорту у формат XLSX. <sup>24.7</sup>
* Додано загальнодоступну властивість [IsProtected](https://reference.aspose.com/words/java/com.aspose.words/vbaproject/#isProtected), яка дозволяє перевірити, чи захищений проект VBA. <sup>24.7</sup>
* Інформація про Шрифт була розширена шляхом додавання властивості **EmbeddingLicensingRights** до класів [FontInfo](https://reference.aspose.com/words/java/com.aspose.words/fontinfo/) та [PhysicalFontInfo](https://reference.aspose.com/words/java/com.aspose.words/physicalfontinfo/). <sup>24.8</sup>
* Для більш точної роботи зі структурою документа був доданий спосіб ефективного очищення верхніх і нижніх колонтитулів розділів зі збереженням водяних знаків. Щоб очистити верхні та нижні колонтитули розділів, використовуйте новий загальнодоступний метод **ClearHeadersFooters**. <sup>24.8</sup>
* Включено цифровий підпис XPS документів з використанням [XpsSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xpssaveoptions/) – для цієї мети додано нову властивість **DigitalSignatureDetails**. <sup>24.8</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Java 24.5 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-5-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 24.6 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-6-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 24.7 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-7-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 24.8 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words для Java 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 покращено можливості керування кольорами обведення, покращено OLE об'єкти та LINQ звіти, а також представлено нову бібліографію загальнодоступних джерел API.

Aspose.Words 24.2 розширені діаграми API, управління стилем і LINQ опції. У цій версії Aspose.Words також з'явилася можливість вказувати SvgSaveOptions під час рендеринга, більш гнучке управління завантаженням Markdown файлів і робота з посилальним текстом для виносок і кінцевих приміток.

Aspose.Words 24.3 представлений новий TIFF Режим читання/запису та емуляція бінарних растрових операцій для WMF метафайлів. Aspose.Words 24.3 також продовжує розширювати діаграми API.

Aspose.Words 24.4 розширені формати збереження, деякі параметри рендеринга, а також поліпшена робота з цифровими підписами.

### Підтримувані формати <sup>24.4</sup>

Сучасний формат зображень **WebP** тепер підтримується у форматі Aspose.Words. Тепер ви можете читати та вставляти зображення WebP у документи, а також зберігати зображення у форматі WebP.

### Рендеринг та друк

#### Управління кольором обведення <sup>24.1</sup>

Клас [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) був розширений набором нових загальнодоступних властивостей, пов'язаних з Керуванням кольорами обведення: [ForeThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeThemeColor) і [BackThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackThemeColor), [ForeTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeTintAndShade) і [BackTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackTintAndShade).

#### DrawingML розширення графіків API <sup>24.2 / 24.3 / 24.4</sup>

Параметр **DrawingML Charts API** продовжує розширюватися.

#### Вставити шрифти, оголошені в правилах @font-face <sup>24.4</sup>

Додана можливість вбудовувати шрифти, оголошені в правилах @font-face, в визначення шрифтів результуючого документа шляхом додавання нового властивості [SupportFontFaceRules](https://reference.aspose.com/words/java/com.aspose.words/htmlloadoptions/#getSupportFontFaceRules).

#### Робота з форматуванням світіння і відображення <sup>24.4</sup>

Реалізована можливість роботи з форматуванням світіння і відображення для об'єкта малювання.

### Завантаження та збереження документів

#### Вкажіть SvgSaveOptions під час рендеринга <sup>24.2</sup>

Додана можливість вказувати [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/) під час рендеринга з використанням методів [ShapeRenderer](https://reference.aspose.com/words/java/com.aspose.words/shaperenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) і [OfficeMathRenderer](https://reference.aspose.com/words/java/com.aspose.words/officemathrenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions).

#### Зберігати порожні рядки при завантаженні Markdown файлів <sup>24.2</sup>

Додана можливість зберігати порожні рядки при завантаженні файлів Markdown.

#### Новий користувач TIFF для читання / запису <sup>24.3</sup>

Розроблено новий TIFF модуль читання / запису для Aspose.Words .NET Standard, .NET 6 і пізніших версій. Aspose.Words для .NET 24.3 додана підтримка читання TIFF зображень з JPEG і старими типами стиснення JPEG, а також значно покращено якість операцій читання і запису.

### Інший

* Можливість змінювати текст елемента керування `TextBox` OLE була реалізована шляхом додавання нової властивості [Text](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/#getText) до нового класу [TextBoxControl](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/). 24.1 <sup>24.1</sup>
* Загальнодоступні джерела бібліографії API були реалізовані шляхом додавання декількох нових класів [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/bibliography/), [Source](https://reference.aspose.com/words/java/com.aspose.words/source/), [ContributorCollection](https://reference.aspose.com/words/java/com.aspose.words/contributorcollection/), [Contributor](https://reference.aspose.com/words/java/com.aspose.words/contributor/), [Corporate](https://reference.aspose.com/words/java/com.aspose.words/corporate/), [PersonCollection](https://reference.aspose.com/words/java/com.aspose.words/personcollection/) і [Person](https://reference.aspose.com/words/java/com.aspose.words/person/) і перерахування [SourceType](https://reference.aspose.com/words/java/com.aspose.words/sourcetype/), а також шляхом додавання нової властивості [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/document/#getBibliography) до класу [Document](https://reference.aspose.com/words/java/com.aspose.words/document/). <sup>24.1</sup>
* Було передбачено API обмеження доступу до елементів типу за допомогою синтаксису шаблону для механізму звітування LINQ. <sup>24.1</sup>
* Клас [Style](https://reference.aspose.com/words/net/aspose.words/style/) додав нові загальнодоступні властивості [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) та [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) для вдосконаленого управління стилем. <sup>24.2</sup>
* Функціональність для отримання фактичного тексту опорного знака для виносок і кінцевих виносок була розширена за допомогою властивості [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) і методу [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* Включена сумісність з графіками `Word 2016` для `LINQ Reporting Engine`. <sup>24.2</sup>
* Реалізована емуляція бінарних растрових операцій для метафайлів WMF. <sup>24.3</sup>
* Можливість визначення параметрів підпису для документів у **SaveOptions** була включена шляхом додавання нового класу [DigitalSignatureDetails](https://reference.aspose.com/words/java/com.aspose.words/digitalsignaturedetails/) з новими відкритими членами, а також додавання нових властивостей до класів [OoxmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/docsaveoptions/) та [OdtSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Java 24.1 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-1-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 24.2 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-2-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 24.3 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-3-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 24.4 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words для Java 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 розширює можливості рендеринга, емуляції рендеринга метафайлів і markdown збереження.

Aspose.Words 23.10 покращено рендеринг, розширені можливості завантаження і збереження документів, а також користувачі можуть по-новому об'єднувати документи.

Aspose.Words 23.11 розширює можливості роботи зі змінами, XLSX форматуванням і шрифтами в легенді діаграми за допомогою додаткових опцій.

Aspose.Words 23.12 додані нові властивості і перерахування для роботи з PDF документами, підтримка WebP зображень і оновлена бібліотека Bouncy Castle.

### Рендеринг та друк

#### Налаштування назв осей в DrawingML діаграмах <sup>23.9</sup>

Можливість налаштовувати назви осей на діаграмах DrawingML з'явилася завдяки впровадженню нової властивості public class [ChartAxisTitle](https://reference.aspose.com/words/java/com.aspose.words/chartaxistitle/) і [Title](https://reference.aspose.com/words/java/com.aspose.words/chartaxis/#getTitle).

#### Визначення вертикального розташування шрифтів в абзаці <sup>23.9</sup>

Тепер можна визначати вертикальне розташування шрифтів в абзаці, використовуючи нову властивість public [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getBaselineAlignment) і нове перерахування [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/baselinealignment/).

#### Управління кольором переднього плану <sup>23.10</sup>

Можливість витягувати колір переднього плану без модифікаторів була додана до класів [Fill](https://reference.aspose.com/words/java/com.aspose.words/fill/) та [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) за допомогою властивості **BaseForeColor**.

#### Розширення функціональності графіків <sup>23.10</sup>

Функціональність класів [ChartDataPointCollection](https://reference.aspose.com/words/java/com.aspose.words/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/java/com.aspose.words/chartseries/) та [ChartFormat](https://reference.aspose.com/words/java/com.aspose.words/chartformat/) була розширена новими методами та властивостями.

#### Автоматична настройка і підгонка зображення під форму <sup>23.10</sup>

Новий метод [FitImageToShape](https://reference.aspose.com/words/java/com.aspose.words/imagedata/#fitImageToShape) надає простий спосіб автоматичної настройки і підгонки зображення під певну форму.

#### Форматування шрифту за замовчуванням для DrawingML записів в умовних позначеннях діаграми <sup>23.11</sup>

Додана можливість задавати форматування шрифту за замовчуванням для записів умовних позначень діаграм DrawingML за допомогою властивості **Font**. Ця функція забезпечує більш впорядкований і однаковий зовнішній вигляд елементів діаграми, покращуючи загальну естетику документа.

#### Вкажіть макет сторінки під час відкриття PDF у Reader <sup>23.12</sup>

Можливість вказувати макет сторінки, який буде використовуватися при відкритті документа в PDF рідері, була додана завдяки введенню нового властивості [PageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getPageLayout) для класу [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/) і нового перерахування [PdfPageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfpagelayout/).

### Завантаження та збереження документів

#### Вказівка імені папки для створення зображення URIs в Markdown <sup>23.9</sup>

Клас [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) було розширено додаванням властивості [ImagesFolderAlias](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImagesFolderAlias), що дозволяє вказати назву папки, яка використовується для створення зображення URIs, записаного в документ Markdown.

#### Зменшити PDF Розмір вихідних даних <sup>23.10</sup>

Були реалізовані різні оптимізації PDF рендеринга для зменшення розміру вихідних даних при використанні налаштувань [OptimizeOutput](https://reference.aspose.com/words/java/com.aspose.words/fixedpagesaveoptions/#getOptimizeOutput).

#### Розпізнавати гіперпосилання при завантаженні TXT документів <sup>23.10</sup>

Функція розпізнавання гіперпосилань при завантаженні документів TXT була реалізована шляхом додавання нової властивості [DetectHyperlinks](https://reference.aspose.com/words/java/com.aspose.words/txtloadoptions/#getDetectHyperlinks).

### Інший

- Реалізована емуляція рендеринга метафайлів для визначення розміру растеризації, зокрема, для WMF ширини пера і EMF косметичної ширини пера. Для досягнення цієї мети властивість **ScaleWmfFontsToMetafileSize** було замінено властивістю [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPage) і додано властивість [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPageResolution). <sup>23.9</sup>
- З використанням методу [InsertDocumentInline](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertDocumentInline-com.aspose.words.Document-int-com.aspose.words.ImportFormatOptions) був представлений спрощений метод вставки одного документа в інший в поточному положенні курсору. <sup>23.10</sup>
- Можливість доступу до властивостей стилю і їх зміни була додана завдяки введенню нового властивості [Locked](https://reference.aspose.com/words/java/com.aspose.words/style/#getLocked). <sup>23.10</sup>
- До методів класу [CompositeNode](https://reference.aspose.com/words/java/com.aspose.words/compositenode/) був доданий параметр універсального типу. <sup>23.10</sup>
- За допомогою методів [Accept](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#accept-com.aspose.words.IRevisionCriteria) і [Reject](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#reject-com.aspose.words.IRevisionCriteria) був реалізований спосіб контролю того, коли певна редакція повинна бути прийнята/відхилена чи ні. Це вдосконалення надає користувачам більш точний контроль над процесом внесення змін. <sup>23.11</sup>
- Можливість записувати всі розділи документа на один і той же робочий лист XLSX була надана завдяки новому типу перерахування [XlsxSectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsectionmode/) і Новій властивості [SectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/#getSectionMode). <sup>23.11</sup>
- Додана підтримка зображень WebP. Будь ласка, зверніть увагу, що ця функція доступна тільки для версій .NetStandart і .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Java 23.9 Примітки до випуску](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-9-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 23.10 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-10-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 23.11 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-11-release-notes/).

Дізнайтеся більше про [Aspose.Words для Java 23.12 примітки до випуску](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-12-release-notes/).

{{% /alert %}}

## Дивіться також

{{% alert color="primary" %}}

На цій сторінці представлені останні новини про релізи за останні 2 роки. Більш детальну інформацію про попередні випуски дивіться в [Примітки до випуску'](https://releases.aspose.com/words/java/release-notes/) сторінки у відповідних розділах.

{{% /alert %}}
