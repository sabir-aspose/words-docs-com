---
title: Qué hay de nuevo
second_title: Aspose.Words por Python via .NET
articleTitle: Qué hay de nuevo en Aspose.Words por Python via .NET
linktitle: Qué hay de nuevo en Aspose.Words por Python via .NET
type: docs
description: "Aspose.Words por Python via .NET se expande y mejora a diario. En esta página, puede conocer las características enormes y más interesantes del producto."
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /es/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-06-23-21-02-49
---

Esta página describe las nuevas funciones Aspose.Words más interesantes introducidas en versiones recientes.

## Aspose.Words por Python via .NET 25.5, 25.6

Aspose.Words 25.5 mejora la personalización de los gráficos con nuevas opciones de estilo y mejora la exportación de Markdown al ofrecer control sobre cómo se manejan los párrafos vacíos.

Aspose.Words 25.6 mejora la precisión de representación y las funciones de visualización al introducir opciones avanzadas de exportación de imágenes, manejo mejorado de MathML y mejor representación de gráficos.

### Conversión, Carga y Guardado de Documentos

#### Exportar Párrafos vacíos a Markdown <sup>25.5</sup>

Se ha introducido la capacidad de controlar cómo se exportan los párrafos vacíos a Markdown agregando la enumeración **MarkdownEmptyParagraphExportMode** y la propiedad **empty_paragraph_export_mode**.

#### Exporte Documentos de Varias páginas a Formatos de Imagen Rasterizada <sup>25.6</sup>

Se ha introducido la capacidad de exportar documentos de varias páginas a formatos de imagen ráster (como PNG y JPEG) con [customizable layouts](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/) (Horizontal, Vertical o Cuadrícula) al ampliar la funcionalidad de exportación de imágenes.

### Renderizado

#### Configuración del Estilo del Gráfico <sup>25.5</sup>

La capacidad de establecer el estilo del gráfico se ha introducido agregando la enumeración **ChartStyle** y la propiedad **style**.

#### Representación de Líneas de Conector en MathML Expresiones <sup>25.6</sup>

La representación de líneas de conexión en expresiones MathML se ha implementado para garantizar una visualización más precisa y visualmente coherente de las fórmulas matemáticas.

#### Leyendas de Renderizado para Gráficos en Cascada <sup>25.6</sup>

Se ha introducido la representación de leyendas para ["Waterfall" charts](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriestype/), lo que aumenta la transparencia de los datos y mejora la interpretabilidad de estos gráficos.

### Otros

* Se ha mejorado la capacidad de ajustar fórmulas matemáticas que contienen varias barras inclinadas, mejorando la claridad del diseño y la legibilidad de la fórmula. <sup>25.6</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words para Python via .NET 25.5 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-5-release-notes/).

Más información sobre [Aspose.Words para Python via .NET 25.6 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words para Python a través de .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 presenta la revisión gramatical impulsada por AI y mejora el guardado de documentos con opciones avanzadas para los formatos HTML, SVG y Markdown.

Aspose.Words 25.2 introduce el resumen de texto con los modelos Anthropic AI, agrega compatibilidad con el formato MsWorks, mejora el control tipográfico y mejora la estructura PDF y el manejo de listas.

Aspose.Words 25.3 mejora un corrector gramatical con tecnología AI y la selección de fuentes con la propiedad UpdateAmbiguousTextFont, además de mejorar la exportación de archivos adjuntos PDF.

Aspose.Words 25.4 introduce compatibilidad con nuevos tamaños de papel, habilita el control avanzado de exportación de HTML y mejora el manejo de marcas de agua.

### AI - funciones potenciadas

#### Documento AI Revisión gramatical

* La capacidad de verificar la gramática del documento proporcionado utilizando OpenAI modelos generativos se ha introducido agregando un nuevo método [check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/). <sup>25.1</sup>
* La función de revisión gramatical impulsada por AI se ha actualizado para admitir todos los modelos disponibles en la enumeración [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Resumen Usando Anthropic Modelos de Lenguaje Generativo <sup>25.2</sup>

Se ha habilitado la síntesis de texto utilizando Anthropic modelos de lenguaje generativo al introducir una nueva clase pública [AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/).

### Formatos Admitidos <sup>25.2</sup>

A partir de la versión 25.2, se ha agregado compatibilidad con el nuevo formato de carga MsWorks para documentos Microsoft Works.

### Conversión, Carga y Guardado de Documentos

#### Guardado mejorado en formatos HTML y SVG <sup>25.1</sup>

Se ha mejorado el guardado en formatos HTML y SVG agregando propiedades **id_prefix** y **remove_java_script_from_links** a las clases [HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/) y [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/).

#### Establezca la Resolución de la Imagen y el Modo de salida OfficeMath Al Guardar en Markdown <sup>25.1</sup>

* Se ha agregado una nueva opción [image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/) a la clase [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) para establecer la resolución de la imagen.
* Se han agregado una nueva opción [office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/) y enumeración [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/) a la clase [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) para establecer el modo de salida OfficeMath.

### Renderizado

#### Control Tipográfico Mejorado <sup>25.2</sup>

Se ha agregado la propiedad [number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/) para mejorar el control tipográfico.

#### Control de la Selección de Fuentes para Caracteres Ambiguos <sup>25.3</sup>

Se ha agregado una nueva propiedad pública [update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/) a la clase [SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/) para controlar la selección de fuentes de acuerdo con el código de caracteres utilizado.

#### Opciones de Tamaño de Papel <sup>25.4</sup>

Se ha introducido la capacidad de usar tamaños de papel JIS B4 y JIS B5 agregando nuevos valores a la enumeración [PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/).

#### HTML Control de Salida <sup>25.4</sup>

Se ha introducido la capacidad de eliminar JavaScript del hipervínculo URLs durante la exportación de HTML agregando la propiedad [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/).

### Otros

* La estructura lógica de PDF se ha mejorado con la compatibilidad con los campos TOA, BIBLIOGRAPHY y INDEX. <sup>25.2</sup>
* El método [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate) se ha introducido para mejorar el manejo de listas. <sup>25.2</sup>
* Se ha agregado una nueva propiedad [attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/) para reemplazar **EmbedAttachments** y mejorar la exportación de PDF archivos adjuntos. Además, se han agregado nuevos valores a la enumeración [PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/) para admitir archivos adjuntos de la versión PDF/A. Además, los archivos adjuntos ahora son compatibles con el cifrado. <sup>25.3</sup>
* La capacidad de establecer una marca de agua de imagen a partir de una secuencia se ha introducido agregando una nueva sobrecarga al método [SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions). <sup>25.4</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por Python via .NET 25.1 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 25.2 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 25.3 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 25.4 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words para Python a través de .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduce la inserción group shape y la inserción StructuredDocumentTag a través de DocumentBuilder, mejora la representación de gráficos radiales con graduaciones, mejora las firmas digitales con compatibilidad con XAdES-EPES, agrega reconocimiento de subrayado Markdown y proporciona acceso a separadores de notas al pie/notas al final.

Aspose.Words 24.10 presenta compatibilidad mejorada con el control ActiveX con la creación de CommandButton, nuevo control de visibilidad de formas, la capacidad de group shapes, exportación mejorada de Markdown para tablas, formato de gráficos para Pie y Doughnut, mejor manejo de codificación Big5 y compatibilidad con fuentes taiwanesas obsoletas.

Aspose.Words 24.11 presenta un resumen de documentos impulsado por AI, opciones de representación mejoradas, acceso mejorado a las propiedades del documento y subtítulos de control ActiveX.

Aspose.Words 24.12 presenta la colocación personalizable de etiquetas de datos, la traducción de texto impulsada por Google AI y las nuevas clases mejoradas de procesamiento de LowCode.

### AI - funciones potenciadas

#### Resumen de documentos Usando OpenAI y Google <sup>24.11</sup>

Se ha integrado la compatibilidad con el resumen de documentos mediante los modelos de lenguaje generativo **OpenAI** y **Google** agregando el espacio de nombres [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) con sus miembros públicos.

#### Traducción de texto utilizando los modelos de lenguaje generativo de Google <sup>24.12</sup>

La capacidad de traducir texto utilizando los modelos de lenguaje generativo de Google se implementó en Aspose.Words al agregar el método [translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/) y la enumeración [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) al espacio de nombres [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Nuevas LowCode clases como [Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) etc. se ha introducido un conjunto de métodos que logran el equilibrio perfecto entre simplicidad y flexibilidad para el procesamiento de documentos.

### Renderizado e Impresión

#### Graduaciones en Gráficos Radiales <sup>24.9</sup>

Se ha implementado la representación de graduaciones en gráficos radiales.

#### CommandButton ActiveX Controles <sup>24.10</sup>

La capacidad de crear controles CommandButton ActiveX se ha introducido agregando un nuevo método público [insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/) y una nueva clase pública [Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/).

#### Controlar la Visibilidad de la Forma <sup>24.10</sup>

Se ha agregado una nueva propiedad pública [hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/) para controlar la visibilidad de las formas.

#### Cambios en los gráficos Pie y Doughnut <sup>24.10</sup>

Se han agregado varias propiedades públicas nuevas a los gráficos de formato Pie y Doughnut.

#### Controle la representación de los Bordes de los Campos del Formulario de Elección PDF <sup>24.11</sup>

Se ha implementado una nueva opción para controlar la representación de los bordes de los campos de formulario de elección PDF agregando una nueva opción pública [render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/).

#### Obtenga y Configure Códigos de Formato para Datos de Gráficos <sup>24.11</sup>

Se ha agregado la capacidad de obtener y establecer códigos de formato para datos de gráficos implementando la propiedad [format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/) en las clases [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/) y [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/).

#### Renderice Gráficos de Histogramas con Contenedores y Etiquetas <sup>24.11</sup>

La representación del gráfico de histogramas se ha mejorado al permitir un número específico de contenedores y etiquetas.

#### Personalice la Ubicación de las Etiquetas de Datos <sup>24.12</sup>

Se ha agregado la capacidad de personalizar la ubicación de las etiquetas de datos al introducir nuevas propiedades en las clases [ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/) y [ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Conversión, Carga y Guardado de Documentos

#### Subrayar el formato al Cargar Markdown Archivos <sup>24.9</sup>

Se ha incorporado la opción de reconocer el formato subrayado al cargar documentos Markdown agregando una nueva propiedad pública [import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/).

#### Exportar tablas como HTML al guardar en Markdown <sup>24.10</sup>

Se ha implementado una opción para exportar tablas como HTML al guardar documentos en formato Markdown agregando una nueva propiedad pública [export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/) y una enumeración [MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/).

#### Exportar PDF con Estructura Lógica Actualizada <sup>24.11</sup>

La exportación PDF se ha mejorado al incluir las propiedades del título de la tabla como títulos de los elementos de la estructura lógica PDF.

### Firmas Digitales

#### Firme documentos con XAdES-EPES <sup>24.9</sup>

Se ha introducido la capacidad de firmar documentos con firmas XAdES-EPES de nivel XML-DSig agregando una nueva propiedad pública [xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/) y una nueva enumeración pública [XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/).

### Otros

* Se ha agregado un nuevo método público [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/) a group shapes. <sup>24.9</sup>
* Se ha agregado un nuevo método público [insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/) para insertar **StructuredDocumentTags** en un documento. <sup>24.9</sup>
* Se ha proporcionado acceso público a los separadores de notas al pie/notas al final agregando algunas clases y propiedades públicas. <sup>24.9</sup>
* La capacidad de agrupar formas individuales, group shapes juntas y agrupar directamente ambas formas y group shapes se ha introducido agregando el método [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist). <sup>24.10</sup>
* Se ha mejorado el manejo de la codificación Big5 para TrueType tablas cmap. <sup>24.10</sup>
* Se ha mejorado la compatibilidad con fuentes taiwanesas obsoletas. <sup>24.10</sup>
* Para acceder a las propiedades extendidas del documento, se han agregado propiedades de solo lectura a la clase [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/). <sup>24.11</sup>
* Se ha habilitado la configuración de subtítulos para los controles ActiveX agregando un nuevo configurador público a la propiedad [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por Python via .NET 24.9 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 24.10 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 24.11 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 24.12 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words para Python a través de .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 expande las opciones para ensamblados, mejora las capacidades de representación y expande algunas otras opciones.

Aspose.Words 24.6 mejora las opciones de representación, mejora la funcionalidad de búsqueda y comparación y amplía varias otras funciones.

Aspose.Words 24.7 cambia la forma de trabajar con ActiveX, amplía las capacidades de renderizado y exporta a formatos Markdown y XLSX.

Aspose.Words 24.8 mejora la personalización de los gráficos con un control preciso sobre las etiquetas de los ejes, amplía la administración de fuentes, mejora el manejo de la estructura de los documentos y agrega nuevas capacidades para la exportación HTML/XAML, la funcionalidad PDF, la conversión de documentos y las firmas digitales.

### Formatos Admitidos

A partir de la versión 24.7, se admite la exportación a PDF/UA-2 para garantizar la accesibilidad de los usuarios con discapacidades.

### Renderizado e Impresión

#### Cambios en Gráficos, Formas y DrawingML <sup>24.5</sup>

* Se ha implementado la representación de efectos DrawingML para gráficos SVG, ampliando la funcionalidad anterior limitada a imágenes.
* Se ha agregado compatibilidad para crear gráficos combinados y ajustar propiedades como el ancho del espacio, la superposición y la escala de burbujas dentro de los grupos de series agregando las clases [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/) y [ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/) y la propiedad [series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/).
* La funcionalidad para manipular el efecto SoftEdge de las formas se ha implementado agregando la clase [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/).
* La capacidad de modificar los valores adjust de las formas se ha implementado agregando las clases públicas **AdjustmentCollection** y **Adjustment** y la propiedad [adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/).

#### Cambios en Gráficos, Formas y Dibujos <sup>24.6</sup>

- Se han mejorado las capacidades de creación de gráficos. Ahora puede crear una variedad más amplia de gráficos, que incluyen *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* gráficos, *Box & Whisker* gráficos, *Waterfalls* y *Funnels*. Esto le permite visualizar sus datos de una manera más diversa e informativa.
- Se ha mejorado el control del color para el formato de las sombras. Puede obtener un control más preciso sobre la apariencia de sus documentos accediendo a los colores de las sombras.
- Se ha mejorado el aumento del rendimiento del renderizado en segundo plano. Puede acelerar significativamente la representación de fondos que contienen elementos pequeños gracias a la tecnología de mosaico nativa.
- Se han añadido degradados realistas para las formas. Ahora puede crear formas DML con degradados no lineales, imitando el estilo visual de Microsoft Word para una apariencia más pulida.

#### Personalización de Etiquetas de Datos de Gráficos <sup>24.7</sup>

Se ha agregado la capacidad de personalizar etiquetas de datos de gráficos como **Orientation** y **Rotation**.

#### Estilo de Número Personalizado para Niveles de Lista <sup>24.7</sup>

Se ha agregado un colocador para la propiedad pública [custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/). Ahora puede definir un estilo de número personalizado para los niveles de lista.

#### Cambios al trabajar con ActiveX <sup>24.7</sup>

- Las propiedades de los objetos ActiveX ahora se pueden modificar, lo que le brinda más control sobre su comportamiento.
- Se ha agregado la capacidad de modificar el valor del control del botón de opción ActiveX para habilitar la interacción dinámica.
- Se ha agregado la capacidad de alternar un ActiveX checkbox a "marcado" o "desmarcado".

#### Control Sobre la Orientación y Rotación de las Etiquetas de las Marcas de Verificación del Eje del Gráfico <sup>24.8</sup>

Se ha agregado un control preciso sobre la orientación y rotación de las etiquetas de marcas del eje del gráfico para una personalización más conveniente del gráfico: la clase [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) se ha ampliado con las nuevas propiedades [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) y [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/).

#### Reemplazando la Barra Invertida con el Signo del Yen <sup>24.8</sup>

Se ha mejorado la exportación HTML y XAML compatible con versiones anteriores para reemplazar el carácter de barra invertida con el signo Yen. Para lograr esto, se ha agregado la propiedad **replace_backslash_with_yen_sign** a las clases [HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/) y [XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/).

#### Usar Etiquetas SDT como Nombres de Campo de Formulario al Exportar a PDF <sup>24.8</sup>

La exportación PDF con soporte para usar etiquetas SDT como nombres de campo de formulario se ha mejorado al agregar una nueva propiedad [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) a la clase [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/).

### Conversión, Carga y Guardado de Documentos

#### Exportación de enlaces al formato Markdown <sup>24.7</sup>

Se ha agregado la capacidad de controlar la exportación de enlaces en formato Markdown mediante la implementación de la propiedad [link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/).

#### LowCode 24.8 <sup>24.8</sup>

Se ha introducido una nueva clase [LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/), diseñada para proporcionar un conjunto de métodos para convertir varios tipos de documentos con una sola línea de código.

### Buscar y Comparar

#### Opciones Avanzadas de Comparación <sup>24.6</sup>

Se ha agregado la capacidad de agilizar los flujos de trabajo de análisis de datos con una funcionalidad de comparación mejorada. Esto incluye una nueva opción [ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/) y una interfaz rediseñada para comparaciones avanzadas.

### Otros

* La función para eliminar páginas vacías de un documento se ha implementado agregando el método [remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/). <sup>24.5</sup>
* Se ha proporcionado la capacidad de verificar la presencia de VBA macros sin cargar un documento agregando la propiedad [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/). <sup>24.5</sup>
* Ahora se admite mantener la numeración de origen al insertar un documento utilizando el Motor de informes LINQ. <sup>24.5</sup>
* Se ha agregado una nueva propiedad [date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/) que proporciona una marca de tiempo más precisa para los comentarios, mejorando la organización y la trazabilidad. <sup>24.6</sup>
* El formato de fecha y hora ahora se detecta automáticamente para una exportación perfecta al formato XLSX. <sup>24.7</sup>
* Se ha agregado la propiedad pública [is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/), que le permite verificar si un proyecto VBA está protegido. <sup>24.7</sup>
* La información de la fuente se ha ampliado con la propiedad **embedding_licensing_rights** agregada a las clases [FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/) y [PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* Se ha agregado una forma de borrar de manera eficiente los encabezados y pies de página de las secciones al tiempo que se conservan las marcas de agua para trabajar con mayor precisión con la estructura del documento. Para borrar los encabezados y pies de página de las secciones, use el nuevo método public [clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default). <sup>24.8</sup>
* Se ha habilitado la firma digital de XPS documentos usando [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/); se ha agregado una nueva propiedad [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/) para este propósito. <sup>24.8</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por Python via .NET 24.5 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 24.6 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 24.7 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 24.8 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words para Python a través de .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 mejora la experiencia en torno a la administración de los colores de trazo, mejora los objetos OLE e introduce un nuevo `Bibliography Sources` público API.

Aspose.Words 24.2 gráficos expandidos API y gestión de estilos. Esta versión de Aspose.Words también introdujo la capacidad de especificar SvgSaveOptions durante el procesamiento, un control más flexible para cargar archivos Markdown y trabajar con texto de referencia para notas al pie y notas al final.

Aspose.Words 24.3 introduce un nuevo Lector/escritor TIFF y emulación de operaciones ráster binarias para metarchivos WMF. Aspose.Words 24.3 también continúa expandiendo los Gráficos API.

Aspose.Words 24.4 mejora los formatos de guardado, algunas opciones de renderizado y mejora el trabajo con firmas digitales.

### Formatos Admitidos <sup>24.4</sup>

El formato de imagen **WebP** moderno ahora es compatible con Aspose.Words por .NET Framework 4.6.2 y más alto. Ahora puede leer e insertar imágenes WebP en documentos, así como guardar imágenes en formato WebP.

Tenga en cuenta que WebP actualmente solo está disponible en .NET Standard y .NET Framework contra4.6.2 y superiores.

### Renderizado e Impresión

#### Control de Color de Trazo <sup>24.1</sup>

La clase [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) se ha ampliado con un conjunto de nuevas propiedades públicas relacionadas con la administración de los colores de trazo: [fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/) y [back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/), [fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/) y [back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### Extensión DrawingML Gráficos API <sup>24.2 / 24.3 / 24.4</sup>

El **DrawingML Charts API** continúa expandiéndose.

#### Incrustar fuentes Declaradas en @font-face Reglas <sup>24.4</sup>

Se agregó la capacidad de incrustar fuentes declaradas en las reglas @font-face en las definiciones de fuentes del documento resultante agregando una nueva propiedad [support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/).

#### Trabajar con Formato de Resplandor y Reflejo <sup>24.4</sup>

Se ha implementado la capacidad de trabajar con formato de resplandor y reflejo para un objeto de dibujo.

### Cargar y Guardar Documentos

#### Especifique SvgSaveOptions Durante el Procesamiento <sup>24.2</sup>

La capacidad de especificar [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) durante el renderizado se ha agregado usando [ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) y [OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) métodos.

#### Conservar las Líneas Vacías al Cargar Markdown archivos <sup>24.2</sup>

Se ha agregado la capacidad de conservar líneas vacías al cargar archivos Markdown.

#### Un Nuevo TIFF Lector / Escritor <sup>24.3</sup>

Se ha desarrollado un nuevo lector/escritor TIFF para Aspose.Words. Aspose.Words por .NET 24.3 se agregó soporte para leer imágenes TIFF con JPEG y tipos de compresión JPEG antiguos, y también se mejoró significativamente la calidad de las operaciones de lectura y escritura.

### Otros

* Se ha introducido la capacidad de modificar el texto del control `TextBox` OLE agregando una nueva propiedad **Text** a la nueva clase **TextBoxControl**. <sup>24.1</sup>
* Las Fuentes de Bibliografía public API se implementaron agregando un nuevo espacio de nombres [Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/) con sus nuevas clases y enumeraciones, y agregando una nueva propiedad [bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/) a la clase [Document](https://reference.aspose.com/words/python-net/aspose.words/document/). <sup>24.1</sup>
* Se han agregado nuevas propiedades públicas [priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/), [unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/) y [semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/) para una mejor administración de estilos a la clase [Style](https://reference.aspose.com/words/python-net/aspose.words/style/). <sup>24.2</sup>
* La funcionalidad para recuperar el texto real de la marca de referencia para notas al pie y notas al final se ha mejorado con la propiedad [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/) y el método [update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default). <sup>24.2</sup>
* Se ha implementado la emulación de operaciones ráster binarias para metarchivos WMF. <sup>24.3</sup>
* La capacidad de definir opciones de firma para documentos dentro de **SaveOptions** se ha habilitado agregando una nueva clase [DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/) con nuevos miembros públicos, así como agregando nuevas propiedades a las clases [OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/) y [OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por Python via .NET 24.1 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 24.2 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 24.3 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 24.4 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words para Python a través de .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 expande las opciones de representación, la emulación de representación de metarchivo y las opciones de guardado markdown.

Aspose.Words 23.10 mejora el renderizado, amplía las opciones para cargar y guardar documentos y permite a los usuarios fusionar documentos de nuevas formas.

Aspose.Words 23.11 mejora el trabajo con revisiones, formato XLSX y fuentes en la leyenda del gráfico con opciones adicionales.

Aspose.Words 23.12 introduce nuevas propiedades y enumeraciones para trabajar con documentos PDF y OOXML, así como compatibilidad con imágenes WebP.

### Renderizado e Impresión

#### Personalización de Títulos de Ejes en Gráficos DrawingML <sup>23.9</sup>

La capacidad de personalizar los títulos de los ejes en los gráficos DrawingML se ha introducido mediante la implementación de una nueva propiedad pública de clase [ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/) y [title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/).

####  Determinar la Posición Vertical de las Fuentes dentro de un Párrafo <sup>23.9</sup>

Ahora es posible definir la posición vertical de las fuentes dentro de un párrafo utilizando la nueva propiedad public [baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/) y la nueva enumeración [BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/).

#### Control de Color de Primer Plano <sup>23.10</sup>

La capacidad de recuperar el color de primer plano sin modificadores se ha agregado a las clases [Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/) y [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) a través de la propiedad **BaseForeColor**.

#### Ampliación de la Funcionalidad de los Gráficos <sup>23.10</sup>

La funcionalidad de las clases [ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/) y [ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/) se ha ampliado con nuevos métodos y propiedades.

#### Ajusta y ajusta Automáticamente una Imagen en una Forma <sup>23.10</sup>

Se ha proporcionado una forma sencilla de ajustar y ajustar automáticamente una imagen dentro de una forma particular a través del nuevo método [fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default).

#### Formato de fuente Predeterminado para las Entradas de Leyenda de Gráfico DrawingML <sup>23.11</sup>

Se ha agregado la capacidad de especificar el formato de fuente predeterminado para las entradas de leyenda de los gráficos DrawingML a través de la propiedad [font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/). Esta característica facilita una apariencia más optimizada y consistente para los elementos del gráfico, mejorando la estética general del documento.

#### Especifique el Diseño de página al Abrir PDF en Reader <sup>23.12</sup>

Se ha agregado la capacidad de especificar el diseño de página que se utilizará al abrir un documento en un lector PDF mediante la introducción de una nueva propiedad [page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/) en la clase [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) y la introducción de una nueva enumeración [PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/).

### Cargar y Guardar Documentos

#### Especificar un Nombre de Carpeta para Construir la Imagen URIs en Markdown <sup>23.9</sup>

La clase [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) se ha ampliado al incluir la propiedad [images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/), que permite especificar el nombre de la carpeta utilizada para construir la imagen URIs escrita en el documento Markdown.

#### Reducir el Tamaño de Salida PDF <sup>23.10</sup>

Se han implementado varias optimizaciones de renderizado PDF para reducir el tamaño de salida al utilizar la configuración [optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/).

#### Reconocer Hipervínculos al Cargar Documentos TXT <sup>23.10</sup>

La función para reconocer hipervínculos al cargar documentos TXT se ha implementado agregando una nueva propiedad [detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/).

### Otros

- Se ha implementado la emulación de representación de metarchivo para determinar el tamaño de rasterización, específicamente para el ancho del lápiz WMF y el ancho del lápiz cosmético EMF. Para lograr esto, la propiedad **ScaleWmfFontsToMetafileSize** se reemplazó con la propiedad [emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/) y se agregó la propiedad [emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/). <sup>23.9</sup>
- Se ha introducido un método simplificado para insertar un documento en otro documento en la posición actual del cursor utilizando el método [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions). <sup>23.10</sup>
- La capacidad de acceder y modificar propiedades de estilo se ha agregado mediante la introducción de la nueva propiedad [locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/). <sup>23.10</sup>
- Se ha agregado un parámetro de tipo genérico a los métodos de la clase [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/). <sup>23.10</sup>
- La capacidad de escribir todas las secciones de un documento en la misma hoja de cálculo XLSX se ha proporcionado a través del nuevo tipo de enumeración [XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/) y la nueva propiedad [section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/). <sup>23.11</sup>
* Se ha implementado una forma de controlar cómo se utilizarán las extensiones de formato ZIP64 para los documentos OOXML a través de la nueva propiedad Zip64Mode de la clase `OoxmlSaveOptions` y la nueva enumeración Zip64Mode. <sup>23.12</sup>
* Se ha introducido soporte para la imagen WebP. Tenga en cuenta que esta función solo está disponible para .versiones NetStandart y .NET6+. <sup>23.12</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por Python via .NET 23.9 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 23.10 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 23.11 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

Más información sobre [Aspose.Words por .NET 23.12 Notas de la Versión](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words para Python a través de .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 mejora la capacidad de trabajar con datos de series de gráficos y la capacidad de trabajar con documentos ODT, así como mejorar los encabezados/pies de página y su ajuste de texto.

Aspose.Words 23.6 amplía las opciones de representación, agrega un nuevo formato de exportación, mejora los informes LINQ y las herramientas LowCode.

Aspose.Words 23.7 mejora las capacidades de generación de informes, agrega un nuevo formato de exportación e introduce cambios en el trabajo con tablas y firmas digitales.

Aspose.Words 23.8 amplía las capacidades de diferentes formatos, mejora el procesamiento y agrega nuevas opciones para trabajar con campos.

### Formatos Admitidos

* A partir de la versión 23.6, es posible guardar un documento en formato XLSX. Ahora puedes convertir tus documentos a formato Excel. <sup>23.6</sup>

* A partir de la versión 23.7, es posible guardar una página o forma de documento en formato EPS. <sup>23.7</sup>

### Nuevas Funciones de Formato

- Se ha introducido la funcionalidad para generar automáticamente una Tabla de contenido (TOC) para MOBI documentos. <sup>23.8</sup>
- El constructor [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) se ha expandido con [PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions). <sup>23.8</sup>
- Se ha implementado la configuración de texto vertical para metarchivos EMF. <sup>23.8</sup>

### Renderizado

#### Obtener y Modificar Datos de Series de Gráficos <sup>23.5</sup>

La función para obtener y modificar datos de series de gráficos se proporcionó agregando:

- nuevas clases: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- nuevos tipos de enumeración: [ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### Soporte para Tipografía Avanzada <sup>23.6</sup>

Se ha agregado soporte para tipografía avanzada en WMF, EMF y EMF+ renderizado.

#### Contenido coloreado en la página <sup>23.6</sup>

Se ha agregado la propiedad pública [PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/), que indica si la página está coloreada o no.

#### Formateo de Etiquetas de Datos de Gráficos <sup>23.6</sup>

Se ha implementado la capacidad de establecer el formato de relleno, trazo y llamada para las etiquetas de datos del gráfico.

### Mail Merge y Presentación de Informes

#### Inserción dinámica HTML para el Motor de Informes LINQ <sup>23.6</sup>

Se ha agregado una nueva forma de inserción dinámica HTML para el motor de informes LINQ.

#### Mustache Soporte de etiquetas <sup>23.7</sup>

Las etiquetas Mustache ahora son compatibles con los métodos [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/) y [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/).

#### Especificar el Tamaño de las Imágenes Renderizadas <sup>23.8</sup>

Se ha introducido una nueva propiedad pública [image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/) para especificar el tamaño de las imágenes renderizadas en píxeles.

#### Conservar espacios en blanco para JSON Valores de cadena - LINQ <sup>23.8</sup>

Se ha agregado una opción al Motor de informes LINQ para conservar los espacios en blanco para los valores de cadena JSON.

### LowCode <sup>23.6</sup>

Se han agregado nuevos métodos LowCode destinados a fusionar diferentes tipos de documentos en un solo documento de salida.

### Otros

- Se ha implementado el soporte para el ajuste de texto en encabezados/pies de página. <sup>23.5</sup>
- Se ha agregado la capacidad de eliminar firmas digitales de ODT documentos a través del método [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str). <sup>23.5</sup>
- Se ha añadido la propiedad pública [phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/) para obtener el texto base y rubí de la guía fonética [Run](https://reference.aspose.com/words/python-net/aspose.words/run/). <sup>23.5</sup>
- Se ha agregado la capacidad de recuperar un valor de firma digital de un documento firmado digitalmente como una matriz de bytes al introducir una nueva propiedad [signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/). <sup>23.7</sup>
- Las clases [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/) y [Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/) se han ampliado con nuevos miembros públicos– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), y [Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/). <sup>23.7</sup>

{{% alert color="primary" %}}

Más información sobre [Aspose.Words por Python via .NET 23.5 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-5-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 23.6 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-6-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 23.7 Notas de la versión](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

Más información sobre [Aspose.Words por Python via .NET 23.8 Notas de la versión](/words/python-net/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## Véase También

{{% alert color="primary" %}}

Esta página contiene las últimas noticias de lanzamiento de los últimos 2 años. Para obtener detalles sobre versiones anteriores, consulte [Notas de la versión'](https://releases.aspose.com/words/python/release-notes/) páginas en las secciones relevantes.

{{% /alert %}}
