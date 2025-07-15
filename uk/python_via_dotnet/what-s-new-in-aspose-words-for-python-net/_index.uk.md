---
title: Що нового
second_title: Aspose.Words для Python via .NET
articleTitle: Що нового в Aspose.Words для Python via .NET
linktitle: Що нового в Aspose.Words для Python via .NET
type: docs
description: "Aspose.Words для Python via .NET з кожним днем асортимент розширюється. На цій сторінці ви можете дізнатися про найважливіші та найцікавіші можливості продукту."
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /uk/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-06-23-21-02-49
---

На цій сторінці описані найцікавіші нові функції Aspose.Words, що з'явилися в останніх версіях.

## Aspose.Words для Python via .NET 25.5, 25.6

Aspose.Words 25.5 розширює можливості налаштування діаграм за допомогою нових варіантів оформлення і покращує Markdown експорт, надаючи можливість управляти обробкою порожніх абзаців.

Aspose.Words 25.6 покращує точність візуалізації та можливості візуалізації завдяки розширеним можливостям експорту зображень, покращеній обробці MathML та кращому представленню діаграм.

### Перетворення, завантаження та збереження документів

#### Експортуйте порожні абзаци в Markdown <sup>25.5</sup>

Можливість керувати тим, як порожні абзаци експортуються в Markdown, з'явилася завдяки додаванню перерахування **MarkdownEmptyParagraphExportMode** і властивості **empty_paragraph_export_mode**.

#### Експорт багатосторінкових документів у формати растрових зображень <sup>25.6</sup>

Можливість експорту багатосторінкових документів у формати растрових зображень (наприклад, PNG і JPEG) з [customizable layouts](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) - по горизонталі, вертикалі або сітці – з'явилася завдяки розширенню функціональності експорту зображень.

### Візуалізація

#### Налаштування стилю діаграми <sup>25.5</sup>

Можливість задавати стиль діаграми була реалізована шляхом додавання перерахування **ChartStyle** і властивості **style**.

#### Відображення сполучних ліній у виразах MathML <sup>25.6</sup>

Для забезпечення більш точного і візуально несуперечливого відображення математичних формул був реалізований рендеринг сполучних ліній у виразах MathML.

#### Візуалізація умовних позначень для каскадних діаграм <sup>25.6</sup>

Була введена візуалізація умовних позначень для ["Waterfall" charts](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriestype/), що підвищує прозорість даних і покращує інтерпретованість цих діаграм.

### Інший

* Покращено можливість перенесення математичних формул, що містять кілька косих рис, що підвищує чіткість компонування і розбірливість формул. <sup>25.6</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Python via .NET приміток до випуску 25.5](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-5-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET приміток до випуску 25.6](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words для Python через .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 реалізована перевірка граматики на основі AI та покращено збереження документів завдяки розширеним параметрам для форматів HTML, SVG та Markdown.

Aspose.Words 25.2 введено Узагальнення тексту за допомогою Anthropic AI моделей, додана підтримка MsWorks форматів, поліпшений контроль типографіки і поліпшена структура PDF і обробка списків.

Aspose.Words 25.3 розширює можливості перевірки граматики на основі AI та вибору шрифту за допомогою властивості UpdateAmbiguousTextFont, а також покращує експорт вкладень на основі PDF.

Aspose.Words 25.4 додана підтримка нових форматів паперу, розширено контроль експорту HTML і поліпшена обробка водяних знаків.

### AI - функціональні можливості

#### Перевірка граматики документа AI

* Можливість перевірки граматики наданого документа з використанням OpenAI генеруючих моделей була реалізована шляхом додавання нового методу [check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/). <sup>25.1</sup>
* Функція перевірки граматики на основі AI була оновлена для підтримки всіх моделей, доступних у списку [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Узагальнення з використанням Anthropic генеруючих мовних моделей <sup>25.2</sup>

Узагальнення тексту за допомогою моделей генеративної мови Anthropic стало можливим завдяки введенню нового загальнодоступного класу [AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/).

### Підтримувані формати <sup>25.2</sup>

Починаючи з версії 25.2, Додана сумісність з новим форматом завантаження MsWorks для робочих документів Microsoft.

### Перетворення, завантаження та збереження документів

#### Покращено збереження у форматах HTML та SVG <sup>25.1</sup>

Збереження у форматах HTML та SVG було покращено додаванням властивостей **id_prefix** та **remove_java_script_from_links** Як до класів [HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/), так і [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/).

#### Встановіть роздільну здатність зображення та режим виводу OfficeMath при збереженні в Markdown <sup>25.1</sup>

* До класу [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) додано нову опцію [image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/) для налаштування роздільної здатності зображення.
* У клас [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) були додані нова опція [office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/) і перерахування [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/), щоб задати режим виведення OfficeMath.

### Візуалізація

#### Покращений типографський контроль <sup>25.2</sup>

Властивість [number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/) було додано для покращення управління типографікою.

#### Управління вибором шрифту для неоднозначних символів <sup>25.3</sup>

До класу [SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/) додано нову загальнодоступну властивість [update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/), що дозволяє керувати вибором шрифту відповідно до використовуваного коду символу.

#### Параметри формату паперу <sup>25.4</sup>

Можливість використання форматів паперу JIS B4 та JIS B5 була реалізована шляхом додавання нових значень до списку [PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/).

#### HTML управління виходом <sup>25.4</sup>

Можливість видалення JavaScript з гіперпосилання URLs під час експорту HTML була реалізована шляхом додавання властивості [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/).

### Інший

* PDF логічна структура була вдосконалена завдяки підтримці полів TOA, BIBLIOGRAPHY та INDEX. <sup>25.2</sup>
* Метод [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate) був введений для поліпшення роботи зі списками. <sup>25.2</sup>
* Додано нову властивість [attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/) замість **EmbedAttachments** для покращення експорту вкладень PDF. Крім того, до Списку [PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/) були додані нові значення для підтримки вкладень версії PDF/A. Крім того, вкладення тепер підтримуються за допомогою шифрування. <sup>25.3</sup>
* Можливість встановлення водяного знака на зображення з потоку була введена шляхом додавання нового перевантаження до методу [SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions). <sup>25.4</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Python via .NET 25.1 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 25.2 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 25.3 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 25.4 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words для Python через .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 додає вставку group shape і вставку StructuredDocumentTag за допомогою DocumentBuilder, покращує відображення радіальних діаграм за допомогою градуювань, покращує цифрові підписи з підтримкою XAdES-EPES, додає розпізнавання підкреслення Markdown і надає доступ до роздільників виносок/кінцевих приміток.

Aspose.Words 24.10 представлена розширена підтримка елементів керування ActiveX зі створенням CommandButton, новий елемент керування видимістю фігур, можливість group shapes, покращений експорт Markdown для таблиць, форматування діаграм для Pie та Doughnut діаграм, Покращена обробка кодувань Big5 та Підтримка застарілих Тайванські шрифти.

Aspose.Words 24.11 реалізована функція Узагальнення документів на основі AI, розширені можливості візуалізації, покращений доступ до властивостей документа і ActiveX Управління субтитрами.

Aspose.Words 24.12 представлені настроюється розміщення міток даних, переклад тексту за допомогою Google AI і поліпшені нові класи обробки LowCode.

### AI - функціональні можливості

#### Узагальнення документів за допомогою OpenAI та Google <sup>24.11</sup>

Підтримка Узагальнення документів за допомогою моделей генеративної мови **OpenAI** та **Google** була інтегрована шляхом додавання простору імен [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) з його загальнодоступними членами.

#### Переклад тексту за допомогою генеративних мовних моделей Google <sup>24.12</sup>

Можливість перекладу тексту за допомогою моделей генеративної мови Google була реалізована в Aspose.Words шляхом додавання методу [translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/) та перерахування [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) у простір імен [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Були введені нові класи LowCode, такі як [Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) і т.д., які пропонують набір методів, що забезпечують ідеальний баланс між простотою і гнучкістю обробки документів.

### Рендеринг та друк

#### Градуювання на радіальних графіках <sup>24.9</sup>

Реалізовано рендеринг градуювань на радіальних графіках.

#### CommandButton ActiveX елементи керування <sup>24.10</sup>

Можливість створення CommandButton ActiveX елементів керування була реалізована шляхом додавання нового загальнодоступного методу [insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/) та нового загальнодоступного класу [Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/).

#### Контролюйте видимість фігури <sup>24.10</sup>

Додано нову загальнодоступну властивість [hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/) для контролю видимості фігур.

#### Зміни на графіках Pie і Doughnut <sup>24.10</sup>

До діаграм формату Pie та Doughnut було додано кілька нових загальнодоступних властивостей.

#### Керувати відображенням меж поля форми вибору PDF <sup>24.11</sup>

Нова опція для управління відображенням меж полів форми вибору PDF була реалізована шляхом додавання нової загальнодоступної опції [render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/).

#### Отримання та встановлення кодів формату для даних діаграми <sup>24.11</sup>

Можливість отримання та встановлення кодів формату для даних діаграми була додана шляхом реалізації властивості [format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/) у класах [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/) та [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/).

#### Візуалізація гістограмних графіків з осередками і написами <sup>24.11</sup>

Покращено рендеринг гістограмних діаграм за рахунок використання заданої кількості осередків і міток.

#### Налаштування розміщення міток даних <sup>24.12</sup>

Додана можливість налаштування розміщення міток даних шляхом додавання нових властивостей до класів [ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/) і [ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Перетворення, завантаження та збереження документів

#### Підкреслення форматування при завантаженні Markdown файлів <sup>24.9</sup>

Можливість розпізнавати форматування підкреслення під час завантаження документів Markdown була реалізована шляхом додавання нової загальнодоступної властивості [import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/).

#### Експорт таблиць як HTML при збереженні в Markdown <sup>24.10</sup>

Можливість експортувати таблиці у форматі HTML при збереженні документів у форматі Markdown була реалізована шляхом додавання нової загальнодоступної властивості [export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/) та перерахування [MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/).

#### Експорт PDF з оновленою логічною структурою <sup>24.11</sup>

PDF експорт було покращено, включивши властивості заголовка таблиці як заголовки елементів логічної структури PDF.

### Цифрові підписи

#### Підписуйте документи за допомогою XAdES-EPES <sup>24.9</sup>

Можливість підписувати документи підписами рівня XAdES-EPES XML-DSig була введена шляхом додавання нової публічної властивості [xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/) та нового публічного переліку [XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/).

### Інший

* До group shapes було додано новий загальнодоступний метод [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/). <sup>24.9</sup>
* Додано новий загальнодоступний метод [insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/) для вставки **StructuredDocumentTags** у документ. <sup>24.9</sup>
* Відкритий доступ до розділювачів виносок і кінцевих приміток був забезпечений шляхом додавання декількох загальнодоступних класів і властивостей. <sup>24.9</sup>
* Можливість групувати окремі фігури, group shapes разом, а також безпосередньо групувати обидві фігури і group shapes з'явилася завдяки додаванню методу [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist). <sup>24.10</sup>
* Покращена обробка кодування Big5 для TrueType таблиць cmap. <sup>24.10</sup>
* Була покращена підтримка застарілих тайванських шрифтів. <sup>24.10</sup>
* Для доступу до розширених властивостей документа в клас [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/) були додані властивості, доступні тільки для читання. <sup>24.11</sup>
* Налаштування підписів для елементів керування ActiveX було ввімкнено шляхом додавання нового загальнодоступного параметра Налаштування до властивості [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.9 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.10 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.11 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.12 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words для Python через .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 розширює можливості для збірок, покращує можливості рендеринга і розширює деякі інші можливості.

Aspose.Words 24.6 покращено параметри рендеринга, розширені можливості пошуку та порівняння, а також розширено ряд інших функцій.

Aspose.Words 24.7 змінює спосіб роботи з ActiveX, розширює можливості рендеринга, а також експорту в формати Markdown і XLSX.

Aspose.Words 24.8 розширює можливості налаштування діаграм за рахунок точного управління мітками осей, розширює можливості управління шрифтами, покращує роботу зі структурою документа і додає нові можливості для експорту HTML/XAML, функціональності PDF, перетворення документів і цифрових підписів.

### Підтримувані формати

Починаючи з версії 24.7, підтримується експорт в PDF/UA-2 для забезпечення доступності для користувачів з обмеженими можливостями.

### Рендеринг та друк

#### Зміни в графіках, фігурах і DrawingML <sup>24.5</sup>

* DrawingML реалізовано рендеринг ефектів для SVG графіки, що розширює попередню функціональність, обмежену зображеннями.
* Підтримка створення комбінованих діаграм та налаштування таких властивостей, як ширина проміжку, перекриття та бульбашковий масштаб у групах рядів була реалізована шляхом додавання класів [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/) та [ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/) та властивості [series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/).
* Функціональність для управління ефектом SoftEdge фігур була реалізована шляхом додавання класу [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/).
* Можливість змінювати коригувальні значення фігур була реалізована шляхом додавання загальнодоступних класів **AdjustmentCollection** і **Adjustment** і властивості [adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/).

#### Зміни в діаграмах, фігурах і кресленнях <sup>24.6</sup>

- Можливості побудови графіків були розширені. Тепер ви можете створювати більш широкий спектр діаграм, включаючи *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* графіки, *Box & Whisker* діаграми, *Waterfalls* і *Funnels*. Це дозволяє візуалізувати ваші дані більш різноманітним та інформативним способом.
- Покращено управління кольором для форматування тіней. Ви можете отримати більш точний контроль над зовнішнім виглядом ваших документів, отримавши доступ до кольорів тіней.
- Покращена продуктивність при рендерингу фону. Ви можете значно прискорити рендеринг фону, що містить невеликі елементи, завдяки вбудованій технології тайлінгу.
- Додані реалістичні градієнти для фігур. Тепер ви можете створювати фігури DML з нелінійними градієнтами, імітуючи візуальний стиль Microsoft Word для надання їм більш досконалого вигляду.

#### Налаштування міток даних діаграми <sup>24.7</sup>

Додано Можливість налаштування міток даних діаграми, таких як **Orientation** та **Rotation**.

#### Користувальницький стиль нумерації для рівнів списку <sup>24.7</sup>

Додано параметр налаштування для властивості public [custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/). Тепер ви можете задати користувальницький стиль нумерації для рівнів списку.

#### Зміни в роботі з ActiveX <sup>24.7</sup>

- Властивості об'єктів ActiveX тепер можна змінювати, що дає вам більше контролю над їх поведінкою.
- Додана можливість змінювати значення перемикача ActiveX для включення динамічної взаємодії.
- Додана можливість перемикати значення ActiveX checkbox на "перевірено" або "знято".

#### Управління орієнтацією і поворотом міток на осі графіка <sup>24.8</sup>

Для більш зручного налаштування графіка був доданий точний контроль над орієнтацією і поворотом міток відміток на осі графіка – клас [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) був розширений новими властивостями [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) і [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/).

#### Заміна зворотної косої риси знаком ієни <sup>24.8</sup>

Покращено експорт із зворотною сумісністю HTML і XAML для заміни символу зворотної косої риски знаком ієни. Для досягнення цієї мети до класів [HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/) та [XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/) було додано властивість **replace_backslash_with_yen_sign**.

#### Використання тегів SDT Як імен полів форми при експорті в PDF <sup>24.8</sup>

PDF експорт із підтримкою Використання тегів SDT Як імен полів форми було розширено додаванням нової властивості [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) до класу [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/).

### Перетворення, завантаження та збереження документів

#### Експорт посилань у формат Markdown <sup>24.7</sup>

Можливість керувати експортом посилань у форматі Markdown була додана завдяки реалізації властивості [link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/).

#### LowCode 24.8 <sup>24.8</sup>

Був представлений новий клас [LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/), призначений для надання набору методів перетворення різних типів документів за допомогою одного рядка коду.

### Пошук та порівняння

#### Розширені параметри порівняння <sup>24.6</sup>

Додана можливість оптимізації робочих процесів аналізу даних з поліпшеною функціональністю порівняння. Це включає нову опцію [ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/) та перероблений інтерфейс для розширених порівнянь.

### Інший

* Функція видалення порожніх сторінок з документа була реалізована шляхом додавання методу [remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/). <sup>24.5</sup>
* Можливість перевірки наявності макросів VBA без завантаження документа була надана шляхом додавання властивості [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/). <sup>24.5</sup>
* Тепер підтримується збереження нумерації джерел при вставці документа за допомогою механізму створення звітів LINQ. <sup>24.5</sup>
* Додано нову властивість [date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/) – вона забезпечує більш точну позначку часу для коментарів, покращуючи організацію та відстеження. <sup>24.6</sup>
* Формат дати та часу тепер автоматично визначається для безперешкодного експорту у формат XLSX. <sup>24.7</sup>
* Додано загальнодоступну властивість [is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/), яка дозволяє перевірити, чи захищений проект VBA. <sup>24.7</sup>
* Інформація про Шрифт була розширена шляхом додавання властивості **embedding_licensing_rights** до класів [FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/) та [PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* Для більш точної роботи зі структурою документа був доданий спосіб ефективного очищення верхніх і нижніх колонтитулів розділів зі збереженням водяних знаків. Щоб очистити верхні та нижні колонтитули розділів, використовуйте новий загальнодоступний метод [clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default). <sup>24.8</sup>
* Включено цифровий підпис XPS документів з використанням [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/) – для цієї мети додано нову властивість [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/). <sup>24.8</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.5 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.6 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.7 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.8 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words для Python через .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 покращено можливості керування кольорами обведення, покращено OLE об'єкти, а також введено новий `Bibliography Sources` загальнодоступний API.

Aspose.Words 24.2 розширені діаграми API і управління стилем. У цій версії Aspose.Words також з'явилася можливість вказувати SvgSaveOptions під час рендеринга, більш гнучке управління завантаженням Markdown файлів і робота з посилальним текстом для виносок і кінцевих приміток.

Aspose.Words 24.3 представлений новий TIFF Режим читання/запису та емуляція бінарних растрових операцій для WMF метафайлів. Aspose.Words 24.3 також продовжує розширювати діаграми API.

Aspose.Words 24.4 розширені формати збереження, деякі параметри рендеринга, а також поліпшена робота з цифровими підписами.

### Підтримувані формати <sup>24.4</sup>

Сучасний формат зображення **WebP** тепер підтримується в Aspose.Words для .NET Framework 4.6.2 і вище. Тепер ви можете читати та вставляти WebP зображення в документи, а також зберігати зображення у форматі WebP.

Зверніть увагу, що WebP наразі доступний лише у версіях .NET Standard та .NET Framework v4.6.2 та вище.

### Рендеринг та друк

#### Управління кольором обведення <sup>24.1</sup>

Клас [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) був розширений набором нових загальнодоступних властивостей, пов'язаних з Керуванням кольорами обведення: [fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/) і [back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/), [fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/) і [back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### DrawingML розширення графіків API <sup>24.2 / 24.3 / 24.4</sup>

Параметр **DrawingML Charts API** продовжує розширюватися.

#### Вставити шрифти, оголошені в правилах @font-face <sup>24.4</sup>

Додана можливість вбудовувати шрифти, оголошені в правилах @font-face, в визначення шрифтів результуючого документа була введена шляхом додавання нової властивості [support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/).

#### Робота з форматуванням світіння і відображення <sup>24.4</sup>

Реалізована можливість роботи з форматуванням світіння і відображення для об'єкта малювання.

### Завантаження та збереження документів

#### Вкажіть SvgSaveOptions під час рендеринга <sup>24.2</sup>

Додана можливість вказувати [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) під час рендеринга з використанням методів [ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) і [OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions).

#### Зберігати порожні рядки при завантаженні Markdown файлів <sup>24.2</sup>

Додана можливість зберігати порожні рядки при завантаженні файлів Markdown.

#### Новий користувач TIFF для читання / запису <sup>24.3</sup>

Розроблено новий режим читання / запису TIFF для Aspose.Words. Aspose.Words для .NET 24.3 додана підтримка читання TIFF зображень з JPEG і старими типами стиснення JPEG, а також значно покращено якість операцій читання і запису.

### Інший

* Можливість змінювати текст елемента керування `TextBox` OLE була реалізована шляхом додавання нової властивості **Text** до нового класу **TextBoxControl**. <sup>24.1</sup>
* Загальнодоступні джерела бібліографії API були реалізовані шляхом додавання нового простору імен [Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/) з його новими класами та перерахуваннями, а також шляхом додавання нової властивості [bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/) до класу [Document](https://reference.aspose.com/words/python-net/aspose.words/document/). <sup>24.1</sup>
* Клас [Style](https://reference.aspose.com/words/python-net/aspose.words/style/) додав нові загальнодоступні властивості [priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/), [unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/) та [semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/) для вдосконаленого управління стилем. <sup>24.2</sup>
* Функціональність для отримання фактичного тексту опорного знака для виносок і кінцевих виносок була розширена за допомогою властивості [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/) і методу [update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default). <sup>24.2</sup>
* Реалізована емуляція бінарних растрових операцій для метафайлів WMF. <sup>24.3</sup>
* Можливість визначення параметрів підпису для документів у **SaveOptions** була включена шляхом додавання нового класу [DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/) з новими відкритими членами, а також додавання нових властивостей до класів [OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/) та [OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.1 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.2 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.3 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 24.4 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words для Python через .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 розширює можливості рендеринга, емуляції рендеринга метафайлів і markdown збереження.

Aspose.Words 23.10 покращено рендеринг, розширені можливості завантаження і збереження документів, а також користувачі можуть по-новому об'єднувати документи.

Aspose.Words 23.11 розширює можливості роботи зі змінами, XLSX форматуванням і шрифтами в легенді діаграми за допомогою додаткових опцій.

Aspose.Words 23.12 додані нові властивості і перерахування для роботи з PDF і OOXML документами, а також підтримка WebP зображень.

### Рендеринг та друк

#### Налаштування назв осей в DrawingML діаграмах <sup>23.9</sup>

Можливість налаштовувати назви осей на діаграмах DrawingML з'явилася завдяки впровадженню нової властивості public class [ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/) і [title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/).

####  Визначення вертикального розташування шрифтів в абзаці <sup>23.9</sup>

Тепер можна визначати вертикальне розташування шрифтів в абзаці, використовуючи нову властивість public [baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/) і нове перерахування [BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/).

#### Управління кольором переднього плану <sup>23.10</sup>

Можливість витягувати колір переднього плану без модифікаторів була додана до класів [Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/) та [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) за допомогою властивості **BaseForeColor**.

#### Розширення функціональності графіків <sup>23.10</sup>

Функціональність класів [ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/) та [ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/) була розширена новими методами та властивостями.

#### Автоматична настройка і підгонка зображення під форму <sup>23.10</sup>

Новий метод [fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default) надає простий спосіб автоматичної настройки і підгонки зображення під певну форму.

#### Форматування шрифту за замовчуванням для DrawingML записів в умовних позначеннях діаграми <sup>23.11</sup>

Додана можливість задавати форматування шрифту за замовчуванням для записів умовних позначень діаграм DrawingML за допомогою властивості [font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/). Ця функція забезпечує більш впорядкований і однаковий зовнішній вигляд елементів діаграми, покращуючи загальну естетику документа.

#### Вкажіть макет сторінки під час відкриття PDF у Reader <sup>23.12</sup>

Можливість вказувати макет сторінки, який буде використовуватися при відкритті документа в PDF рідері, була додана завдяки введенню нового властивості [page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/) для класу [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) і нового перерахування [PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/).

### Завантаження та збереження документів

#### Вказівка імені папки для створення зображення URIs в Markdown <sup>23.9</sup>

Клас [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) було розширено додаванням властивості [images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/), що дозволяє вказати назву папки, яка використовується для створення зображення URIs, записаного в документ Markdown.

#### Зменшити PDF Розмір вихідних даних <sup>23.10</sup>

Були реалізовані різні оптимізації PDF рендеринга для зменшення розміру вихідних даних при використанні налаштувань [optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/).

#### Розпізнавати гіперпосилання при завантаженні TXT документів <sup>23.10</sup>

Функція розпізнавання гіперпосилань при завантаженні документів TXT була реалізована шляхом додавання нової властивості [detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/).

### Інший

- Реалізована емуляція рендеринга метафайлів для визначення розміру растеризації, зокрема, для WMF ширини пера і EMF косметичної ширини пера. Для досягнення цієї мети властивість **ScaleWmfFontsToMetafileSize** було замінено властивістю [emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/) і додано властивість [emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/). <sup>23.9</sup>
- З використанням методу [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions) був представлений спрощений метод вставки одного документа в інший в поточному положенні курсору. <sup>23.10</sup>
- Можливість доступу до властивостей стилю і їх зміни була додана завдяки введенню нового властивості [locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/). <sup>23.10</sup>
- До методів класу [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/) був доданий параметр універсального типу. <sup>23.10</sup>
- Можливість записувати всі розділи документа на один і той же робочий лист XLSX була надана завдяки новому типу перерахування [XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/) і Новій властивості [section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/). <sup>23.11</sup>
* Спосіб управління тим, як розширення формату ZIP64 будуть використовуватися для документів OOXML, був реалізований за допомогою нової властивості Zip64Mode класу `OoxmlSaveOptions` та нового переліку Zip64Mode. <sup>23.12</sup>
* Додана підтримка зображень WebP. Будь ласка, зверніть увагу, що ця функція доступна тільки для версій .NetStandart і .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Python via .NET 23.9 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 23.10 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 23.11 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

Дізнайтеся більше про [Aspose.Words для .NET 23.12 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words для Python через .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 розширює можливості роботи з даними рядів діаграм і документами ODT, а також покращує верхні і нижні колонтитули і їх текстове оформлення.

Aspose.Words 23.6 розширені можливості візуалізації, додано новий формат експорту, покращено LINQ звіти та LowCode інструменти.

Aspose.Words 23.7 розширені можливості створення звітів, доданий новий формат експорту і внесені зміни в роботу з таблицями і цифровими підписами.

Aspose.Words 23.8 розширює можливості різних форматів, покращує візуалізацію і додає нові опції для роботи з полями.

### Підтримувані формати

* Починаючи з версії 23.6, можна зберігати документи у форматі XLSX. Тепер ви можете конвертувати свої документи у формат Excel. <sup>23.6</sup>

* Починаючи з версії 23.7, можна зберігати сторінку документа або фігуру в форматі EPS. <sup>23.7</sup>

### Нові можливості формату

- Додана функціональність для автоматичного створення змісту (TOC) для MOBI документів. <sup>23.8</sup>
- Конструктор [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) було розширено до [PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions). <sup>23.8</sup>
- Реалізовано формування вертикального тексту для метафайлів EMF. <sup>23.8</sup>

### Візуалізація

#### Отримання та зміна даних ряду діаграм <sup>23.5</sup>

Можливість отримувати і змінювати дані рядів діаграм була надана шляхом додавання:

- нові класи: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- нові типи перерахувань: [ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### Підтримка розширеної типографіки <sup>23.6</sup>

Додана підтримка розширеної типографіки при рендерингу WMF, EMF і EMF+.

#### Кольоровий вміст на сторінці <sup>23.6</sup>

Додано загальнодоступну властивість [PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/), яка вказує, чи є сторінка кольоровою чи ні.

#### Форматування міток даних діаграми <sup>23.6</sup>

Реалізована можливість налаштування форматування заливки, обведення і виносок для міток даних діаграми.

### Mail Merge та звітність

#### Динамічне вставлення HTML для механізму звітності LINQ <sup>23.6</sup>

Додано новий спосіб динамічної вставки HTML для механізму звітування LINQ.

#### Mustache Підтримка тегів <sup>23.7</sup>

Mustache теги тепер підтримуються в методах [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/) та [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/).

#### Вказівка розміру відображуваних зображень <sup>23.8</sup>

Введено нову загальнодоступну властивість [image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/), щоб вказати розмір відтворюваних зображень у пікселях.

#### Зберегти пробіли для JSON рядкових значень - LINQ <sup>23.8</sup>

У механізм створення звітів LINQ додана опція для збереження пробілів для рядкових значень JSON.

### LowCode <sup>23.6</sup>

Додано нові LowCode методи, призначені для об'єднання різних типів документів в єдиний вихідний документ.

### Інший

- Реалізована підтримка перенесення тексту в верхні і нижні колонтитули. <sup>23.5</sup>
- Додана можливість видаляти цифрові підписи з ODT документів за допомогою методу [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str). <sup>23.5</sup>
- Додано загальнодоступне властивість [phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/) для отримання базового і ruby-тексту фонетичного керівництва [Run](https://reference.aspose.com/words/python-net/aspose.words/run/). <sup>23.5</sup>
- Додана можливість витягувати значення цифрового підпису з документа з цифровим підписом у вигляді масиву байт, ввівши нову властивість [signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/). <sup>23.7</sup>
- Класи [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/) і [Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/) були розширені за рахунок нових відкритих учасників– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), і [Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/). <sup>23.7</sup>

{{% alert color="primary" %}}

Дізнайтеся більше про [Aspose.Words для Python via .NET 23.5 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-5-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 23.6 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-6-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 23.7 примітки до випуску](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

Дізнайтеся більше про [Aspose.Words для Python via .NET 23.8 Примітки до випуску](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## Дивіться також

{{% alert color="primary" %}}

На цій сторінці представлені останні новини про релізи за останні 2 роки. Більш детальну інформацію про попередні випуски дивіться в [Примітки до випуску'](https://releases.aspose.com/words/python/release-notes/) сторінки у відповідних розділах.

{{% /alert %}}
