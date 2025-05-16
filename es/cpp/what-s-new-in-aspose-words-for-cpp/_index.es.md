---
title: Qué hay de nuevo
second_title: Aspose.Words por C++
articleTitle: Qué hay de nuevo en Aspose.Words por C++
linktitle: Qué hay de nuevo en Aspose.Words por C++
type: docs
description: "Aspose.Words por C++ se expande y mejora a diario. En esta página, puede conocer las características enormes y más interesantes del producto."
weight: 2
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /es/cpp/what-s-new-in-aspose-words-for-cpp/
timestamp: 2025-04-15-08-02-05
---

Esta página describe las nuevas funciones Aspose.Words más interesantes introducidas en versiones recientes.

## Aspose.Words por C++ 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 presenta la revisión gramatical impulsada por AI y mejora el guardado de documentos con opciones avanzadas para los formatos HTML, SVG y Markdown.

Aspose.Words 25.2 introduce el resumen de texto con los modelos Anthropic AI, agrega compatibilidad con el formato MsWorks, mejora el control tipográfico y mejora la estructura PDF y el manejo de listas.

Aspose.Words 25.3 mejora un corrector gramatical con tecnología AI y la selección de fuentes con la propiedad UpdateAmbiguousTextFont, además de mejorar la exportación de archivos adjuntos PDF.

Aspose.Words 25.4 presenta compatibilidad con nuevos tamaños de papel, habilita el control avanzado de exportación de HTML, mejora el manejo de marcas de agua y mejora la usabilidad de LowCode API.

### AI - funciones potenciadas

#### Documento AI Revisión gramatical

* La capacidad de verificar la gramática del documento proporcionado utilizando OpenAI modelos generativos se ha introducido agregando un nuevo método [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/). <sup>25.1</sup>
* La función de revisión gramatical impulsada por AI se ha actualizado para admitir todos los modelos disponibles en la enumeración [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Resumen Usando Anthropic Modelos de Lenguaje Generativo <sup>25.2</sup>

Se ha habilitado la síntesis de texto utilizando Anthropic modelos de lenguaje generativo al introducir una nueva clase pública [AnthropicAiModel](https://reference.aspose.com/words/cpp/aspose.words.ai/).

### Low Code

#### Low Code API Usabilidad <sup>25.4</sup>

Se han introducido mejoras significativas en la usabilidad del **LowCode API**, simplificando el procesamiento de documentos y reduciendo la necesidad de código repetitivo.

### Formatos Admitidos <sup>25.2</sup>

A partir de la versión 25.2, se ha agregado compatibilidad con el nuevo formato de carga MsWorks para documentos Microsoft Works.

### Conversión, Carga y Guardado de Documentos

#### Guardado mejorado en formatos HTML y SVG <sup>25.1</sup>

Se ha mejorado el guardado en formatos HTML y SVG agregando propiedades **IdPrefix** y **RemoveJavaScriptFromLinks** a las clases [HtmlFixedSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlfixedsaveoptions/) y [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/).

#### Establezca la Resolución de la Imagen y el Modo de salida OfficeMath Al Guardar en Markdown <sup>25.1</sup>

- Se ha agregado una nueva opción [ImageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imageresolution/) a la clase [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) para establecer la resolución de la imagen.
- Se han agregado una nueva opción [OfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_officemathexportmode/) y enumeración [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownofficemathexportmode/) a la clase [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) para establecer el modo de salida OfficeMath.
- La capacidad de establecer una marca de agua de imagen a partir de una secuencia se ha introducido agregando una nueva sobrecarga al método [SetImage](https://reference.aspose.com/words/cpp/aspose.words/watermark/setimage/#watermarksetimageconst-systemsharedptrsystemiostream-const-systemsharedptrasposewordsimagewatermarkoptions-method). <sup>25.4</sup>

### Renderizado

#### Control Tipográfico Mejorado <sup>25.2</sup>

Se ha agregado la propiedad [NumberSpacing](https://reference.aspose.com/words/cpp/aspose.words/font/get_numberspacing/) para mejorar el control tipográfico.

#### Control de la Selección de Fuentes para Caracteres Ambiguos <sup>25.3</sup>

Se ha agregado una nueva propiedad pública [UpdateAmbiguousTextFont](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/get_updateambiguoustextfont/) a la clase [SaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/) para controlar la selección de fuentes de acuerdo con el código de caracteres utilizado.

#### Opciones de Tamaño de Papel <sup>25.4</sup>

Se ha introducido la capacidad de usar tamaños de papel JIS B4 y JIS B5 agregando nuevos valores a la enumeración [PaperSize](https://reference.aspose.com/words/cpp/aspose.words/papersize/).

#### HTML Control de Salida <sup>25.4</sup>

Se ha introducido la capacidad de eliminar JavaScript del hipervínculo URLs durante la exportación de HTML agregando la propiedad [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlsaveoptions/get_removejavascriptfromlinks/).

### Otros

* La estructura lógica de PDF se ha mejorado con la compatibilidad con los campos TOA, BIBLIOGRAPHY y INDEX. <sup>25.2</sup>
* El método [AddSingleLevelList](https://reference.aspose.com/words/cpp/aspose.words.lists/listcollection/addsinglelevellist/) se ha introducido para mejorar el manejo de listas. <sup>25.2</sup>
* Se ha agregado una nueva propiedad [AttachmentsEmbeddingMode](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/get_attachmentsembeddingmode/) para reemplazar **EmbedAttachments** y mejorar la exportación de PDF archivos adjuntos. Además, se han agregado nuevos valores a la enumeración [PdfCompliance](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfcompliance/) para admitir archivos adjuntos de la versión PDF/A. Además, los archivos adjuntos ahora son compatibles con el cifrado. <sup>25.3</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por C++ 25.1 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-1-release-notes/).

Más información sobre [Aspose.Words por C++ 25.2 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-2-release-notes/).

Más información sobre [Aspose.Words por C++ 25.3 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-3-release-notes/).

Más información sobre [Aspose.Words por C++ 25.4 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words por C++ 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduce la inserción group shape y la inserción StructuredDocumentTag a través de DocumentBuilder, mejora la representación de gráficos radiales con graduaciones, mejora las firmas digitales con compatibilidad con XAdES-EPES, agrega reconocimiento de subrayado Markdown y proporciona acceso a separadores de notas al pie/notas al final.

Aspose.Words 24.10 presenta compatibilidad mejorada con el control ActiveX con la creación de CommandButton, nuevo control de visibilidad de formas, la capacidad de group shapes, exportación mejorada de Markdown para tablas, formato de gráficos para Pie y Doughnut, mejor manejo de codificación Big5 y compatibilidad con fuentes taiwanesas obsoletas.

Aspose.Words 24.11 presenta un resumen de documentos impulsado por AI, opciones de representación mejoradas, acceso mejorado a las propiedades del documento y subtítulos de control ActiveX.

Aspose.Words 24.12 presenta la colocación personalizable de etiquetas de datos, la traducción de texto impulsada por Google AI, las opciones mejoradas de limpieza de Mail Merge y las nuevas clases de procesamiento de LowCode.

### AI - funciones potenciadas

#### Resumen de documentos Usando OpenAI y Google <sup>24.11</sup>

Se ha integrado el soporte para el resumen de documentos utilizando modelos de lenguaje generativo **OpenAI** y **Google**.

#### Traducción de texto utilizando los modelos de lenguaje generativo de Google <sup>24.12</sup>

La capacidad de traducir texto utilizando los modelos de lenguaje generativo de Google se implementó en Aspose.Words al agregar el método [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) y la enumeración [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) al espacio de nombres [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Nuevas LowCode clases como [Comparer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/cpp/aspose.words.lowcode/merger/), [Replacer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/cpp/aspose.words.lowcode/splitter/) etc. se ha introducido un conjunto de métodos que logran el equilibrio perfecto entre simplicidad y flexibilidad para el procesamiento de documentos.

### Renderizado e Impresión

#### Graduaciones en Gráficos Radiales <sup>24.9</sup>

Se ha implementado la representación de graduaciones en gráficos radiales.

#### CommandButton ActiveX Controles <sup>24.10</sup>

La capacidad de crear controles CommandButton ActiveX se ha introducido agregando un nuevo método público [InsertForms2OleControl](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertforms2olecontrol/) y una nueva clase pública **Forms2OleControl**.

#### Controlar la Visibilidad de la Forma <sup>24.10</sup>

Se ha agregado una nueva propiedad pública [Hidden](https://reference.aspose.com/words/cpp/aspose.words.drawing/shapebase/get_hidden/) para controlar la visibilidad de las formas.

#### Cambios en los gráficos Pie y Doughnut <sup>24.10</sup>

Se han agregado varias propiedades públicas nuevas a los gráficos de formato Pie y Doughnut.

#### Controle la representación de los Bordes de los Campos del Formulario de Elección PDF <sup>24.11</sup>

Se ha implementado una nueva opción para controlar la representación de los bordes de los campos de formulario de elección PDF agregando una nueva opción pública **RenderChoiceFormFieldBorder**.

#### Obtenga y Configure Códigos de Formato para Datos de Gráficos <sup>24.11</sup>

Se ha agregado la capacidad de obtener y establecer códigos de formato para datos de gráficos implementando la propiedad **FormatCode** en las clases [ChartXValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartyvaluecollection/) y [BubbleSizeCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/bubblesizecollection/).

#### Renderice Gráficos de Histogramas con Contenedores y Etiquetas <sup>24.11</sup>

La representación del gráfico de histogramas se ha mejorado al permitir un número específico de contenedores y etiquetas.

#### Personalice la Ubicación de las Etiquetas de Datos <sup>24.12</sup>

Se ha agregado la capacidad de personalizar la ubicación de las etiquetas de datos al introducir nuevas propiedades en las clases [ChartDataLabel](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabel/) y [ChartDataLabelCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabelcollection/).

### Conversión, Carga y Guardado de Documentos

#### Subrayar el formato al Cargar Markdown Archivos <sup>24.9</sup>

Se ha incorporado la opción de reconocer el formato subrayado al cargar documentos Markdown agregando una nueva propiedad pública **ImportUnderlineFormatting**.

#### Exportar tablas como HTML al guardar en Markdown <sup>24.10</sup>

Se ha implementado una opción para exportar tablas como HTML al guardar documentos en formato Markdown agregando una nueva propiedad pública [ExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_exportashtml/) y una enumeración [MarkdownExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownexportashtml/).

#### Exportar PDF con Estructura Lógica Actualizada <sup>24.11</sup>

La exportación PDF se ha mejorado al incluir las propiedades del título de la tabla como títulos de los elementos de la estructura lógica PDF.

### Mail Merge y Presentación de Informes

#### Eliminar Tablas vacías durante Mail Merge <sup>24.12</sup>

Se ha agregado una nueva opción **RemoveEmptyTables** a la enumeración [MailMergeCleanupOptions](https://reference.aspose.com/words/cpp/aspose.words.mailmerging/mailmergecleanupoptions/) para refinar la salida Mail Merge.

### Firmas Digitales

#### Firme documentos con XAdES-EPES <sup>24.9</sup>

Se ha introducido la capacidad de firmar documentos con firmas XAdES-EPES de nivel XML-DSig agregando una nueva propiedad pública **XmlDsigLevel** y una nueva enumeración pública **XmlDsigLevel**.

### Otros

* Se ha agregado un nuevo método público [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/) a group shapes. <sup>24.9</sup>
* Se ha agregado un nuevo método público [InsertStructuredDocumentTag](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertstructureddocumenttag/) para insertar **StructuredDocumentTags** en un documento. <sup>24.9</sup>
* Se ha proporcionado acceso público a los separadores de notas al pie/notas al final agregando algunas clases y propiedades públicas. <sup>24.9</sup>
* La capacidad de agrupar formas individuales, group shapes juntas y agrupar directamente ambas formas y group shapes se ha introducido agregando el método [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/). <sup>24.10</sup>
* Se ha mejorado el manejo de la codificación Big5 para TrueType tablas cmap. <sup>24.10</sup>
* Se ha mejorado la compatibilidad con fuentes taiwanesas obsoletas. <sup>24.10</sup>
* Para acceder a las propiedades extendidas del documento, se han agregado propiedades de solo lectura a la clase **BuiltInDocumentProperties**. <sup>24.11</sup>
* Se ha habilitado la configuración de subtítulos para los controles ActiveX agregando un nuevo configurador público a la propiedad **Forms2OleControl.Caption**. <sup>24.11</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por C++ 24.9 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-9-release-notes/).

Más información sobre [Aspose.Words por C++ 24.10 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-10-release-notes/).

Más información sobre [Aspose.Words por C++ 24.11 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-11-release-notes/).

Más información sobre [Aspose.Words por C++ 24.12 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words por C++ 24.5, 24.6, 24.7

Aspose.Words 24.5 expande las opciones para ensamblados, mejora las capacidades de representación y expande algunas otras opciones.

Aspose.Words 24.6 mejora las opciones de representación, mejora la funcionalidad de búsqueda y comparación y amplía varias otras funciones.

Aspose.Words 24.7 cambia la forma de trabajar con ActiveX, amplía las capacidades de renderizado y exporta a formatos Markdown y XLSX.

### Formatos Admitidos

A partir de la versión 24.7, se admite la exportación a PDF/UA-2 para garantizar la accesibilidad de los usuarios con discapacidades.

### Renderizado e Impresión

#### Cambios en Gráficos, Formas y DrawingML <sup>24.5</sup>

- Se ha implementado la representación de efectos DrawingML para gráficos SVG, ampliando la funcionalidad anterior limitada a imágenes.
- Se ha agregado compatibilidad para crear gráficos combinados y ajustar propiedades como el ancho del espacio, la superposición y la escala de burbujas dentro de los grupos de series agregando las clases **ChartSeriesGroup** y **ChartSeriesGroupCollection** y la propiedad **SeriesGroups**.
- La funcionalidad para manipular el efecto SoftEdge de las formas se ha implementado agregando la clase **SoftEdgeFormat**.
- La capacidad de modificar los valores adjust de las formas se ha implementado agregando las clases públicas **AdjustmentCollection** y **Adjustment** y la propiedad **Adjustments**.

#### Cambios en Gráficos, Formas y Dibujos <sup>24.6</sup>

- Se han mejorado las capacidades de creación de gráficos. Ahora puede crear una variedad más amplia de gráficos, que incluyen *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* gráficos, *Box & Whisker* gráficos, *Waterfalls* y *Funnels*. Esto le permite visualizar sus datos de una manera más diversa e informativa.
- Se ha mejorado el control del color para el formato de las sombras. Puede obtener un control más preciso sobre la apariencia de sus documentos accediendo a los colores de las sombras.
- Se ha mejorado el aumento del rendimiento del renderizado en segundo plano. Puede acelerar significativamente la representación de fondos que contienen elementos pequeños gracias a la tecnología de mosaico nativa.
- Se han añadido degradados realistas para las formas. Ahora puede crear formas DML con degradados no lineales, imitando el estilo visual de Microsoft Word para una apariencia más pulida.

#### Personalización de Etiquetas de Datos de Gráficos <sup>24.7</sup>

Se ha agregado la capacidad de personalizar etiquetas de datos de gráficos como **Orientation** y **Rotation**.

#### Estilo de Número Personalizado para Niveles de Lista <sup>24.7</sup>

Se ha agregado un colocador para la propiedad pública [CustomNumberStyleFormat](https://reference.aspose.com/words/cpp/aspose.words.lists/listlevel/get_customnumberstyleformat/). Ahora puede definir un estilo de número personalizado para los niveles de lista.

#### Cambios al trabajar con ActiveX <sup>24.7</sup>

- Las propiedades de los objetos ActiveX ahora se pueden modificar, lo que le brinda más control sobre su comportamiento.
- Se ha agregado la capacidad de modificar el valor del control del botón de opción ActiveX para habilitar la interacción dinámica.
- Se ha agregado la capacidad de alternar un ActiveX checkbox a "marcado" o "desmarcado".

### Cargar y Guardar Documentos

#### Exportación de enlaces al formato Markdown <sup>24.7</sup>

Se ha agregado la capacidad de controlar la exportación de enlaces en formato Markdown mediante la implementación de la propiedad [LinkExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_linkexportmode/).

### Buscar y Comparar

#### Opciones Avanzadas de Comparación <sup>24.6</sup>

Se ha agregado la capacidad de agilizar los flujos de trabajo de análisis de datos con una funcionalidad de comparación mejorada. Esto incluye una nueva opción **IgnoreStoreItemId** y una interfaz rediseñada para comparaciones avanzadas.

### Otros

- La función para eliminar páginas vacías de un documento se ha implementado agregando el método [RemoveBlankPages](https://reference.aspose.com/words/cpp/aspose.words/document/removeblankpages/). <sup>24.5</sup>
- Se ha proporcionado la capacidad de verificar la presencia de VBA macros sin cargar un documento agregando la propiedad **HasMacros**. <sup>24.5</sup>
- Se ha agregado una nueva propiedad **DateTimeUtc** que proporciona una marca de tiempo más precisa para los comentarios, mejorando la organización y la trazabilidad. <sup>24.6</sup>
- El formato de fecha y hora ahora se detecta automáticamente para una exportación perfecta al formato XLSX. <sup>24.7</sup>
- Se ha agregado la propiedad pública [IsProtected](https://reference.aspose.com/words/cpp/aspose.words.vba/vbaproject/get_isprotected/), que le permite verificar si un proyecto VBA está protegido. <sup>24.7</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por C++ 24.5 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-5-release-notes/).

Más información sobre [Aspose.Words por C++ 24.6 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-6-release-notes/).

Más información sobre [Aspose.Words por C++ 24.7 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-7-release-notes/).

{{% /alert %}}

## Aspose.Words por C++ 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 mejora la experiencia en torno a la administración de los colores de los trazos, mejora los objetos OLE e introduce una nueva Fuente de Bibliografía pública API.

Aspose.Words 24.2 gráficos expandidos API y gestión de estilos. Esta versión de Aspose.Words también introdujo la capacidad de especificar SvgSaveOptions durante el procesamiento, un control más flexible para cargar archivos Markdown y trabajar con texto de referencia para notas al pie y notas al final.

Aspose.Words 24.3 introduce la emulación de operaciones ráster binarias para WMF metarchivos y también continúa expandiendo los Gráficos API.

Aspose.Words 24.4 mejora algunas opciones de representación, así como el trabajo con firmas digitales.

### Renderizado e Impresión

#### Control de Color de Trazo <sup>24.1</sup>

La clase [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) se ha ampliado con un conjunto de nuevas propiedades públicas relacionadas con la administración de los colores de trazo: [ForeThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_forethemecolor/) y [BackThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_foretintandshade/) y [BackTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backtintandshade/).

#### Extensión DrawingML Gráficos API <sup>24.2 / 24.3 / 24.4</sup>

El **DrawingML Charts API** continúa expandiéndose.

#### Incrustar fuentes Declaradas en @font-face Reglas <sup>24.4</sup>

Se agregó la capacidad de incrustar fuentes declaradas en las reglas @font-face en las definiciones de fuentes del documento resultante agregando una nueva propiedad [SupportFontFaceRules](https://reference.aspose.com/words/cpp/aspose.words.loading/htmlloadoptions/get_supportfontfacerules/).

#### Trabajar con Formato de Resplandor y Reflejo <sup>24.4</sup>

Se ha implementado la capacidad de trabajar con formato de resplandor y reflejo para un objeto de dibujo.

### Cargar y Guardar Documentos

#### Especifique SvgSaveOptions Durante el Procesamiento <sup>24.2</sup>

La capacidad de especificar [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/) durante el renderizado se ha agregado usando [ShapeRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) y [OfficeMathRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) métodos.

#### Conservar las Líneas Vacías al Cargar Markdown archivos <sup>24.2</sup>

Se ha agregado la capacidad de conservar líneas vacías al cargar archivos Markdown.

### Otros

- Se ha introducido la capacidad de modificar el texto del control `TextBox` OLE agregando una nueva propiedad **Text** a la nueva clase **TextBoxControl**. <sup>24.1</sup>
- Las Fuentes de Bibliografía public API se implementaron agregando un nuevo espacio de nombres [Aspose.Words.Bibliography](https://reference.aspose.com/words/cpp/aspose.words.bibliography/) con sus nuevas clases y enumeraciones, y agregando una nueva propiedad [Bibliography](https://reference.aspose.com/words/cpp/aspose.words/document/get_bibliography/) a la clase [Document](https://reference.aspose.com/words/cpp/aspose.words/document/). <sup>24.1</sup>
- Se han agregado nuevas propiedades públicas [Priority](https://reference.aspose.com/words/cpp/aspose.words/style/get_priority/), [UnhideWhenUsed](https://reference.aspose.com/words/cpp/aspose.words/style/get_unhidewhenused/) y [SemiHidden](https://reference.aspose.com/words/cpp/aspose.words/style/get_semihidden/) para una mejor administración de estilos a la clase [Style](https://reference.aspose.com/words/cpp/aspose.words/style/). <sup>24.2</sup>
- La funcionalidad para recuperar el texto real de la marca de referencia para notas al pie y notas al final se ha mejorado con la propiedad [ActualReferenceMark](https://reference.aspose.com/words/cpp/aspose.words.notes/footnote/get_actualreferencemark/) y el método [UpdateActualReferenceMarks](https://reference.aspose.com/words/cpp/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
- Se ha implementado la emulación de operaciones ráster binarias para metarchivos WMF. <sup>24.3</sup>
- La capacidad de definir opciones de firma para documentos dentro de **SaveOptions** se ha habilitado agregando una nueva clase **DigitalSignatureDetails** con nuevos miembros públicos, así como agregando nuevas propiedades a las clases [OoxmlSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/docsaveoptions/) y [OdtSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por C++ 24.1 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-1-release-notes/).

Más información sobre [Aspose.Words por C++ 24.2 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-2-release-notes/).

Más información sobre [Aspose.Words por C++ 24.3 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-3-release-notes/).

Más información sobre [Aspose.Words por C++ 24.4 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words por C++ 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 expande las opciones de representación, la emulación de representación de metarchivo y las opciones de guardado markdown.

Aspose.Words 23.10 mejora el renderizado, amplía las opciones para cargar y guardar documentos y permite a los usuarios fusionar documentos de nuevas formas.

Aspose.Words 23.11 mejora el trabajo con revisiones, formato XLSX y fuentes en la leyenda del gráfico con opciones adicionales.

Aspose.Words 23.12 introduce nuevas propiedades y enumeraciones para trabajar con documentos PDF y OOXML, así como compatibilidad con imágenes WebP.

### Renderizado e Impresión

#### Personalización de Títulos de Ejes en Gráficos DrawingML <sup>23.9</sup>

La capacidad de personalizar los títulos de los ejes en los gráficos DrawingML se ha introducido mediante la implementación de una nueva propiedad pública de clase **ChartAxisTitle** y [Title](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartaxis/get_title/).

#### Determinar la Posición Vertical de las Fuentes dentro de un Párrafo <sup>23.9</sup>

Ahora es posible definir la posición vertical de las fuentes dentro de un párrafo utilizando la nueva propiedad public [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/paragraphformat/get_baselinealignment/) y la nueva enumeración [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/baselinealignment/).

#### Control de Color de Primer Plano <sup>23.10</sup>

La capacidad de recuperar el color de primer plano sin modificadores se ha agregado a las clases [Fill](https://reference.aspose.com/words/cpp/aspose.words.drawing/fill/) y [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) a través de la propiedad **BaseForeColor**.

#### Ampliación de la Funcionalidad de los Gráficos <sup>23.10</sup>

La funcionalidad de las clases [ChartDataPointCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartseries/) y [ChartFormat](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartformat/) se ha ampliado con nuevos métodos y propiedades.

#### Ajusta y ajusta Automáticamente una Imagen en una Forma <sup>23.10</sup>

Se ha proporcionado una forma sencilla de ajustar y ajustar automáticamente una imagen dentro de una forma particular a través del nuevo método [FitImageToShape](https://reference.aspose.com/words/cpp/aspose.words.drawing/imagedata/fitimagetoshape/).

#### Formato de fuente Predeterminado para las Entradas de Leyenda de Gráfico DrawingML <sup>23.11</sup>

Se ha agregado la capacidad de especificar el formato de fuente predeterminado para las entradas de leyenda de los gráficos DrawingML a través de la propiedad [Font](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartlegend/get_font/). Esta característica facilita una apariencia más optimizada y consistente para los elementos del gráfico, mejorando la estética general del documento.

#### Especifique el Diseño de página al Abrir PDF en Reader <sup>23.12</sup>

Se ha agregado la capacidad de especificar el diseño de página que se utilizará al abrir un documento en un lector PDF mediante la introducción de una nueva propiedad **PageLayout** en la clase [PdfSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/) y la introducción de una nueva enumeración **PdfPageLayout**.

### Cargar y Guardar Documentos

#### Especificar un Nombre de Carpeta para Construir la Imagen URIs en Markdown <sup>23.9</sup>

La clase [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) se ha ampliado al incluir la propiedad [ImagesFolderAlias](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imagesfolderalias/), que permite especificar el nombre de la carpeta utilizada para construir la imagen URIs escrita en el documento Markdown.

#### Reducir el Tamaño de Salida PDF <sup>23.10</sup>

Se han implementado varias optimizaciones de renderizado PDF para reducir el tamaño de salida al utilizar la configuración [OptimizeOutput](https://reference.aspose.com/words/cpp/aspose.words.saving/fixedpagesaveoptions/get_optimizeoutput/).

#### Reconocer Hipervínculos al Cargar Documentos TXT <sup>23.10</sup>

La función para reconocer hipervínculos al cargar documentos TXT se ha implementado agregando una nueva propiedad [DetectHyperlinks](https://reference.aspose.com/words/cpp/aspose.words.loading/txtloadoptions/get_detecthyperlinks/).

### Otros

- Se ha implementado la emulación de representación de metarchivo para determinar el tamaño de rasterización, específicamente para el ancho del lápiz WMF y el ancho del lápiz cosmético EMF. Para lograr esto, la propiedad **ScaleWmfFontsToMetafileSize** se reemplazó con la propiedad [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpage/) y se agregó la propiedad [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpageresolution/). <sup>23.9</sup>
* Se ha introducido un método simplificado para insertar un documento en otro documento en la posición actual del cursor utilizando el método [InsertDocumentInline](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertdocumentinline/). <sup>23.10</sup>
* La capacidad de acceder y modificar propiedades de estilo se ha agregado mediante la introducción de la nueva propiedad [Locked](https://reference.aspose.com/words/cpp/aspose.words/style/get_locked/). <sup>23.10</sup>
* Se ha agregado un parámetro de tipo genérico a los métodos de la clase [CompositeNode](https://reference.aspose.com/words/cpp/aspose.words/compositenode/). <sup>23.10</sup>
* Se ha implementado una forma de controlar cuándo se debe aceptar/rechazar o no una determinada revisión utilizando los métodos [Accept](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/accept/) y [Reject](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/reject/). Esta mejora otorga a los usuarios un control más preciso sobre el proceso de revisión. <sup>23.11</sup>
* La capacidad de escribir todas las secciones de un documento en la misma hoja de cálculo XLSX se ha proporcionado a través del nuevo tipo de enumeración [XlsxSectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsectionmode/) y la nueva propiedad [SectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsaveoptions/get_sectionmode/). <sup>23.11</sup>
* Se ha implementado una forma de controlar cómo se utilizarán las extensiones de formato ZIP64 para los documentos OOXML a través de la nueva propiedad Zip64Mode de la clase `OoxmlSaveOptions` y la nueva enumeración Zip64Mode. <sup>23.12</sup>
* Se ha introducido soporte para la imagen WebP. Tenga en cuenta que esta función solo está disponible para .versiones NetStandart y .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por C++ 23.9 Notas de la versión](/words/cpp/aspose-words-for-cpp-23-9-release-notes/).
Más información sobre [Aspose.Words por C++ 23.10 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-10-release-notes/).
Más información sobre [Aspose.Words por C++ 23.11 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-11-release-notes/).
Más información sobre [Aspose.Words por C++ 23.12 Notas de la versión](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-12-release-notes/).

{{% /alert %}}

## Véase También

{{% alert color="primary" %}}

Esta página contiene las últimas noticias de lanzamiento de los últimos 2 años. Para obtener detalles sobre versiones anteriores, consulte [Notas de la versión'](/words/cpp/release-notes/) páginas en las secciones relevantes.

{{% /alert %}}
