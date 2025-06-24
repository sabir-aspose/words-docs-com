---
title: Qué hay de nuevo
second_title: Aspose.Words por Java
articleTitle: Qué hay de nuevo en Aspose.Words por Java
linktitle: Qué hay de nuevo en Aspose.Words por Java
type: docs
description: "Aspose.Words por Java se expande y mejora a diario. En esta página, puede conocer las características enormes y más interesantes del producto."
weight: 2
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /es/java/what-s-new-in-aspose-words-for-java/
timestamp: 2025-06-23-21-02-49
---

Esta página describe las nuevas funciones Aspose.Words más interesantes introducidas en versiones recientes.

## Aspose.Words por Java 25.5, 25.6

Aspose.Words 25.5 mejora la personalización de los gráficos con nuevas opciones de estilo y mejora la exportación de Markdown al ofrecer control sobre cómo se manejan los párrafos vacíos.

Aspose.Words 25.6 mejora la precisión de representación y las funciones de visualización al introducir opciones avanzadas de exportación de imágenes, manejo mejorado de MathML y mejor representación de gráficos.

### Conversión, Carga y Guardado de Documentos

#### Exportar Párrafos vacíos a Markdown <sup>25.5</sup>

Se ha introducido la capacidad de controlar cómo se exportan los párrafos vacíos a Markdown agregando la enumeración [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownemptyparagraphexportmode/) y la propiedad [EmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getEmptyParagraphExportMode).

#### Exporte Documentos de Varias páginas a Formatos de Imagen Rasterizada <sup>25.6</sup>

Se ha introducido la capacidad de exportar documentos de varias páginas a formatos de imagen ráster (como PNG y JPEG) con [customizable layouts](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) (Horizontal, Vertical o Cuadrícula) al ampliar la funcionalidad de exportación de imágenes.

### Renderizado

#### Configuración del Estilo del Gráfico <sup>25.5</sup>

La capacidad de establecer el estilo del gráfico se ha introducido agregando la enumeración [ChartStyle](https://reference.aspose.com/words/java/com.aspose.words/chartstyle/) y la propiedad [Style](https://reference.aspose.com/words/java/com.aspose.words/chart/#getStyle).

#### Representación de Líneas de Conector en MathML Expresiones <sup>25.6</sup>

La representación de líneas de conexión en expresiones MathML se ha implementado para garantizar una visualización más precisa y visualmente coherente de las fórmulas matemáticas.

#### Leyendas de Renderizado para Gráficos en Cascada <sup>25.6</sup>

Se ha introducido la representación de leyendas para ["Waterfall" charts](https://reference.aspose.com/words/java/com.aspose.words/chartseriestype/), lo que aumenta la transparencia de los datos y mejora la interpretabilidad de estos gráficos.

### Otros

* Se ha mejorado la capacidad de ajustar fórmulas matemáticas que contienen varias barras inclinadas, mejorando la claridad del diseño y la legibilidad de la fórmula. <sup>25.6</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words para Java 25.5 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-5-release-notes/).

Más información sobre [Aspose.Words para Java 25.6 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words por Java 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 presenta la revisión gramatical impulsada por AI y mejora el guardado de documentos con opciones avanzadas para los formatos HTML, SVG y Markdown.

Aspose.Words 25.2 introduce el resumen de texto con los modelos Anthropic AI, agrega compatibilidad con el formato MsWorks, mejora el control tipográfico y mejora la estructura PDF y el manejo de listas.

Aspose.Words 25.3 mejora un corrector gramatical con tecnología AI y la selección de fuentes con la propiedad UpdateAmbiguousTextFont, además de mejorar la exportación de archivos adjuntos PDF.

Aspose.Words 25.4 presenta compatibilidad con nuevos tamaños de papel, habilita el control avanzado de exportación de HTML, mejora el manejo de marcas de agua y mejora la usabilidad de LowCode API.

### AI - funciones potenciadas

#### Documento AI Revisión gramatical

* La capacidad de verificar la gramática del documento proporcionado utilizando OpenAI modelos generativos se ha introducido agregando un nuevo método [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions). <sup>25.1</sup>
* La función de revisión gramatical impulsada por AI se ha actualizado para admitir todos los modelos disponibles en la enumeración [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/). <sup>25.3</sup>

#### Resumen Usando Anthropic Modelos de Lenguaje Generativo <sup>25.2</sup>

Se ha habilitado la síntesis de texto utilizando Anthropic modelos de lenguaje generativo al introducir una nueva clase pública [AnthropicAiModel](https://reference.aspose.com/words/java/com.aspose.words/anthropicaimodel/).

### Low Code

#### Low Code API Usabilidad <sup>25.4</sup>

Se han introducido mejoras significativas en la usabilidad del **LowCode API**, simplificando el procesamiento de documentos y reduciendo la necesidad de código repetitivo.

### Formatos Admitidos <sup>25.2</sup>

A partir de la versión 25.2, se ha agregado compatibilidad con el nuevo formato de carga MsWorks para documentos Microsoft Works.

### Conversión, Carga y Guardado de Documentos

#### Guardado mejorado en formatos HTML y SVG <sup>25.1</sup>

Se ha mejorado el guardado en formatos HTML y SVG agregando propiedades **IdPrefix** y **RemoveJavaScriptFromLinks** a las clases [HtmlFixedSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlfixedsaveoptions/) y [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/).

#### Establezca la Resolución de la Imagen y el Modo de salida OfficeMath Al Guardar en Markdown <sup>25.1</sup>

* Se ha agregado una nueva opción [ImageResolution](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImageResolution) a la clase [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) para establecer la resolución de la imagen.
* Se han agregado una nueva opción [OfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getOfficeMathExportMode) y enumeración [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownofficemathexportmode/) a la clase [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) para establecer el modo de salida OfficeMath.
* La capacidad de establecer una marca de agua de imagen a partir de una secuencia se ha introducido agregando una nueva sobrecarga al método [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.io.InputStream-com.aspose.words.ImageWatermarkOptions). <sup>25.4</sup>

### Renderizado

#### Control Tipográfico Mejorado <sup>25.2</sup>

Se ha agregado la propiedad [NumberSpacing](https://reference.aspose.com/words/java/com.aspose.words/font/#getNumberSpacing) para mejorar el control tipográfico.

#### Control de la Selección de Fuentes para Caracteres Ambiguos <sup>25.3</sup>

Se ha agregado una nueva propiedad pública [UpdateAmbiguousTextFont](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/#getUpdateAmbiguousTextFont) a la clase [SaveOptions](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/) para controlar la selección de fuentes de acuerdo con el código de caracteres utilizado.

#### Opciones de Tamaño de Papel <sup>25.4</sup>

Se ha introducido la capacidad de usar tamaños de papel JIS B4 y JIS B5 agregando nuevos valores a la enumeración [PaperSize](https://reference.aspose.com/words/java/com.aspose.words/papersize/).

#### HTML Control de Salida <sup>25.4</sup>

Se ha introducido la capacidad de eliminar JavaScript del hipervínculo URLs durante la exportación de HTML agregando la propiedad [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/#getRemoveJavaScriptFromLinks).

### Otros

* La estructura lógica de PDF se ha mejorado con la compatibilidad con los campos TOA, BIBLIOGRAPHY y INDEX. <sup>25.2</sup>
* El método [AddSingleLevelList](https://reference.aspose.com/words/java/com.aspose.words/listcollection/#addSingleLevelList-int) se ha introducido para mejorar el manejo de listas. <sup>25.2</sup>
* Se ha agregado una nueva propiedad [AttachmentsEmbeddingMode](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getAttachmentsEmbeddingMode) para reemplazar **EmbedAttachments** y mejorar la exportación de PDF archivos adjuntos. Además, se han agregado nuevos valores a la enumeración [PdfCompliance](https://reference.aspose.com/words/java/com.aspose.words/pdfcompliance/) para admitir archivos adjuntos de la versión PDF/A. Además, los archivos adjuntos ahora son compatibles con el cifrado. <sup>25.3</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por Java 25.1 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-1-release-notes/).

Más información sobre [Aspose.Words por Java 25.2 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-2-release-notes/).

Más información sobre [Aspose.Words por Java 25.3 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-3-release-notes/).

Más información sobre [Aspose.Words por Java 25.4 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words por Java 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduce la inserción group shape y la inserción StructuredDocumentTag a través de DocumentBuilder, mejora la representación de gráficos radiales con graduaciones, mejora las firmas digitales con compatibilidad con XAdES-EPES, agrega reconocimiento de subrayado Markdown y proporciona acceso a separadores de notas al pie/notas al final.

Aspose.Words 24.10 presenta compatibilidad mejorada con el control ActiveX con la creación de CommandButton, nuevo control de visibilidad de formas, la capacidad de group shapes, exportación mejorada de Markdown para tablas, formato de gráficos para Pie y Doughnut, mejor manejo de codificación Big5 y compatibilidad con fuentes taiwanesas obsoletas.

Aspose.Words 24.11 presenta un resumen de documentos impulsado por AI, opciones de representación mejoradas, acceso mejorado a las propiedades del documento y subtítulos de control ActiveX.

Aspose.Words 24.12 presenta la colocación personalizable de etiquetas de datos, la traducción de texto impulsada por Google AI, las opciones mejoradas de limpieza de Mail Merge y las nuevas clases de procesamiento de LowCode.

### AI - funciones potenciadas

#### Resumen de documentos Usando OpenAI y Google <sup>24.11</sup>

Se ha integrado el soporte para el resumen de documentos utilizando modelos de lenguaje generativo **OpenAI** y **Google**.

#### Traducción de texto utilizando los modelos de lenguaje generativo de Google <sup>24.12</sup>

La capacidad de traducir texto utilizando los modelos de lenguaje generativo de Google se implementó en Aspose.Words agregando el método [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) y la enumeración [Language](https://reference.aspose.com/words/java/com.aspose.words/language/).

### Low Code <sup>24.12</sup>

Nuevas LowCode clases como [Comparer](https://reference.aspose.com/words/java/com.aspose.words/comparer/), [MailMerger](https://reference.aspose.com/words/java/com.aspose.words/mailmerger/), [Replacer](https://reference.aspose.com/words/java/com.aspose.words/replacer/), [Splitter](https://reference.aspose.com/words/java/com.aspose.words/splitter/) etc. se ha introducido un conjunto de métodos que logran el equilibrio perfecto entre simplicidad y flexibilidad para el procesamiento de documentos.

### Renderizado e Impresión

#### Graduaciones en Gráficos Radiales <sup>24.9</sup>

Se ha implementado la representación de graduaciones en gráficos radiales.

#### CommandButton ActiveX Controles <sup>24.10</sup>

La capacidad de crear controles CommandButton ActiveX se ha introducido agregando un nuevo método público [InsertForms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertForms2OleControl-com.aspose.words.Forms2OleControl) y una nueva clase pública [Forms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/).

#### Controlar la Visibilidad de la Forma <sup>24.10</sup>

Se ha agregado una nueva propiedad pública [Hidden](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#getHidden) para controlar la visibilidad de las formas.

#### Cambios en los gráficos Pie y Doughnut <sup>24.10</sup>

Se han agregado varias propiedades públicas nuevas a los gráficos de formato Pie y Doughnut.

#### Controle la representación de los Bordes de los Campos del Formulario de Elección PDF <sup>24.11</sup>

Se ha implementado una nueva opción para controlar la representación de los bordes de los campos de formulario de elección PDF agregando una nueva opción pública [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getRenderChoiceFormFieldBorder).

#### Obtenga y Configure Códigos de Formato para Datos de Gráficos <sup>24.11</sup>

Se ha agregado la capacidad de obtener y establecer códigos de formato para datos de gráficos implementando la propiedad [FormatCode](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/#getFormatCode) en las clases [ChartXValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartyvaluecollection/) y [BubbleSizeCollection](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/).

#### Renderice Gráficos de Histogramas con Contenedores y Etiquetas <sup>24.11</sup>

La representación del gráfico de histogramas se ha mejorado al permitir un número específico de contenedores y etiquetas.

### Conversión, Carga y Guardado de Documentos

#### Subrayar el formato al Cargar Markdown Archivos <sup>24.9</sup>

Se ha incorporado la opción de reconocer el formato subrayado al cargar documentos Markdown agregando una nueva propiedad pública [ImportUnderlineFormatting](https://reference.aspose.com/words/java/com.aspose.words/markdownloadoptions/#getImportUnderlineFormatting).

#### Exportar tablas como HTML al guardar en Markdown <sup>24.10</sup>

Se ha implementado una opción para exportar tablas como HTML al guardar documentos en formato Markdown agregando una nueva propiedad pública [ExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getExportAsHtml) y una enumeración [MarkdownExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownexportashtml/).

#### Exportar PDF con Estructura Lógica Actualizada <sup>24.11</sup>

La exportación PDF se ha mejorado al incluir las propiedades del título de la tabla como títulos de los elementos de la estructura lógica PDF.

### Mail Merge y Presentación de Informes

#### Eliminar Tablas vacías durante Mail Merge <sup>24.12</sup>

Se ha agregado una nueva opción **RemoveEmptyTables** a la enumeración [MailMergeCleanupOptions](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/) para refinar la salida Mail Merge.

### Firmas Digitales

#### Firme documentos con XAdES-EPES <sup>24.9</sup>

Se ha introducido la capacidad de firmar documentos con firmas XAdES-EPES de nivel XML-DSig agregando una nueva propiedad pública [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/signoptions/#getXmlDsigLevel) y una nueva enumeración pública [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/xmldsiglevel/)

### Otros

* Se ha agregado un nuevo método público [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-com.aspose.words.Shape...) a group shapes. <sup>24.9</sup>
* Se ha agregado un nuevo método público [InsertStructuredDocumentTag](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertStructuredDocumentTag-int) para insertar **StructuredDocumentTags** en un documento. <sup>24.9</sup>
* Se ha proporcionado acceso público a los separadores de notas al pie/notas al final agregando algunas clases y propiedades públicas. <sup>24.9</sup>
* La capacidad de agrupar formas individuales, group shapes juntas y agrupar directamente ambas formas y group shapes se ha introducido agregando el método [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-double-double-double-double-com.aspose.words.ShapeBase...). <sup>24.10</sup>
* Se ha mejorado el manejo de la codificación Big5 para TrueType tablas cmap. <sup>24.10</sup>
* Se ha mejorado la compatibilidad con fuentes taiwanesas obsoletas. <sup>24.10</sup>
* Para acceder a las propiedades extendidas del documento, se han agregado propiedades de solo lectura a la clase [BuiltInDocumentProperties](https://reference.aspose.com/words/java/com.aspose.words/builtindocumentproperties/). <sup>24.11</sup>
* Se ha habilitado la configuración de subtítulos para los controles ActiveX agregando un nuevo configurador público a la propiedad [Forms2OleControl.Caption](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/#getCaption). <sup>24.11</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por Java 24.9 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-9-release-notes/).

Más información sobre [Aspose.Words por Java 24.10 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-10-release-notes/).

Más información sobre [Aspose.Words por Java 24.11 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-11-release-notes/).

Más información sobre [Aspose.Words por Java 24.12 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words por Java 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 expande las opciones para ensamblados, mejora las capacidades de representación y expande algunas otras opciones.

Aspose.Words 24.6 mejora las opciones de representación, mejora la funcionalidad de búsqueda y comparación y amplía varias otras funciones.

Aspose.Words 24.7 cambia la forma de trabajar con ActiveX, amplía las capacidades de renderizado y exporta a formatos Markdown y XLSX.

Aspose.Words 24.8 mejora la personalización de los gráficos con un control preciso sobre las etiquetas de los ejes, amplía la administración de fuentes, mejora el manejo de la estructura de los documentos y agrega nuevas capacidades para la exportación HTML/XAML, la funcionalidad PDF, la conversión de documentos y las firmas digitales.

### Formatos Admitidos

A partir de la versión 24.7, se admite la exportación a PDF/UA-2 para garantizar la accesibilidad de los usuarios con discapacidades.

### Renderizado e Impresión

#### Cambios en Gráficos, Formas y DrawingML <sup>24.5</sup>

- Se ha implementado la representación de efectos DrawingML para gráficos SVG, ampliando la funcionalidad anterior limitada a imágenes.
- Se ha agregado compatibilidad para crear gráficos combinados y ajustar propiedades como el ancho del espacio, la superposición y la escala de burbujas dentro de los grupos de series agregando las clases [ChartSeriesGroup](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroup/) y [ChartSeriesGroupCollection](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroupcollection/) y la propiedad [SeriesGroups](https://reference.aspose.com/words/java/com.aspose.words/chart/#getSeriesGroups).
- La funcionalidad para manipular el efecto SoftEdge de las formas se ha implementado agregando la clase [SoftEdgeFormat](https://reference.aspose.com/words/java/com.aspose.words/softedgeformat/).
- La capacidad de modificar los valores adjust de las formas se ha implementado agregando las clases públicas [AdjustmentCollection](https://reference.aspose.com/words/java/com.aspose.words/adjustmentcollection/) y [Adjustment](https://reference.aspose.com/words/java/com.aspose.words/adjustment/) y la propiedad [Adjustments](https://reference.aspose.com/words/java/com.aspose.words/shape/#getAdjustments).

#### Cambios en Gráficos, Formas y Dibujos <sup>24.6</sup>

- Se han mejorado las capacidades de creación de gráficos. Ahora puede crear una variedad más amplia de gráficos, que incluyen *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* gráficos, *Box & Whisker* gráficos, *Waterfalls* y *Funnels*. Esto le permite visualizar sus datos de una manera más diversa e informativa.
- Se ha mejorado el control del color para el formato de las sombras. Puede obtener un control más preciso sobre la apariencia de sus documentos accediendo a los colores de las sombras.
- Se ha mejorado el aumento del rendimiento del renderizado en segundo plano. Puede acelerar significativamente la representación de fondos que contienen elementos pequeños gracias a la tecnología de mosaico nativa.
- Se han añadido degradados realistas para las formas. Ahora puede crear formas DML con degradados no lineales, imitando el estilo visual de Microsoft Word para una apariencia más pulida.

#### Personalización de Etiquetas de Datos de Gráficos <sup>24.7</sup>

Se ha agregado la capacidad de personalizar etiquetas de datos de gráficos como **Orientation** y **Rotation**.

#### Estilo de Número Personalizado para Niveles de Lista <sup>24.7</sup>

Se ha agregado un colocador para la propiedad pública [CustomNumberStyleFormat](https://reference.aspose.com/words/java/com.aspose.words/listlevel/#getCustomNumberStyleFormat). Ahora puede definir un estilo de número personalizado para los niveles de lista.

#### Cambios al trabajar con ActiveX <sup>24.7</sup>

* Las propiedades de los objetos ActiveX ahora se pueden modificar, lo que le brinda más control sobre su comportamiento.
* Se ha agregado la capacidad de modificar el valor del control del botón de opción ActiveX para habilitar la interacción dinámica.
* Se ha agregado la capacidad de alternar un ActiveX checkbox a "marcado" o "desmarcado".

#### Control Sobre la Orientación y Rotación de las Etiquetas de las Marcas de Verificación del Eje del Gráfico <sup>24.8</sup>

Se ha agregado un control preciso sobre la orientación y rotación de las etiquetas de marcas del eje del gráfico para una personalización más conveniente del gráfico: la clase [AxisTickLabels](https://reference.aspose.com/words/java/com.aspose.words/axisticklabels/) se ha ampliado con las nuevas propiedades **Orientation** y **Rotation**.

#### Reemplazando la Barra Invertida con el Signo del Yen <sup>24.8</sup>

Se ha mejorado la exportación HTML y XAML compatible con versiones anteriores para reemplazar el carácter de barra invertida con el signo Yen. Para lograr esto, se ha agregado la propiedad **ReplaceBackslashWithYenSign** a las clases [HtmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/) y [XamlFlowSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/).

#### Usar Etiquetas SDT como Nombres de Campo de Formulario al Exportar a PDF <sup>24.8</sup>

La exportación PDF con soporte para usar etiquetas SDT como nombres de campo de formulario se ha mejorado al agregar una nueva propiedad **UseSdtTagAsFormFieldName** a la clase [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/).

### Conversión, Carga y Guardado de Documentos

#### Exportación de enlaces al formato Markdown <sup>24.7</sup>

Se ha agregado la capacidad de controlar la exportación de enlaces en formato Markdown mediante la implementación de la propiedad [LinkExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getLinkExportMode).

#### LowCode 24.8 <sup>24.8</sup>

Se ha introducido una nueva clase **LowCode.Converter**, diseñada para proporcionar un conjunto de métodos para convertir varios tipos de documentos con una sola línea de código.

### Buscar y Comparar

#### Opciones Avanzadas de Comparación <sup>24.6</sup>

Se ha agregado la capacidad de agilizar los flujos de trabajo de análisis de datos con una funcionalidad de comparación mejorada. Esto incluye una nueva opción [IgnoreStoreItemId](https://reference.aspose.com/words/java/com.aspose.words/advancedcompareoptions/#getIgnoreStoreItemId) y una interfaz rediseñada para comparaciones avanzadas.

### Otros

* La función para eliminar páginas vacías de un documento se ha implementado agregando el método [RemoveBlankPages](https://reference.aspose.com/words/java/com.aspose.words/document/#removeBlankPages). <sup>24.5</sup>
* Se ha proporcionado la capacidad de verificar la presencia de VBA macros sin cargar un documento agregando la propiedad [HasMacros](https://reference.aspose.com/words/java/com.aspose.words/fileformatinfo/#hasMacros). <sup>24.5</sup>
* Ahora se admite mantener la numeración de origen al insertar un documento utilizando el Motor de informes LINQ. <sup>24.5</sup>
* Se ha agregado una nueva propiedad [DateTimeUtc](https://reference.aspose.com/words/java/com.aspose.words/comment/#getDateTimeUtc) que proporciona una marca de tiempo más precisa para los comentarios, mejorando la organización y la trazabilidad. <sup>24.6</sup>
* Se ha mejorado el motor de informes LINQ. Se ha realizado la eliminación selectiva de párrafos vacíos y la definición de mensajes personalizados para miembros de objetos faltantes, lo que lleva a informes más limpios e informativos. <sup>24.6</sup>
* El formato de fecha y hora ahora se detecta automáticamente para una exportación perfecta al formato XLSX. <sup>24.7</sup>
* Se ha agregado la propiedad pública [IsProtected](https://reference.aspose.com/words/java/com.aspose.words/vbaproject/#isProtected), que le permite verificar si un proyecto VBA está protegido. <sup>24.7</sup>
* La información de la fuente se ha ampliado con la propiedad **EmbeddingLicensingRights** agregada a las clases [FontInfo](https://reference.aspose.com/words/java/com.aspose.words/fontinfo/) y [PhysicalFontInfo](https://reference.aspose.com/words/java/com.aspose.words/physicalfontinfo/). <sup>24.8</sup>
* Se ha agregado una forma de borrar de manera eficiente los encabezados y pies de página de las secciones al tiempo que se conservan las marcas de agua para trabajar con mayor precisión con la estructura del documento. Para borrar los encabezados y pies de página de las secciones, use el nuevo método public **ClearHeadersFooters**. <sup>24.8</sup>
* Se ha habilitado la firma digital de XPS documentos usando [XpsSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xpssaveoptions/); se ha agregado una nueva propiedad **DigitalSignatureDetails** para este propósito. <sup>24.8</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por Java 24.5 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-5-release-notes/).

Más información sobre [Aspose.Words por Java 24.6 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-6-release-notes/).

Más información sobre [Aspose.Words por Java 24.7 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-7-release-notes/).

Más información sobre [Aspose.Words por Java 24.8 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words por Java 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 mejora la experiencia en torno a la administración de los colores de los trazos, mejora los objetos OLE y los informes LINQ, así como presenta una nueva Fuente de Bibliografía pública API.

Aspose.Words 24.2 gráficos expandidos API, gestión de estilos y LINQ opciones. Esta versión de Aspose.Words también introdujo la capacidad de especificar SvgSaveOptions durante el procesamiento, un control más flexible para cargar archivos Markdown y trabajar con texto de referencia para notas al pie y notas al final.

Aspose.Words 24.3 introduce un nuevo Lector/escritor TIFF y emulación de operaciones ráster binarias para metarchivos WMF. Aspose.Words 24.3 también continúa expandiendo los Gráficos API.

Aspose.Words 24.4 mejora los formatos de guardado, algunas opciones de renderizado y mejora el trabajo con firmas digitales.

### Formatos Admitidos <sup>24.4</sup>

El formato de imagen **WebP** moderno ahora es compatible con Aspose.Words. Ahora puede leer e insertar imágenes WebP en documentos, así como guardar imágenes en formato WebP.

### Renderizado e Impresión

#### Control de Color de Trazo <sup>24.1</sup>

La clase [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) se ha ampliado con un conjunto de nuevas propiedades públicas relacionadas con la administración de los colores de trazo: [ForeThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeThemeColor) y [BackThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackThemeColor), [ForeTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeTintAndShade) y [BackTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackTintAndShade).

#### Extensión DrawingML Gráficos API <sup>24.2 / 24.3 / 24.4</sup>

El **DrawingML Charts API** continúa expandiéndose.

#### Incrustar fuentes Declaradas en @font-face Reglas <sup>24.4</sup>

Se agregó la capacidad de incrustar fuentes declaradas en las reglas @font-face en las definiciones de fuentes del documento resultante agregando una nueva propiedad [SupportFontFaceRules](https://reference.aspose.com/words/java/com.aspose.words/htmlloadoptions/#getSupportFontFaceRules).

#### Trabajar con Formato de Resplandor y Reflejo <sup>24.4</sup>

Se ha implementado la capacidad de trabajar con formato de resplandor y reflejo para un objeto de dibujo.

### Cargar y Guardar Documentos

#### Especifique SvgSaveOptions Durante el Procesamiento <sup>24.2</sup>

La capacidad de especificar [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/) durante el renderizado se ha agregado usando [ShapeRenderer](https://reference.aspose.com/words/java/com.aspose.words/shaperenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) y [OfficeMathRenderer](https://reference.aspose.com/words/java/com.aspose.words/officemathrenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) métodos.

#### Conservar las Líneas Vacías al Cargar Markdown archivos <sup>24.2</sup>

Se ha agregado la capacidad de conservar líneas vacías al cargar archivos Markdown.

#### Un Nuevo TIFF Lector / Escritor <sup>24.3</sup>

Se ha desarrollado un nuevo lector/escritor TIFF para Aspose.Words para .NET Standard, .NET 6 y posteriores. Aspose.Words por .NET 24.3 se agregó soporte para leer TIFF imágenes con JPEG y tipos de compresión JPEG antiguos, y también se mejoró significativamente la calidad de las operaciones de lectura y escritura.

### Otros

* Se ha introducido la capacidad de modificar el texto del control `TextBox` OLE agregando una nueva propiedad [Text](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/#getText) a la nueva clase [TextBoxControl](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/). 24.1 <sup>24.1</sup>
* Las Fuentes Bibliográficas públicas API se implementaron agregando algunas nuevas [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/bibliography/), [Source](https://reference.aspose.com/words/java/com.aspose.words/source/), [ContributorCollection](https://reference.aspose.com/words/java/com.aspose.words/contributorcollection/), [Contributor](https://reference.aspose.com/words/java/com.aspose.words/contributor/), [Corporate](https://reference.aspose.com/words/java/com.aspose.words/corporate/), [PersonCollection](https://reference.aspose.com/words/java/com.aspose.words/personcollection/) y [Person](https://reference.aspose.com/words/java/com.aspose.words/person/) clases y una enumeración [SourceType](https://reference.aspose.com/words/java/com.aspose.words/sourcetype/), así como agregando una nueva propiedad [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/document/#getBibliography) a la clase [Document](https://reference.aspose.com/words/java/com.aspose.words/document/). <sup>24.1</sup>
* Se ha proporcionado un API para limitar el acceso a los miembros de tipo utilizando la sintaxis de plantilla para el Motor de informes LINQ. <sup>24.1</sup>
* Se han agregado nuevas propiedades públicas [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) y [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) para una mejor administración de estilos a la clase [Style](https://reference.aspose.com/words/net/aspose.words/style/). <sup>24.2</sup>
* La funcionalidad para recuperar el texto real de la marca de referencia para notas al pie y notas al final se ha mejorado con la propiedad [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) y el método [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* Se ha habilitado la compatibilidad con los gráficos `Word 2016` para `LINQ Reporting Engine`. <sup>24.2</sup>
* Se ha implementado la emulación de operaciones ráster binarias para metarchivos WMF. <sup>24.3</sup>
* La capacidad de definir opciones de firma para documentos dentro de **SaveOptions** se ha habilitado agregando una nueva clase [DigitalSignatureDetails](https://reference.aspose.com/words/java/com.aspose.words/digitalsignaturedetails/) con nuevos miembros públicos, así como agregando nuevas propiedades a las clases [OoxmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/docsaveoptions/) y [OdtSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por Java 24.1 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-1-release-notes/).

Más información sobre [Aspose.Words por Java 24.2 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-2-release-notes/).

Más información sobre [Aspose.Words por Java 24.3 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-3-release-notes/).

Más información sobre [Aspose.Words por Java 24.4 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words por Java 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 expande las opciones de representación, la emulación de representación de metarchivo y las opciones de guardado markdown.

Aspose.Words 23.10 mejora el renderizado, amplía las opciones para cargar y guardar documentos y permite a los usuarios fusionar documentos de nuevas formas.

Aspose.Words 23.11 mejora el trabajo con revisiones, formato XLSX y fuentes en la leyenda del gráfico con opciones adicionales.

Aspose.Words 23.12 presenta nuevas propiedades y enumeraciones para trabajar con documentos PDF, compatibilidad con imágenes WebP y biblioteca actualizada de castillos hinchables.

### Renderizado e Impresión

#### Personalización de Títulos de Ejes en Gráficos DrawingML <sup>23.9</sup>

La capacidad de personalizar los títulos de los ejes en los gráficos DrawingML se ha introducido mediante la implementación de una nueva propiedad pública de clase [ChartAxisTitle](https://reference.aspose.com/words/java/com.aspose.words/chartaxistitle/) y [Title](https://reference.aspose.com/words/java/com.aspose.words/chartaxis/#getTitle).

#### Determinar la Posición Vertical de las Fuentes dentro de un Párrafo <sup>23.9</sup>

Ahora es posible definir la posición vertical de las fuentes dentro de un párrafo utilizando la nueva propiedad public [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getBaselineAlignment) y la nueva enumeración [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/baselinealignment/).

#### Control de Color de Primer Plano <sup>23.10</sup>

La capacidad de recuperar el color de primer plano sin modificadores se ha agregado a las clases [Fill](https://reference.aspose.com/words/java/com.aspose.words/fill/) y [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) a través de la propiedad **BaseForeColor**.

#### Ampliación de la Funcionalidad de los Gráficos <sup>23.10</sup>

La funcionalidad de las clases [ChartDataPointCollection](https://reference.aspose.com/words/java/com.aspose.words/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/java/com.aspose.words/chartseries/) y [ChartFormat](https://reference.aspose.com/words/java/com.aspose.words/chartformat/) se ha ampliado con nuevos métodos y propiedades.

#### Ajusta y ajusta Automáticamente una Imagen en una Forma <sup>23.10</sup>

Se ha proporcionado una forma sencilla de ajustar y ajustar automáticamente una imagen dentro de una forma particular a través del nuevo método [FitImageToShape](https://reference.aspose.com/words/java/com.aspose.words/imagedata/#fitImageToShape).

#### Formato de fuente Predeterminado para las Entradas de Leyenda de Gráfico DrawingML <sup>23.11</sup>

Se ha agregado la capacidad de especificar el formato de fuente predeterminado para las entradas de leyenda de los gráficos DrawingML a través de la propiedad **Font**. Esta característica facilita una apariencia más optimizada y consistente para los elementos del gráfico, mejorando la estética general del documento.

#### Especifique el Diseño de página al Abrir PDF en Reader <sup>23.12</sup>

Se ha agregado la capacidad de especificar el diseño de página que se utilizará al abrir un documento en un lector PDF mediante la introducción de una nueva propiedad [PageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getPageLayout) en la clase [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/) y la introducción de una nueva enumeración [PdfPageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfpagelayout/).

### Cargar y Guardar Documentos

#### Especificar un Nombre de Carpeta para Construir la Imagen URIs en Markdown <sup>23.9</sup>

La clase [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) se ha ampliado al incluir la propiedad [ImagesFolderAlias](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImagesFolderAlias), que permite especificar el nombre de la carpeta utilizada para construir la imagen URIs escrita en el documento Markdown.

#### Reducir el Tamaño de Salida PDF <sup>23.10</sup>

Se han implementado varias optimizaciones de renderizado PDF para reducir el tamaño de salida al utilizar la configuración [OptimizeOutput](https://reference.aspose.com/words/java/com.aspose.words/fixedpagesaveoptions/#getOptimizeOutput).

#### Reconocer Hipervínculos al Cargar Documentos TXT <sup>23.10</sup>

La función para reconocer hipervínculos al cargar documentos TXT se ha implementado agregando una nueva propiedad [DetectHyperlinks](https://reference.aspose.com/words/java/com.aspose.words/txtloadoptions/#getDetectHyperlinks).

### Otros

- Se ha implementado la emulación de representación de metarchivo para determinar el tamaño de rasterización, específicamente para el ancho del lápiz WMF y el ancho del lápiz cosmético EMF. Para lograr esto, la propiedad **ScaleWmfFontsToMetafileSize** se reemplazó con la propiedad [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPage) y se agregó la propiedad [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPageResolution). <sup>23.9</sup>
- Se ha introducido un método simplificado para insertar un documento en otro documento en la posición actual del cursor utilizando el método [InsertDocumentInline](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertDocumentInline-com.aspose.words.Document-int-com.aspose.words.ImportFormatOptions). <sup>23.10</sup>
- La capacidad de acceder y modificar propiedades de estilo se ha agregado mediante la introducción de la nueva propiedad [Locked](https://reference.aspose.com/words/java/com.aspose.words/style/#getLocked). <sup>23.10</sup>
- Se ha agregado un parámetro de tipo genérico a los métodos de la clase [CompositeNode](https://reference.aspose.com/words/java/com.aspose.words/compositenode/). <sup>23.10</sup>
- Se ha implementado una forma de controlar cuándo se debe aceptar/rechazar o no una determinada revisión utilizando los métodos [Accept](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#accept-com.aspose.words.IRevisionCriteria) y [Reject](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#reject-com.aspose.words.IRevisionCriteria). Esta mejora otorga a los usuarios un control más preciso sobre el proceso de revisión. <sup>23.11</sup>
- La capacidad de escribir todas las secciones de un documento en la misma hoja de cálculo XLSX se ha proporcionado a través del nuevo tipo de enumeración [XlsxSectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsectionmode/) y la nueva propiedad [SectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/#getSectionMode). <sup>23.11</sup>
- Se ha introducido soporte para la imagen WebP. Tenga en cuenta que esta función solo está disponible para .versiones NetStandart y .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por Java 23.9 Notas de la versión](/words/java/aspose-words-for-java-23-9-release-notes/).

Más información sobre [Aspose.Words por Java 23.10 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-10-release-notes/).

Más información sobre [Aspose.Words por Java 23.11 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-11-release-notes/).

Más información sobre [Aspose.Words por Java 23.12 Notas de la versión](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-12-release-notes/).

{{% /alert %}}

## Véase También

{{% alert color="primary" %}}

Esta página contiene las últimas noticias de lanzamiento de los últimos 2 años. Para obtener detalles sobre versiones anteriores, consulte [Notas de la versión'](https://releases.aspose.com/words/java/release-notes/) páginas en las secciones relevantes.

{{% /alert %}}
