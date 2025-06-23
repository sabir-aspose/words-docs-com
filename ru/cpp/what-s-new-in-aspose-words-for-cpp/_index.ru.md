---
title: Что нового
second_title: Aspose.Words для C++
articleTitle: Что нового в Aspose.Words для C++
linktitle: Что нового в Aspose.Words для C++
type: docs
description: "Aspose.Words для C++ с каждым днем расширяется и улучшается сервис. На этой странице вы можете узнать о самых важных и интересных возможностях продукта."
weight: 2
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ru/cpp/what-s-new-in-aspose-words-for-cpp/
timestamp: 2025-06-23-19-12-25
---

На этой странице описаны наиболее интересные новые функции Aspose.Words, появившиеся в последних версиях.

## Aspose.Words для C++ 25.5

Aspose.Words 25.5 расширяет возможности настройки диаграмм с помощью новых вариантов оформления и улучшает Markdown экспорт, предоставляя возможность управлять обработкой пустых абзацев.

### Преобразование, загрузка и сохранение документов

#### Экспортируйте пустые абзацы в Markdown <sup>25.5</sup>

Возможность управлять тем, как пустые абзацы экспортируются в Markdown, появилась благодаря добавлению перечисления [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownemptyparagraphexportmode/) и свойства [EmptyParagraphExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_emptyparagraphexportmode/).

### Визуализация

#### Настройка стиля диаграммы <sup>25.5</sup>

Возможность задавать стиль диаграммы была реализована путем добавления перечисления [ChartStyle](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartstyle/) и свойства [Style](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chart/get_style/).

{{% alert color="primary" %}}

Узнайте больше о [Aspose.Words для C++ Примечаний к выпуску 25.5](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-5-release-notes/).

{{% /alert %}}

## Aspose.Words для C++ 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 реализована проверка грамматики на основе AI и улучшено сохранение документов благодаря расширенным параметрам для форматов HTML, SVG и Markdown.

Aspose.Words 25.2 введено обобщение текста с помощью Anthropic AI моделей, добавлена поддержка MsWorks форматов, улучшен контроль типографики и улучшена структура PDF и обработка списков.

Aspose.Words 25.3 расширяет возможности проверки грамматики на базе AI и выбора шрифта с помощью свойства UpdateAmbiguousTextFont, а также улучшает экспорт вложений на основе PDF.

Aspose.Words 25.4 реализована поддержка новых форматов бумаги, расширен экспортный контроль HTML, улучшена обработка водяных знаков и удобство использования LowCode API.

### AI -функциональные возможности

#### Проверка грамматики документа AI

* Возможность проверки грамматики предоставленного документа с использованием OpenAI порождающих моделей была реализована путем добавления нового метода [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/). <sup>25.1</sup>
* Функция проверки грамматики на основе AI была обновлена для поддержки всех моделей, доступных в перечислении [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Обобщение с использованием Anthropic Порождающих языковых моделей <sup>25.2</sup>

Обобщение текста с использованием моделей порождающего языка Anthropic стало возможным благодаря введению нового общедоступного класса [AnthropicAiModel](https://reference.aspose.com/words/cpp/aspose.words.ai/).

### Low Code

#### Low Code API Удобство использования <sup>25.4</sup>

Были внесены значительные улучшения в удобство использования **LowCode API**, что упростило обработку документов и уменьшило необходимость в повторяющемся коде.

### Поддерживаемые форматы <sup>25.2</sup>

Начиная с версии 25.2, добавлена совместимость с новым форматом загрузки MsWorks для рабочих документов Microsoft.

### Преобразование, загрузка и сохранение документов

#### Улучшено сохранение в форматах HTML и SVG <sup>25.1</sup>

Сохранение в форматах HTML и SVG было улучшено за счет добавления свойств **IdPrefix** и **RemoveJavaScriptFromLinks** как к классам [HtmlFixedSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlfixedsaveoptions/), так и [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/).

#### Установите разрешение изображения и режим вывода OfficeMath При сохранении в Markdown <sup>25.1</sup>

- В класс [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) добавлена новая опция [ImageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imageresolution/) для настройки разрешения изображения.
- В класс [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) были добавлены новая опция [OfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_officemathexportmode/) и перечисление [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownofficemathexportmode/), чтобы задать режим вывода OfficeMath.
- Возможность установки водяного знака на изображение из потока была введена путем добавления новой перегрузки к методу [SetImage](https://reference.aspose.com/words/cpp/aspose.words/watermark/setimage/#watermarksetimageconst-systemsharedptrsystemiostream-const-systemsharedptrasposewordsimagewatermarkoptions-method). <sup>25.4</sup>

### Визуализация

#### Улучшенный типографский контроль <sup>25.2</sup>

Свойство [NumberSpacing](https://reference.aspose.com/words/cpp/aspose.words/font/get_numberspacing/) было добавлено для улучшения управления типографикой.

#### Управление выбором шрифта для неоднозначных символов <sup>25.3</sup>

К классу [SaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/) добавлено новое общедоступное свойство [UpdateAmbiguousTextFont](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/get_updateambiguoustextfont/), позволяющее управлять выбором шрифта в соответствии с используемым кодом символа.

#### Параметры формата бумаги <sup>25.4</sup>

Возможность использования форматов бумаги JIS B4 и JIS B5 была реализована путем добавления новых значений в список [PaperSize](https://reference.aspose.com/words/cpp/aspose.words/papersize/).

#### HTML Управление выходом <sup>25.4</sup>

Возможность удалять JavaScript из гиперссылки URLs во время экспорта HTML была реализована путем добавления свойства [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlsaveoptions/get_removejavascriptfromlinks/).

### Другой

* PDF логическая структура была улучшена за счет поддержки полей TOA, BIBLIOGRAPHY и INDEX. <sup>25.2</sup>
* Метод [AddSingleLevelList](https://reference.aspose.com/words/cpp/aspose.words.lists/listcollection/addsinglelevellist/) был введен для улучшения работы со списками. <sup>25.2</sup>
* Было добавлено новое свойство [AttachmentsEmbeddingMode](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/get_attachmentsembeddingmode/) вместо **EmbedAttachments** для улучшения экспорта вложений PDF. Кроме того, в список [PdfCompliance](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfcompliance/) были добавлены новые значения для поддержки вложений версии PDF/A. Кроме того, вложения теперь поддерживаются с помощью шифрования. <sup>25.3</sup>

{{% alert color="primary" %}}

Узнайте больше о [Aspose.Words для C++ 25.1 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-1-release-notes/).

Узнайте больше о [Aspose.Words для C++ 25.2 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-2-release-notes/).

Узнайте больше о [Aspose.Words для C++ 25.3 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-3-release-notes/).

Узнайте больше о [Aspose.Words для C++ 25.4 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words для C++ 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 добавляет вставку group shape и вставку StructuredDocumentTag с помощью DocumentBuilder, улучшает отображение радиальных диаграмм с помощью градуировок, улучшает цифровые подписи с поддержкой XAdES-EPES, добавляет распознавание подчеркивания Markdown и предоставляет доступ к разделителям сносок/концевых примечаний.

Aspose.Words 24.10 представлена расширенная поддержка ActiveX элементов управления с созданием CommandButton, новый элемент управления видимостью фигур, возможность group shapes, улучшенный экспорт Markdown для таблиц, форматирование диаграмм для Pie и Doughnut диаграмм, улучшенная обработка кодировок Big5 и поддержка устаревших Тайваньские шрифты.

Aspose.Words 24.11 реализована функция обобщения документов на основе AI, расширены возможности визуализации, улучшен доступ к свойствам документа и ActiveX управление субтитрами.

Aspose.Words 24.12 представлены настраиваемое размещение меток данных, перевод текста с помощью Google AI, расширенные Mail Merge возможности очистки и новые LowCode классы обработки.

### AI -функциональные возможности

#### Обобщение документов с помощью OpenAI и Google <sup>24.11</sup>

Была интегрирована поддержка обобщения документов с использованием моделей порождающего языка **OpenAI** и **Google**.

#### Перевод текста с использованием порождающих языковых моделей Google <sup>24.12</sup>

Возможность перевода текста с использованием моделей порождающего языка Google была реализована в Aspose.Words путем добавления метода [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) и перечисления [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) в пространство имен [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Были введены новые классы LowCode, такие как [Comparer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/cpp/aspose.words.lowcode/merger/), [Replacer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/cpp/aspose.words.lowcode/splitter/) и т.д., которые предлагают набор методов, обеспечивающих идеальный баланс между простотой и гибкостью обработки документов.

### Рендеринг и печать

#### Градуировки на радиальных графиках <sup>24.9</sup>

Реализован рендеринг градаций на радиальных диаграммах.

#### CommandButton ActiveX Элементы управления <sup>24.10</sup>

Возможность создания CommandButton ActiveX элементов управления была реализована путем добавления нового общедоступного метода [InsertForms2OleControl](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertforms2olecontrol/) и нового общедоступного класса **Forms2OleControl**.

#### Контролируйте видимость фигуры <sup>24.10</sup>

Было добавлено новое общедоступное свойство [Hidden](https://reference.aspose.com/words/cpp/aspose.words.drawing/shapebase/get_hidden/) для управления видимостью фигур.

#### Изменения на графиках Pie и Doughnut <sup>24.10</sup>

В диаграммы формата Pie и Doughnut было добавлено несколько новых общедоступных свойств.

#### Управлять отображением границ поля формы выбора PDF <sup>24.11</sup>

Новая опция для управления отображением границ полей формы выбора PDF была реализована путем добавления новой общедоступной опции **RenderChoiceFormFieldBorder**.

#### Получение и установка кодов формата для данных диаграммы <sup>24.11</sup>

Возможность получать и устанавливать коды формата для данных диаграммы была добавлена путем реализации свойства **FormatCode** в классах [ChartXValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartyvaluecollection/) и [BubbleSizeCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/bubblesizecollection/).

#### Визуализация гистограммных графиков с ячейками и надписями <sup>24.11</sup>

Улучшен рендеринг гистограммных диаграмм за счет использования заданного количества ячеек и меток.

#### Настройка размещения меток данных <sup>24.12</sup>

Добавлена возможность настройки размещения меток данных путем добавления новых свойств к классам [ChartDataLabel](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabel/) и [ChartDataLabelCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabelcollection/).

### Преобразование, загрузка и сохранение документов

#### Подчеркивание форматирования при загрузке Markdown файлов <sup>24.9</sup>

Возможность распознавать форматирование с подчеркиванием при загрузке документов Markdown была реализована путем добавления нового общедоступного свойства **ImportUnderlineFormatting**.

#### Экспорт таблиц как HTML при сохранении в Markdown <sup>24.10</sup>

Возможность экспортировать таблицы в формате HTML при сохранении документов в формате Markdown была реализована путем добавления нового общедоступного свойства [ExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_exportashtml/) и перечисления [MarkdownExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownexportashtml/).

#### Экспорт PDF с обновленной логической структурой <sup>24.11</sup>

PDF экспорт был улучшен за счет включения свойств заголовка таблицы в качестве заголовков элементов логической структуры PDF.

### Mail Merge и отчетность

#### Удалять пустые таблицы в течение Mail Merge <sup>24.12</sup>

В перечисление [MailMergeCleanupOptions](https://reference.aspose.com/words/cpp/aspose.words.mailmerging/mailmergecleanupoptions/) был добавлен новый параметр **RemoveEmptyTables** для уточнения выходных данных Mail Merge.

### Цифровые подписи

#### Подписывайте документы с помощью XAdES-EPES <sup>24.9</sup>

Возможность подписывать документы подписями XAdES-EPES уровня XML-DSig была реализована путем добавления нового общедоступного свойства **XmlDsigLevel** и нового общедоступного перечисления **XmlDsigLevel**.

### Другой

* В group shapes был добавлен новый общедоступный метод [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/). <sup>24.9</sup>
* Был добавлен новый общедоступный метод [InsertStructuredDocumentTag](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertstructureddocumenttag/) для вставки **StructuredDocumentTags** в документ. <sup>24.9</sup>
* Открытый доступ к разделителям сносок и концевых примечаний был обеспечен путем добавления нескольких общедоступных классов и свойств. <sup>24.9</sup>
* Возможность группировать отдельные фигуры, group shapes вместе, а также напрямую группировать обе фигуры и group shapes появилась благодаря добавлению метода [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/). <sup>24.10</sup>
* Улучшена обработка кодировки Big5 для TrueType таблиц cmap. <sup>24.10</sup>
* Была улучшена поддержка устаревших тайваньских шрифтов. <sup>24.10</sup>
* Для доступа к расширенным свойствам документа в класс **BuiltInDocumentProperties** были добавлены свойства, доступные только для чтения. <sup>24.11</sup>
* Настройка подписей для элементов управления ActiveX была включена путем добавления нового общедоступного параметра настройки к свойству **Forms2OleControl.Caption**. <sup>24.11</sup>

{{% alert color="primary" %}}

Узнайте больше о [Aspose.Words для C++ 24.9 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-9-release-notes/).

Узнайте больше о [Aspose.Words для C++ 24.10 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-10-release-notes/).

Узнайте больше о [Aspose.Words для C++ 24.11 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-11-release-notes/).

Узнайте больше о [Aspose.Words для C++ 24.12 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words для C++ 24.5, 24.6, 24.7

Aspose.Words 24.5 расширяет возможности для сборок, улучшает возможности рендеринга и расширяет некоторые другие возможности.

Aspose.Words 24.6 улучшены параметры рендеринга, расширены возможности поиска и сравнения, а также расширен ряд других функций.

Aspose.Words 24.7 изменяет способ работы с ActiveX, расширяет возможности рендеринга, а также экспорта в форматы Markdown и XLSX.

### Поддерживаемые форматы

Начиная с версии 24.7, поддерживается экспорт в PDF/UA-2 для обеспечения доступности для пользователей с ограниченными возможностями.

### Рендеринг и печать

#### Изменения в графиках, фигурах и DrawingML <sup>24.5</sup>

- DrawingML реализован рендеринг эффектов для SVG графики, расширяющий предыдущую функциональность, ограниченную изображениями.
- Поддержка создания комбинированных диаграмм и настройки таких свойств, как ширина промежутка, перекрытие и пузырьковый масштаб, в группах рядов была реализована путем добавления классов **ChartSeriesGroup** и **ChartSeriesGroupCollection**, а также свойства **SeriesGroups**.
- Функциональность для управления эффектом SoftEdge фигур была реализована путем добавления класса **SoftEdgeFormat**.
- Возможность изменять корректирующие значения фигур была реализована путем добавления общедоступных классов **AdjustmentCollection** и **Adjustment** и свойства **Adjustments**.

#### Изменения в диаграммах, фигурах и чертежах <sup>24.6</sup>

- Возможности построения графиков были расширены. Теперь вы можете создавать более широкий спектр диаграмм, включая *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* графики, *Box & Whisker* диаграммы, *Waterfalls* и *Funnels*. Это позволяет вам визуализировать ваши данные более разнообразным и информативным образом.
- Улучшено управление цветом для форматирования теней. Вы можете получить более точный контроль над внешним видом ваших документов, получив доступ к цветам теней.
- Улучшена производительность при рендеринге фона. Вы можете значительно ускорить рендеринг фона, содержащего небольшие элементы, благодаря встроенной технологии тайлинга.
- Добавлены реалистичные градиенты для фигур. Теперь вы можете создавать фигуры DML с нелинейными градиентами, имитируя визуальный стиль Microsoft Word для придания им более совершенного вида.

#### Настройка меток данных диаграммы <sup>24.7</sup>

Была добавлена возможность настраивать метки данных диаграммы, такие как **Orientation** и **Rotation**.

#### Пользовательский стиль нумерации для уровней списка <sup>24.7</sup>

Добавлен параметр настройки для свойства public [CustomNumberStyleFormat](https://reference.aspose.com/words/cpp/aspose.words.lists/listlevel/get_customnumberstyleformat/). Теперь вы можете задать пользовательский стиль нумерации для уровней списка.

#### Изменения в работе с ActiveX <sup>24.7</sup>

- Свойства объектов ActiveX теперь можно изменять, что дает вам больше контроля над их поведением.
- Добавлена возможность изменять значение переключателя ActiveX для включения динамического взаимодействия.
- Добавлена возможность переключать значение ActiveX checkbox на "проверено" или "снято".

### Загрузка и сохранение документов

#### Экспорт ссылок в формат Markdown <sup>24.7</sup>

Возможность управлять экспортом ссылок в формате Markdown была добавлена благодаря реализации свойства [LinkExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_linkexportmode/).

### Поиск и сравнение

#### Расширенные параметры сравнения <sup>24.6</sup>

Добавлена возможность оптимизации рабочих процессов анализа данных с улучшенной функциональностью сравнения. Это включает в себя новую опцию **IgnoreStoreItemId** и переработанный интерфейс для расширенных сравнений.

### Другой

- Функция удаления пустых страниц из документа была реализована путем добавления метода [RemoveBlankPages](https://reference.aspose.com/words/cpp/aspose.words/document/removeblankpages/). <sup>24.5</sup>
- Возможность проверять наличие VBA макросов без загрузки документа была предоставлена путем добавления свойства **HasMacros**. <sup>24.5</sup>
- Добавлено новое свойство **DateTimeUtc** – оно обеспечивает более точную временную метку для комментариев, улучшая организацию и отслеживаемость. <sup>24.6</sup>
- Формат даты и времени теперь автоматически определяется для беспрепятственного экспорта в формат XLSX. <sup>24.7</sup>
- Было добавлено общедоступное свойство [IsProtected](https://reference.aspose.com/words/cpp/aspose.words.vba/vbaproject/get_isprotected/), которое позволяет вам проверить, защищен ли проект VBA. <sup>24.7</sup>

{{% alert color="primary" %}}

Узнайте больше о [Aspose.Words для C++ 24.5 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-5-release-notes/).

Узнайте больше о [Aspose.Words для C++ 24.6 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-6-release-notes/).

Узнайте больше о [Aspose.Words для C++ 24.7 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-7-release-notes/).

{{% /alert %}}

## Aspose.Words для C++ 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 улучшены возможности управления цветами обводки, расширены возможности OLE объектов, а также представлена новая библиография общедоступных источников API.

Aspose.Words 24.2 расширены диаграммы API и управление стилем. В этой версии Aspose.Words также появилась возможность указывать SvgSaveOptions во время рендеринга, более гибкое управление загрузкой Markdown файлов и работа со ссылочным текстом для сносок и концевых примечаний.

Aspose.Words 24.3 введена эмуляция бинарных растровых операций для WMF метафайлов, а также продолжается расширение графиков API.

Aspose.Words 24.4 расширены некоторые возможности рендеринга, а также улучшена работа с цифровыми подписями.

### Рендеринг и печать

#### Управление цветом обводки <sup>24.1</sup>

Класс [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) был расширен набором новых общедоступных свойств, связанных с управлением цветами обводки: [ForeThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_forethemecolor/) и [BackThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_foretintandshade/) и [BackTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backtintandshade/).

#### DrawingML Расширение графиков API <sup>24.2 / 24.3 / 24.4</sup>

Параметр **DrawingML Charts API** продолжает расширяться.

#### Вставлять шрифты, объявленные в правилах @font-face <sup>24.4</sup>

Добавлена возможность встраивать шрифты, объявленные в правилах @font-face, в определения шрифтов результирующего документа была введена путем добавления нового свойства [SupportFontFaceRules](https://reference.aspose.com/words/cpp/aspose.words.loading/htmlloadoptions/get_supportfontfacerules/).

#### Работа с форматированием свечения и отражения <sup>24.4</sup>

Реализована возможность работы с форматированием свечения и отражения для объекта рисования.

### Загрузка и сохранение документов

#### Укажите SvgSaveOptions Во время рендеринга <sup>24.2</sup>

Добавлена возможность указывать [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/) во время рендеринга с использованием методов [ShapeRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) и [OfficeMathRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/).

#### Сохранять пустые строки при загрузке Markdown файлов <sup>24.2</sup>

Добавлена возможность сохранять пустые строки при загрузке файлов Markdown.

### Другой

- Возможность изменять текст элемента управления `TextBox` OLE была реализована путем добавления нового свойства **Text** к новому классу **TextBoxControl**. <sup>24.1</sup>
- Общедоступные источники библиографии API были реализованы путем добавления нового пространства имен [Aspose.Words.Bibliography](https://reference.aspose.com/words/cpp/aspose.words.bibliography/) с его новыми классами и перечислениями, а также путем добавления нового свойства [Bibliography](https://reference.aspose.com/words/cpp/aspose.words/document/get_bibliography/) к классу [Document](https://reference.aspose.com/words/cpp/aspose.words/document/). <sup>24.1</sup>
- В класс [Style](https://reference.aspose.com/words/cpp/aspose.words/style/) добавлены новые общедоступные свойства [Priority](https://reference.aspose.com/words/cpp/aspose.words/style/get_priority/), [UnhideWhenUsed](https://reference.aspose.com/words/cpp/aspose.words/style/get_unhidewhenused/) и [SemiHidden](https://reference.aspose.com/words/cpp/aspose.words/style/get_semihidden/) для улучшенного управления стилем. <sup>24.2</sup>
- Функциональность для получения фактического текста опорного знака для сносок и концевых сносок была расширена с помощью свойства [ActualReferenceMark](https://reference.aspose.com/words/cpp/aspose.words.notes/footnote/get_actualreferencemark/) и метода [UpdateActualReferenceMarks](https://reference.aspose.com/words/cpp/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
- Реализована эмуляция бинарных растровых операций для метафайлов WMF. <sup>24.3</sup>
- Возможность определять параметры подписи для документов в рамках **SaveOptions** была включена путем добавления нового класса **DigitalSignatureDetails** с новыми открытыми членами, а также добавления новых свойств к классам [OoxmlSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/docsaveoptions/) и [OdtSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Узнайте больше о [Aspose.Words для C++ 24.1 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-1-release-notes/).

Узнайте больше о [Aspose.Words для C++ 24.2 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-2-release-notes/).

Узнайте больше о [Aspose.Words для C++ 24.3 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-3-release-notes/).

Узнайте больше о [Aspose.Words для C++ 24.4 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words для C++ 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 расширяет возможности рендеринга, эмуляции рендеринга метафайлов и markdown сохранения.

Aspose.Words 23.10 улучшен рендеринг, расширены возможности загрузки и сохранения документов, а также пользователи могут по-новому объединять документы.

Aspose.Words 23.11 расширяет возможности работы с изменениями, XLSX форматированием и шрифтами в легенде диаграммы с помощью дополнительных опций.

Aspose.Words 23.12 добавлены новые свойства и перечисления для работы с PDF и OOXML документами, а также поддержка WebP изображений.

### Рендеринг и печать

#### Настройка названий осей в DrawingML диаграммах <sup>23.9</sup>

Возможность настраивать названия осей на диаграммах DrawingML появилась благодаря внедрению нового общедоступного класса **ChartAxisTitle** и свойства [Title](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartaxis/get_title/).

#### Определение вертикального расположения шрифтов в абзаце <sup>23.9</sup>

Теперь можно определять вертикальное расположение шрифтов в абзаце, используя новое свойство public [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/paragraphformat/get_baselinealignment/) и новое перечисление [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/baselinealignment/).

#### Управление цветом переднего плана <sup>23.10</sup>

Возможность извлекать цвет переднего плана без модификаторов была добавлена в классы [Fill](https://reference.aspose.com/words/cpp/aspose.words.drawing/fill/) и [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) с помощью свойства **BaseForeColor**.

#### Расширение функциональности графиков <sup>23.10</sup>

Функциональность классов [ChartDataPointCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartseries/) и [ChartFormat](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartformat/) была расширена за счет новых методов и свойств.

#### Автоматическая настройка и подгонка изображения под форму <sup>23.10</sup>

Новый метод [FitImageToShape](https://reference.aspose.com/words/cpp/aspose.words.drawing/imagedata/fitimagetoshape/) предоставляет простой способ автоматической настройки и подгонки изображения под определенную форму.

#### Форматирование шрифта по умолчанию для DrawingML записей в условных обозначениях диаграммы <sup>23.11</sup>

Добавлена возможность задавать форматирование шрифта по умолчанию для записей условных обозначений диаграмм DrawingML с помощью свойства [Font](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartlegend/get_font/). Эта функция обеспечивает более упорядоченный и единообразный внешний вид элементов диаграммы, улучшая общую эстетику документа.

#### Укажите макет страницы при открытии PDF в Reader <sup>23.12</sup>

Возможность указывать макет страницы, который будет использоваться при открытии документа в PDF ридере, была добавлена благодаря введению нового свойства **PageLayout** для класса [PdfSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/) и введению нового перечисления **PdfPageLayout**.

### Загрузка и сохранение документов

#### Указание имени папки для создания изображения URIs в Markdown <sup>23.9</sup>

Класс [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) был расширен за счет добавления свойства [ImagesFolderAlias](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imagesfolderalias/), которое позволяет указать имя папки, используемой для создания изображения URIs, записанного в документ Markdown.

#### Уменьшить PDF Размер выходных данных <sup>23.10</sup>

Были реализованы различные оптимизации PDF рендеринга для уменьшения размера выходных данных при использовании настроек [OptimizeOutput](https://reference.aspose.com/words/cpp/aspose.words.saving/fixedpagesaveoptions/get_optimizeoutput/).

#### Распознавать гиперссылки при загрузке TXT документов <sup>23.10</sup>

Функция распознавания гиперссылок при загрузке документов TXT была реализована путем добавления нового свойства [DetectHyperlinks](https://reference.aspose.com/words/cpp/aspose.words.loading/txtloadoptions/get_detecthyperlinks/).

### Другой

- Реализована эмуляция рендеринга метафайлов для определения размера растеризации, в частности, для WMF ширины пера и EMF косметической ширины пера. Для достижения этой цели свойство **ScaleWmfFontsToMetafileSize** было заменено свойством [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpage/) и добавлено свойство [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpageresolution/). <sup>23.9</sup>
* С использованием метода [InsertDocumentInline](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertdocumentinline/) был представлен упрощенный метод вставки одного документа в другой в текущем положении курсора. <sup>23.10</sup>
* Возможность доступа к свойствам стиля и их изменения была добавлена благодаря введению нового свойства [Locked](https://reference.aspose.com/words/cpp/aspose.words/style/get_locked/). <sup>23.10</sup>
* К методам класса [CompositeNode](https://reference.aspose.com/words/cpp/aspose.words/compositenode/) был добавлен параметр универсального типа. <sup>23.10</sup>
* С помощью методов [Accept](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/accept/) и [Reject](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/reject/) был реализован способ контроля того, когда определенная редакция должна быть принята/отклонена или нет. Это усовершенствование предоставляет пользователям более точный контроль над процессом внесения изменений. <sup>23.11</sup>
* Возможность записывать все разделы документа на один и тот же рабочий лист XLSX была предоставлена благодаря новому типу перечисления [XlsxSectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsectionmode/) и новому свойству [SectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsaveoptions/get_sectionmode/). <sup>23.11</sup>
* Способ управления тем, как расширения формата ZIP64 будут использоваться для документов OOXML, был реализован с помощью нового свойства Zip64Mode класса `OoxmlSaveOptions` и нового перечисления Zip64Mode. <sup>23.12</sup>
* Добавлена поддержка изображений WebP. Пожалуйста, обратите внимание, что эта функция доступна только для версий .NetStandart и .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Узнайте больше о [Aspose.Words для C++ 23.9 Примечания к выпуску](/words/cpp/aspose-words-for-cpp-23-9-release-notes/).
Узнайте больше о [Aspose.Words для C++ 23.10 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-10-release-notes/).
Узнайте больше о [Aspose.Words для C++ 23.11 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-11-release-notes/).
Узнайте больше о [Aspose.Words для C++ 23.12 Примечания к выпуску](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-12-release-notes/).

{{% /alert %}}

## Смотрите также

{{% alert color="primary" %}}

На этой странице представлены последние новости о релизах за последние 2 года. Более подробную информацию о предыдущих выпусках смотрите в [Примечания к выпуску'](/words/cpp/release-notes/) страницы в соответствующих разделах.

{{% /alert %}}
