---
title: O que há de novo
second_title: Aspose.Words Para .NET
articleTitle: O que há de novo em Aspose.Words Para .NET
linktitle: O que há de novo em Aspose.Words Para .NET
type: docs
description: "Aspose.Words Para .NET expande e melhora diariamente. Nesta página, você pode aprender sobre as características enormes e mais interessantes do produto."
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pt/net/what-s-new-in-aspose-words-for-net/
timestamp: 2025-04-16-07-02-05
---

Esta página descreve os novos recursos Aspose.Words mais interessantes introduzidos em versões recentes.

## Aspose.Words para .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 introduz a verificação gramatical com AI e aprimora o salvamento de documentos com opções avançadas para os formatos HTML, SVG e Markdown.

Aspose.Words 25.2 introduz sumarização de texto com Anthropic AI modelos, adiciona MsWorks suporte ao formato, aprimora o controle tipográfico e melhora a estrutura PDF e o tratamento de listas.

Aspose.Words 25.3 melhora um verificador gramatical com AI e a seleção de fontes com a propriedade UpdateAmbiguousTextFont, bem como melhora a exportação de anexos PDF.

Aspose.Words 25.4 introduz suporte para novos tamanhos de papel, habilita o controle avançado de exportação de HTML, melhora o manuseio da marca d'água e melhora a usabilidade do LowCode API.

### AI - recursos alimentados

#### Documento AI Verificação Gramatical

* A capacidade de verificar a gramática do documento fornecido utilizando modelos generativos OpenAI foi introduzida através da adição de um novo método [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/). <sup>25.1</sup>
* O recurso de verificação gramatical com AI foi atualizado para suportar todos os modelos disponíveis na enumeração [AiModelType](https://reference.aspose.com/words/net/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### Resumo Usando Anthropic Modelos De Linguagem Generativa <sup>25.2</sup>

A sumarização de texto usando Anthropic Modelos de linguagem generativa foi habilitada pela introdução de uma nova classe pública [AnthropicAiModel](https://reference.aspose.com/words/net/aspose.words.ai/anthropicaimodel/).

### Low Code

#### Low Code API usabilidade <sup>25.4</sup>

Foram introduzidas melhorias significativas na usabilidade do **LowCode API**, simplificando o processamento de documentos e reduzindo a necessidade de código repetitivo.

### Formatos Suportados <sup>25.2</sup>

A partir da versão 25.2, foi adicionada a compatibilidade com o novo formato de carregamento MsWorks para os documentos de trabalho Microsoft.

### Converter, carregar e guardar documentos

#### Melhoria da poupança para os formatos HTML e SVG <sup>25.1</sup>

Salvar nos formatos HTML e SVG foi aprimorado adicionando propriedades **IdPrefix** e **RemoveJavaScriptFromLinks** às classes [HtmlFixedSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlfixedsaveoptions/) e [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/).

#### Defina a Resolução da imagem e o modo de saída OfficeMath ao Salvar para Markdown <sup>25.1</sup>

* Uma nova opção [ImageResolution](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imageresolution/) foi adicionada à classe [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) para definir a resolução da imagem.
* Uma nova opção [OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/officemathexportmode/) e uma enumeração [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownofficemathexportmode/) foram adicionadas à classe [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) para definir o modo de saída OfficeMath.
* A capacidade de definir uma marca d'água de imagem a partir de um fluxo foi introduzida adicionando uma nova sobrecarga ao método [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage_2). <sup>25.4</sup>

### Renderização

#### Melhor Controlo Tipográfico <sup>25.2</sup>

A propriedade [NumberSpacing](https://reference.aspose.com/words/net/aspose.words/font/numberspacing/) foi adicionada para melhorar o controlo Tipográfico.

#### Controlando a seleção de fontes para caracteres ambíguos <sup>25.3</sup>

Uma nova propriedade pública [UpdateAmbiguousTextFont](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/updateambiguoustextfont/) foi adicionada à classe [SaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/) para controlar a seleção da fonte de acordo com o código de caracteres usado.

#### Opções De Tamanho De Papel <sup>25.4</sup>

A capacidade de utilizar os tamanhos de papel JIS B4 e JIS B5 foi introduzida adicionando novos valores à enumeração [PaperSize](https://reference.aspose.com/words/net/aspose.words/papersize/).

#### HTML Controlo De Saída <sup>25.4</sup>

A capacidade de remover JavaScript da hiperligação URLs durante a exportação HTML foi introduzida adicionando a propriedade [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/removejavascriptfromlinks/).

### Outros

* PDF a estrutura lógica foi melhorada com suporte para os campos TOA, BIBLIOGRAPHY e INDEX. <sup>25.2</sup>
* O método [AddSingleLevelList](https://reference.aspose.com/words/net/aspose.words.lists/listcollection/addsinglelevellist/) foi introduzido para melhorar o tratamento de listas. <sup>25.2</sup>
* Uma nova propriedade [AttachmentsEmbeddingMode](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/attachmentsembeddingmode/) foi adicionada para substituir **EmbedAttachments** para melhorar a exportação de PDF anexos. Além disso, novos valores foram adicionados à enumeração [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) para suportar anexos de versão PDF/A. Além disso, os anexos são agora suportados com encriptação. <sup>25.3</sup>

{{% alert color="primary" %}}

Saiba mais sobre [Aspose.Words para .NET 25.1 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-1-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 25.2 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-2-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 25.3 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-3-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 25.4 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words para .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduz group shape inserção e StructuredDocumentTag inserção via DocumentBuilder, melhora a renderização de gráficos radiais com graduações, melhora as assinaturas digitais com suporte a XAdES-EPES, adiciona reconhecimento de sublinhado Markdown e fornece acesso a separadores de notas de rodapé/notas de fim.

Aspose.Words 24.10 introduz um suporte de controlo ActiveX melhorado com a criação de CommandButton, um novo controlo de visibilidade de forma, a capacidade de group shapes, exportação Markdown melhorada para tabelas, formatação de gráficos para Pie e Doughnut Gráficos, Melhor Tratamento de codificação Big5 e suporte para Fontes taiwanesas desatualizadas.

Aspose.Words 24.11 introduz AI sumarização de documentos, opções de renderização aprimoradas, acesso aprimorado às propriedades do documento e ActiveX Legendas de controle.

Aspose.Words 24.12 introduz a colocação de etiquetas de dados personalizáveis, a tradução de texto com o Google AI, as opções de limpeza Mail Merge melhoradas e as novas classes de processamento LowCode.

### AI - recursos alimentados

#### Resumo do documento usando OpenAI e Google <sup>24.11</sup>

O suporte para sumarização de documentos usando modelos de linguagem generativa **OpenAI** e **Google** foi integrado adicionando o namespace [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) com seus membros públicos.

#### Tradução de texto usando os modelos de linguagem generativa do Google <sup>24.12</sup>

A capacidade de traduzir texto usando os modelos de linguagem generativa do Google foi implementada em Aspose.Words Adicionando o método [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) e a enumeração [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) ao namespace [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

Novas LowCode classes como [Comparer](https://reference.aspose.com/words/net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/net/aspose.words.lowcode/splitter/) etc. foi introduzido, oferecendo um conjunto de métodos que alcançam o equilíbrio perfeito entre simplicidade e flexibilidade para o processamento de documentos.

### Renderização e impressão

#### Graduações em gráficos radiais <sup>24.9</sup>

A renderização de graduações em gráficos radiais foi implementada.

#### CommandButton ActiveX controlos <sup>24.10</sup>

A capacidade de criar controles CommandButton ActiveX foi introduzida adicionando um novo método público [InsertForms2OleControl](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertforms2olecontrol/) e uma nova classe pública [Forms2OleControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/).

#### Visibilidade Da Forma De Controlo <sup>24.10</sup>

Uma nova propriedade pública [Hidden](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/hidden/) foi adicionada para controlar a visibilidade das formas.

#### Alterações nos gráficos Pie e Doughnut <sup>24.10</sup>

Várias novas propriedades públicas foram adicionadas aos gráficos format Pie e Doughnut.

#### Controlar a renderização das bordas do campo do formulário de escolha PDF <sup>24.11</sup>

Uma nova opção para controlar a renderização de PDF fronteiras de campo de formulário de escolha foi implementada adicionando uma nova opção pública [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/renderchoiceformfieldborder/).

#### Obter e definir códigos de formato para dados do Gráfico <sup>24.11</sup>

A capacidade de obter e definir códigos de formato para dados de gráfico foi adicionada implementando a propriedade [FormatCode](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/formatcode/) nas classes [ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/) e [BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/).

#### Renderizar gráficos de histograma com caixas e rótulos <sup>24.11</sup>

A renderização do Gráfico de histograma foi melhorada, permitindo um número especificado de caixas e rótulos.

#### Personalizar a colocação de rótulos de dados <sup>24.12</sup>

A capacidade de personalizar a colocação de rótulos de dados foi adicionada através da introdução de novas propriedades nas classes [ChartDataLabel](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabel/) e [ChartDataLabelCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/).

### Converter, carregar e guardar documentos

#### Sublinhar a formatação ao carregar ficheiros Markdown <sup>24.9</sup>

A opção de reconhecer a formatação de sublinhado ao carregar documentos Markdown foi incorporada adicionando uma nova propriedade pública [ImportUnderlineFormatting](https://reference.aspose.com/words/net/aspose.words.loading/markdownloadoptions/importunderlineformatting/).

#### Exportando tabelas como HTML ao salvar em Markdown <sup>24.10</sup>

Uma opção para exportar tabelas como HTML ao salvar documentos no formato Markdown foi implementada adicionando uma nova propriedade pública [ExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/exportashtml/) e uma enumeração [MarkdownExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownexportashtml/).

#### Exportar PDF com estrutura lógica actualizada <sup>24.11</sup>

PDF a exportação foi melhorada através da inclusão de propriedades de título de tabela como PDF títulos de elementos de estrutura lógica.

### Mail Merge e relatórios

#### Remover tabelas vazias durante Mail Merge <sup>24.12</sup>

Uma nova opção **RemoveEmptyTables** foi adicionada à enumeração [MailMergeCleanupOptions](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmergecleanupoptions/) para refinar a saída Mail Merge.

### Assinaturas Digitais

#### Assinar documentos com XAdES-EPES <sup>24.9</sup>

A capacidade de assinar documentos com assinaturas de XAdES-EPES Nível XML-DSig foi introduzida adicionando uma nova propriedade pública [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/signoptions/xmldsiglevel/) e uma nova enumeração pública [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/xmldsiglevel/).

### Outros

* Um novo método público [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/) foi adicionado a group shapes. <sup>24.9</sup>
* Um novo método público [InsertStructuredDocumentTag](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertstructureddocumenttag/) foi adicionado para inserir **StructuredDocumentTags** em um documento. <sup>24.9</sup>
* O acesso público aos separadores de notas de rodapé/notas de fim foi proporcionado pela adição de algumas classes e propriedades públicas. <sup>24.9</sup>
* A capacidade de agrupar formas individuais, group shapes juntas, e agrupar diretamente ambas as formas e group shapes foi introduzida pela adição do método [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/#insertgroupshape_1). <sup>24.10</sup>
* O tratamento de codificação Big5 para TrueType tabelas cmap foi melhorado. <sup>24.10</sup>
* O Suporte Para fontes taiwanesas desatualizadas foi aprimorado. <sup>24.10</sup>
* Para acessar as propriedades do documento estendido, propriedades somente leitura foram adicionadas à classe [BuiltInDocumentProperties](https://reference.aspose.com/words/net/aspose.words.properties/builtindocumentproperties/). <sup>24.11</sup>
* A definição de legendas para os controlos ActiveX foi activada adicionando um novo setter público à propriedade [Forms2OleControl.Caption](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/caption/). <sup>24.11</sup>

{{% alert color="primary" %}}

Saiba mais sobre [Aspose.Words para .NET 24.9 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-9-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 24.10 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-10-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 24.11 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-11-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 24.12 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words para .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 expande as opções para assemblies, melhora os recursos de renderização e expande algumas outras opções.

Aspose.Words 24.6 melhora as opções de renderização, melhora a funcionalidade de pesquisa e comparação e expande vários outros recursos.

Aspose.Words 24.7 altera a forma como trabalha com ActiveX, expande as capacidades de renderização, bem como exporta para os formatos Markdown e XLSX.

Aspose.Words 24.8 aprimora a personalização do gráfico com controle preciso sobre os rótulos dos eixos, expande o gerenciamento de fontes, melhora o manuseio da estrutura do documento e adiciona novos recursos para exportação HTML/XAML, funcionalidade PDF, conversão de documentos e assinaturas digitais.

### Formatos Suportados

A partir da versão 24.7, a exportação para PDF/UA-2 é suportada para garantir a acessibilidade aos utilizadores com deficiência.

### Plataformas <sup>24.5</sup>

.NET 7.0/8.0 assemblies foram incluídos no pacote Aspose.Words NuGet.

### Renderização e impressão

#### Alterações nos gráficos, formas e DrawingML <sup>24.5</sup>

* DrawingML a renderização de efeitos para SVG gráficos, estendendo a funcionalidade anterior limitada a imagens, foi implementada.
* Foi introduzido o suporte para a criação de gráficos combinados e para o ajuste de propriedades, tais como a largura do intervalo, a sobreposição e a escala de bolhas nos grupos de séries, adicionando-se as classes [ChartSeriesGroup](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroup/) e [ChartSeriesGroupCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroupcollection/) e a propriedade [SeriesGroups](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/seriesgroups/).
* A funcionalidade para manipular o efeito SoftEdge das formas foi implementada adicionando a classe [SoftEdgeFormat](https://reference.aspose.com/words/net/aspose.words.drawing/softedgeformat/).
* A capacidade de modificar ajustar valores de formas foi implementada adicionando as classes públicas [AdjustmentCollection](https://reference.aspose.com/words/net/aspose.words.drawing/adjustmentcollection/) e [Adjustment](https://reference.aspose.com/words/net/aspose.words.drawing/adjustment/) e a propriedade [Adjustments](https://reference.aspose.com/words/net/aspose.words.drawing/shape/adjustments/).

#### Alterações nos gráficos, formas e desenhos <sup>24.6</sup>

* As capacidades de gráficos foram melhoradas. Agora você pode criar uma variedade maior de gráficos, incluindo *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* gráficos, *Box & Whisker* gráficos, *Waterfalls* e *Funnels*. Isto permite-lhe visualizar os seus dados de uma forma mais diversificada e informativa.
* O controlo das cores para a formatação das Sombras foi melhorado. Você pode obter um controle mais preciso sobre a aparência de seus documentos acessando cores de sombra.
* O aumento de desempenho para a renderização em segundo plano foi melhorado. Você pode acelerar significativamente a renderização de fundos contendo pequenos elementos graças à tecnologia nativa de ladrilhos.
* Foram adicionados gradientes realistas para formas. Agora você pode criar DML formas com gradientes não lineares, imitando o estilo visual de Microsoft Word para uma aparência mais polida.

#### Personalização Do Rótulo Dos Dados Do Gráfico <sup>24.7</sup>

Foi adicionada a capacidade de personalizar rótulos de dados do gráfico, como **Orientation** e **Rotation**.

#### Estilo De Número personalizado para níveis de Lista <sup>24.7</sup>

Foi adicionado um setter para a propriedade pública [CustomNumberStyleFormat](https://reference.aspose.com/words/net/aspose.words.lists/listlevel/customnumberstyleformat/). Agora você pode definir um estilo de número personalizado para níveis de lista.

#### Mudanças no trabalho com ActiveX <sup>24.7</sup>

* As propriedades dos objectos ActiveX podem agora ser modificadas, dando - lhe mais controlo sobre o seu comportamento.
* Foi adicionada a capacidade de modificar o valor do controlo do botão de opção ActiveX para permitir a interacção dinâmica.
* A capacidade de alternar um ActiveX checkbox para "marcado" ou "desmarcado" foi adicionada.

#### Controlo sobre a orientação e rotação das etiquetas de Marcação Do Eixo do Gráfico <sup>24.8</sup>

Foi adicionado um controlo preciso sobre a orientação e rotação dos rótulos de escala do eixo do gráfico para uma personalização mais conveniente do gráfico – A classe [AxisTickLabels](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/) foi alargada com novas propriedades [Orientation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/orientation/) e [Rotation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/rotation/).

#### Substituindo a barra invertida pelo sinal do Iene <sup>24.8</sup>

A exportação HTML e XAML Compatível com versões anteriores para substituir o caractere de barra invertida pelo sinal de iene foi melhorada. Para conseguir isso, a propriedade **ReplaceBackslashWithYenSign** foi adicionada às classes [HtmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/) e [XamlFlowSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xamlflowsaveoptions/).

#### Usando SDT Tags como nomes de campo de formulário ao exportar para PDF <sup>24.8</sup>

A exportação PDF com suporte para o uso de tags SDT como nomes de campos de formulário foi aprimorada adicionando uma nova propriedade [UseSdtTagAsFormFieldName](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/usesdttagasformfieldname/) à classe [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/).

### Converter, carregar e guardar documentos

#### Exportando Links para o formato Markdown <sup>24.7</sup>

A capacidade de controlar a exportação de links no formato Markdown foi adicionada através da implementação da propriedade [LinkExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/linkexportmode/).

#### LowCode 24.8 <sup>24.8</sup>

Foi introduzida uma nova classe [LowCode.Converter](https://reference.aspose.com/words/net/aspose.words.lowcode/converter/), concebida para fornecer um conjunto de métodos para converter vários tipos de documentos com uma única linha de código.

### Pesquisar e comparar

#### Opções Avançadas De Comparação <sup>24.6</sup>
Foi adicionada a capacidade de simplificar os fluxos de trabalho de análise de dados com uma funcionalidade de comparação melhorada. Isso inclui uma nova opção [IgnoreStoreItemId](https://reference.aspose.com/words/net/aspose.words.comparing/advancedcompareoptions/ignorestoreitemid/) e uma interface redesenhada para comparações avançadas.

### Outros

* A função para eliminar páginas vazias de um documento foi implementada adicionando o método [RemoveBlankPages](https://reference.aspose.com/words/net/aspose.words/document/removeblankpages/). <sup>24.5</sup>
* A capacidade de verificar a presença de VBA macros sem carregar um documento foi fornecida adicionando a propriedade [HasMacros](https://reference.aspose.com/words/net/aspose.words/fileformatinfo/hasmacros/). <sup>24.5</sup>
* A manutenção da numeração de origem durante a inserção de um documento utilizando o mecanismo de relatórios LINQ é agora suportada. <sup>24.5</sup>
* Uma nova propriedade [DateTimeUtc](https://reference.aspose.com/words/net/aspose.words/comment/datetimeutc/) foi adicionada-isto fornece um carimbo de data / hora mais preciso para os comentários, melhorando a organização e a rastreabilidade. <sup>24.6</sup>
* O mecanismo de relatórios LINQ foi melhorado. A remoção selectiva de parágrafos vazios e a definição de mensagens personalizadas para membros de objectos em falta foram efectuadas, o que levou a relatórios mais limpos e informativos. <sup>24.6</sup>
* O formato datetime agora é detectado automaticamente para exportação contínua para o formato XLSX. <sup>24.7</sup>
* A propriedade pública [IsProtected](https://reference.aspose.com/words/net/aspose.words.vba/vbaproject/isprotected/), que permite verificar se um projeto VBA está protegido, foi adicionada. <sup>24.7</sup>
* As informações da fonte foram expandidas com a propriedade **EmbeddingLicensingRights** adicionada às classes [FontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/fontinfo/) e [PhysicalFontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/physicalfontinfo/). <sup>24.8</sup>
* Uma maneira de limpar eficientemente os cabeçalhos e rodapés das seções, preservando marcas d'água, foi adicionada para trabalhar com mais precisão com a estrutura do documento. Para limpar os cabeçalhos e rodapés das secções, utilize o novo método público [ClearHeadersFooters](https://reference.aspose.com/words/net/aspose.words/section/clearheadersfooters/). <sup>24.8</sup>
* A assinatura Digital de XPS documentos usando [XpsSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/) foi ativada – uma nova propriedade [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/digitalsignaturedetails/) foi adicionada para esse fim. <sup>24.8</sup>

{{% alert color="primary" %}}

Saiba mais sobre [Aspose.Words para .NET 24.5 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-5-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 24.6 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-6-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 24.7 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-7-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 24.8 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words para .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 melhora a experiência em torno do gerenciamento de cores de traçado, aprimora OLE objetos e LINQ relatórios, bem como introduz um novo `Bibliography Sources` Público API.

Aspose.Words 24.2 gráficos expandidos API, gestão de estilos e opções LINQ. Esta versão de Aspose.Words também introduziu a capacidade de especificar SvgSaveOptions durante a renderização, controle mais flexível Carregando Markdown arquivos e trabalhando com texto de referência para notas de rodapé e notas de fim.

Aspose.Words 24.3 introduz um novo TIFF Leitor/Gravador e emulação de operações de varredura binária para WMF metarquivos. Aspose.Words 24.3 também continua a expandir os gráficos API.

Aspose.Words 24.4 melhora os formatos de gravação, algumas opções de renderização, bem como melhora o trabalho com assinaturas digitais.

### Formatos Suportados <sup>24.4</sup>

O formato de imagem **WebP** moderno é agora suportado em Aspose.Words para .NET Framework 4.6.2 e mais alto. Agora você pode ler e inserir imagens WebP em documentos, bem como salvar imagens no formato WebP.

Observe que WebP está atualmente disponível apenas em .NET Standard e .NET Framework v4.6.2 e acima.

### Renderização e impressão

#### Controlo Da Cor Do Traçado <sup>24.1</sup>

A classe [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) foi estendida com um conjunto de novas propriedades públicas relacionadas ao gerenciamento de cores de traçado: [ForeThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/forethemecolor/) e [BackThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/foretintandshade/) e [BackTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backtintandshade/).

#### DrawingML Gráficos API Extensão <sup>24.2 / 24.3 / 24.4</sup>

O **DrawingML Charts API** continua a ser expandido.

#### Incorporar fontes declaradas em @font-face regras <sup>24.4</sup>

Adicionada a capacidade de incorporar fontes declaradas nas regras @font-face nas definições de fonte do documento resultante foi introduzida adicionando uma nova propriedade [SupportFontFaceRules](https://reference.aspose.com/words/net/aspose.words.loading/htmlloadoptions/supportfontfacerules/).

#### Trabalhar com formatação de brilho e reflexão <sup>24.4</sup>

A capacidade de trabalhar com formatação de brilho e reflexão para um objeto de desenho foi implementada.

### Carregar e guardar documentos

#### Especifique SvgSaveOptions Durante A Renderização <sup>24.2</sup>

A capacidade de especificar [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/) durante a renderização foi adicionada usando o [ShapeRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) e [OfficeMathRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) métodos.

#### Preservar linhas vazias ao carregar ficheiros Markdown <sup>24.2</sup>

A capacidade de preservar linhas vazias ao carregar arquivos Markdown foi adicionada.

#### Um Novo TIFF Leitor / Escritor <sup>24.3</sup>

Foi desenvolvido um novo leitor/gravador TIFF para Aspose.Words para .NET Standard, .NET 6 e posteriores. Aspose.Words para .NET 24.3 Adicionado suporte para leitura de imagens TIFF com tipos de compressão JPEG e antigos JPEG, e também melhorou significativamente a qualidade das operações de leitura e gravação.

### Outros

* A capacidade de modificar o texto do controlo `TextBox` OLE foi introduzida adicionando uma nova propriedade [Text](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/text/) à nova classe [TextBoxControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/). <sup>24.1</sup>
* A bibliografia Sources public API foi implementada através da adição de um novo namespace [Aspose.Words.Bibliography](https://reference.aspose.com/words/net/aspose.words.bibliography/) com as suas novas classes e enumerações, e através da adição de uma nova propriedade [Bibliography](https://reference.aspose.com/words/net/aspose.words/document/bibliography/) à classe [Document](https://reference.aspose.com/words/net/aspose.words/document/). <sup>24.1</sup>
* Um API para limitar o acesso aos membros do tipo usando a sintaxe do modelo para o `LINQ Reporting Engine` foi fornecido. <sup>24.1</sup>
* Novas propriedades públicas [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) e [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) para gerenciamento de estilo aprimorado foram adicionadas à classe [Style](https://reference.aspose.com/words/net/aspose.words/style/). <sup>24.2</sup>
* A funcionalidade para recuperar o texto real da marca de referência para notas de rodapé e notas de fim foi melhorada com a propriedade [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) e o método [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
* A compatibilidade com os gráficos `Word 2016` para o `LINQ Reporting Engine` foi activada. <sup>24.2</sup>
* A emulação de operações de varredura binária para metarquivos WMF foi implementada. <sup>24.3</sup>
* A capacidade de definir opções de assinatura para documentos dentro de **SaveOptions** foi habilitada adicionando uma nova classe [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/digitalsignaturedetails/) com novos membros públicos, bem como adicionando novas propriedades às classes [OoxmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/docsaveoptions/) e [OdtSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Saiba mais sobre [Aspose.Words para .NET 24.1 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-1-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 24.2 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-2-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 24.3 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-3-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 24.4 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words para .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 expande as opções de renderização, emulação de renderização de metarquivo e opções de salvamento de markdown.

Aspose.Words 23.10 melhora a renderização, expande as opções para carregar e salvar documentos e permite que os usuários mesclem documentos de novas maneiras.

Aspose.Words 23.11 melhora o trabalho com revisões, XLSX formato e fontes na legenda do gráfico com opções adicionais.

Aspose.Words 23.12 introduz novas propriedades e enumerações para trabalhar com documentos PDF e OOXML, bem como suporte para imagens WebP.

### Renderização e impressão

#### Personalização dos títulos dos eixos em gráficos DrawingML <sup>23.9</sup>

A capacidade de personalizar títulos de eixos em gráficos DrawingML foi introduzida pela implementação de uma nova propriedade public class [ChartAxisTitle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxistitle/) e [Title](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxis/title/).

#### Determinação da posição Vertical das fontes num parágrafo <sup>23.9</sup>

Agora é possível definir a posição vertical das fontes dentro de um parágrafo usando a nova propriedade public [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/paragraphformat/baselinealignment/) e a nova enumeração [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/baselinealignment/).

#### Controlo Da Cor Do Primeiro Plano <sup>23.10</sup>

A capacidade de recuperar a cor de primeiro plano sem modificadores foi adicionada às classes [Fill](https://reference.aspose.com/words/net/aspose.words.drawing/fill/) e [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) através da propriedade **BaseForeColor**.

#### Expansão da funcionalidade dos gráficos <sup>23.10</sup>

A funcionalidade das classes [ChartDataPointCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseries/) e [ChartFormat](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartformat/) foi expandida com novos métodos e propriedades.

#### Ajustar e ajustar automaticamente uma imagem numa forma <sup>23.10</sup>

Uma maneira simples de ajustar e ajustar automaticamente uma imagem dentro de uma forma específica foi fornecida através do novo método [FitImageToShape](https://reference.aspose.com/words/net/aspose.words.drawing/imagedata/fitimagetoshape/).

#### Formatação de fonte padrão para DrawingML entradas de legenda de gráfico <sup>23.11</sup>

A capacidade de especificar a formatação de fonte padrão para entradas de legenda de gráficos DrawingML foi adicionada por meio da propriedade [Font](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartlegend/font/). Este recurso facilita uma aparência mais simplificada e consistente para os elementos do gráfico, melhorando a estética geral do documento.

#### Especificar o Layout da Página ao Abrir PDF No Reader <sup>23.12</sup>

A capacidade de especificar o layout de página a ser usado ao abrir um documento em um leitor PDF foi adicionada através da introdução de uma nova propriedade [PageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/pagelayout/) à classe [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) e da introdução de uma nova enumeração [PdfPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfpagelayout/).

### Carregar e guardar documentos

#### Especificando um nome de pasta para construir a imagem URIs em Markdown <sup>23.9</sup>

A classe [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) foi expandida incluindo a propriedade [ImagesFolderAlias](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imagesfolderalias/), que permite especificar o nome da pasta usada para construir a imagem URIs escrita no documento Markdown.

#### Reduzir PDF Tamanho Da Saída <sup>23.10</sup>

Várias otimizações de renderização PDF para reduzir o tamanho da saída ao utilizar as configurações [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) foram implementadas.

#### Reconhecer hiperligações ao carregar TXT documentos <sup>23.10</sup>

O recurso para reconhecer hiperlinks ao carregar documentos TXT foi implementado adicionando uma nova propriedade [DetectHyperlinks](https://reference.aspose.com/words/net/aspose.words.loading/txtloadoptions/detecthyperlinks/).

### Outros

* A emulação de renderização de metarquivo para determinar o tamanho da rasterização foi implementada, especificamente para WMF Largura da caneta e EMF Largura da caneta cosmética. Para isso, a propriedade **ScaleWmfFontsToMetafileSize** foi substituída pela propriedade [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpage/) e a propriedade [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpageresolution/) foi adicionada. <sup>23.9</sup>
* Foi introduzido um método simplificado para inserir um documento noutro documento na posição actual do cursor utilizando o método [InsertDocumentInline](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertdocumentinline/). <sup>23.10</sup>
* A capacidade de aceder e modificar propriedades de estilo foi adicionada através da introdução da nova propriedade [Locked](https://reference.aspose.com/words/net/aspose.words/style/locked/). <sup>23.10</sup>
* Um parâmetro de tipo genérico foi adicionado aos métodos da classe [CompositeNode](https://reference.aspose.com/words/net/aspose.words/compositenode/). <sup>23.10</sup>
* Uma forma de controlar quando uma determinada revisão deve ser aceite/rejeitada ou não foi implementada utilizando os métodos [Accept](https://reference.aspose.com/words/net/aspose.words/revisioncollection/accept/) e [Reject](https://reference.aspose.com/words/net/aspose.words/revisioncollection/reject/). Esta melhoria confere aos utilizadores um controlo mais rigoroso sobre o processo de revisão. <sup>23.11</sup>
* A capacidade de escrever todas as secções de um documento na mesma folha de cálculo XLSX foi fornecida através do novo tipo de enumeração [XlsxSectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsectionmode/) e da propriedade new [SectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsaveoptions/sectionmode/). <sup>23.11</sup>
* Uma maneira de controlar como as extensões de formato ZIP64 serão usadas para documentos OOXML foi implementada por meio da nova propriedade Zip64Mode da classe `OoxmlSaveOptions` e da nova enumeração Zip64Mode. <sup>23.12</sup>
* Foi introduzido o suporte para a imagem WebP. Observe que esse recurso está disponível apenas para .NetStandart e .NET6+ versões. <sup>23.12</sup>

{{% alert color="primary" %}}

Saiba mais sobre [Aspose.Words para .NET 23.9 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-9-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 23.10 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-10-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 23.11 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-11-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 23.12 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words para .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 melhora a capacidade de trabalhar com dados de séries de gráficos e a capacidade de trabalhar com documentos ODT, bem como melhorar cabeçalhos/rodapés e sua quebra de texto.

Aspose.Words 23.6 expande as opções de renderização, adiciona um novo formato de exportação, melhora as ferramentas LINQ Relatórios e LowCode.

Aspose.Words 23.7 aprimora os recursos de relatórios, adiciona um novo formato de exportação e introduz alterações no trabalho com tabelas e assinaturas digitais.

Aspose.Words 23.8 expande as capacidades de diferentes formatos, melhora a renderização e adiciona novas opções para trabalhar com campos.

### Formatos Suportados

* A partir da versão 23.6, é possível guardar um documento no formato XLSX. Agora você pode converter seus documentos para o formato Excel. <sup>23.6</sup>
* A partir da versão 23.7, é possível guardar uma página ou forma de documento no formato EPS. <sup>23.7</sup>

### Novos Recursos De Formato

* Foi introduzida a funcionalidade para gerar automaticamente o sumário (TOC) para MOBI documentos. <sup>23.8</sup>
* O construtor [PdfEncryptionDetails](https://reference.aspose.com/words/net/aspose.words.saving/pdfencryptiondetails/pdfencryptiondetails/) foi expandido com [PdfPermissions](https://reference.aspose.com/words/net/aspose.words.saving/pdfpermissions/). <sup>23.8</sup>
* A definição do texto vertical para os metarquivos EMF foi implementada. <sup>23.8</sup>

### Renderização e impressão

#### Obter e modificar dados da série de gráficos <sup>23.5</sup>

O recurso para obter e modificar os dados da série de gráficos foi fornecido adicionando:

* novas classes: [ChartXValue](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartmultilevelvalue/)
* novos tipos de enum: [ChartXValueType](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluetype/), [ChartYValueType](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluetype/)

#### Suporte para tipografia avançada <sup>23.6</sup>

Foi adicionado suporte para tipografia avançada em WMF, EMF e EMF+ renderização.

#### Conteúdo colorido na página <sup>23.6</sup>

A propriedade pública [PageInfo.Colored](https://reference.aspose.com/words/net/aspose.words.rendering/pageinfo/colored/), indicando se a página é colorida ou não, foi adicionada.

#### Formatação dos rótulos dos dados do Gráfico <sup>23.6</sup>

A capacidade de definir preenchimento, traçado e formatação de texto explicativo para rótulos de dados de gráfico foi implementada.

### Mail Merge e relatórios

#### Dinâmica HTML inserção para LINQ Mecanismo de relatório <sup>23.6</sup>

Foi adicionada uma nova forma de inserção dinâmica HTML para o mecanismo de Relatórios LINQ.

#### Mustache Suporte A Tags <sup>23.7</sup>

As tags Mustache são agora suportadas nos métodos [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/getregionshierarchy/) e [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmerge/getfieldnamesforregion/#getfieldnamesforregion).

#### LINQ Actualizações Da Sintaxe Do Modelo Do Motor De Relatórios <sup>23.7</sup>

A sintaxe do modelo do mecanismo de Relatório LINQ agora suporta os métodos de extensão `ElementAt` e ElementAtOrDefault.

#### Especificando o tamanho das imagens renderizadas <sup>23.8</sup>

Foi introduzida uma nova propriedade pública [ImageSize](https://reference.aspose.com/words/net/aspose.words.saving/imagesaveoptions/imagesize/) para especificar o tamanho das imagens renderizadas em pixel.

#### Preservar espaços em branco para JSON valores de cadeia de caracteres - LINQ <sup>23.8</sup>

Uma opção foi adicionada ao mecanismo de relatório LINQ para preservar espaços em branco para valores de string JSON.

### LowCode <sup>23.6</sup>

Foram adicionados novos métodos LowCode destinados a fundir diferentes tipos de documentos num único documento de saída.

### Outros

* Foi implementado o apoio à quebra de texto nos cabeçalhos/rodapés. <sup>23.5</sup>
* A capacidade de remover assinaturas digitais de documentos ODT foi adicionada através do método [RemoveAllSignatures](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignatureutil/removeallsignatures/). <sup>23.5</sup>
* A propriedade pública [PhoneticGuide](https://reference.aspose.com/words/net/aspose.words/run/phoneticguide/) para obter o texto base e ruby do guia fonético [Run](https://reference.aspose.com/words/net/aspose.words/run/) foi adicionada. <sup>23.5</sup>
* A capacidade de recuperar um valor de assinatura digital de um documento assinado digitalmente como uma matriz de Bytes foi adicionada através da introdução de uma nova propriedade [SignatureValue](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/digitalsignature/signaturevalue/). <sup>23.7</sup>
* As classes [Row](https://reference.aspose.com/words/net/aspose.words.tables/row/) e [Cell](https://reference.aspose.com/words/net/aspose.words.tables/cell/) foram alargadas com novos membros públicos– [Row.NextRow](https://reference.aspose.com/words/net/aspose.words.tables/row/nextrow/), [Row.PreviousRow](https://reference.aspose.com/words/net/aspose.words.tables/row/previousrow/), [Cell.NextCell](https://reference.aspose.com/words/net/aspose.words.tables/cell/nextcell/), e [Cell.PreviousCell](https://reference.aspose.com/words/net/aspose.words.tables/cell/previouscell/). <sup>23.7</sup>
* Foi adicionado suporte para os campos CITATION e BIBLIOGRAPHY. <sup>23.8</sup>

{{% alert color="primary" %}}

Saiba mais sobre [Aspose.Words para .NET 23.5 Notas De Lançamento](/words/net/aspose-words-for-net-23-5-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 23.6 Notas De Lançamento](/words/net/aspose-words-for-net-23-6-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 23.7 Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-7-release-notes/).

Saiba mais sobre [Aspose.Words para .NET 23.8 Notas De Lançamento](/words/net/aspose-words-for-net-23-8-release-notes/).

{{% /alert %}}

## Ver Também

{{% alert color="primary" %}}

Esta página contém as últimas notícias de lançamento dos últimos 2 anos. Para obter detalhes sobre versões anteriores, consulte o [Notas De Lançamento](https://releases.aspose.com/words/net/release-notes/) páginas nas secções relevantes.

{{% /alert %}}
