---
title: O que há de novo
second_title: Aspose.Words Para C++
articleTitle: O que há de novo em Aspose.Words Para C++
linktitle: O que há de novo em Aspose.Words Para C++
type: docs
description: "Aspose.Words Para C++ expande e melhora diariamente. Nesta página, você pode aprender sobre as características enormes e mais interessantes do produto."
weight: 2
url: /pt/cpp/what-s-new-in-aspose-words-for-cpp/
timestamp: 2025-03-09-12-38-00
---

Esta página descreve os novos recursos Aspose.Words mais interessantes introduzidos em versões recentes.

## Aspose.Words para C++ 25.1, 25.2

Aspose.Words 25.1 introduz a verificação gramatical com AI e aprimora o salvamento de documentos com opções avançadas para os formatos HTML, SVG e Markdown.

Aspose.Words 25.2 introduz a sumarização de texto com modelos antrópicos AI, adiciona suporte ao formato MsWorks, melhora o controle tipográfico e melhora a estrutura PDF e o tratamento de listas.

### AI - recursos alimentados

#### Documento AI Verificação Gramatical <sup>25.1</sup>

A capacidade de verificar a gramática do documento fornecido utilizando modelos generativos OpenAI foi introduzida através da adição de um novo método [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/).

#### Resumo Usando Modelos De Linguagem Gerativa Antrópica <sup>25.2</sup>

A sumarização do texto utilizando modelos de linguagem Gerativa antrópica foi possibilitada pela introdução de uma nova classe pública [AnthropicAiModel](https://reference.aspose.com/words/cpp/aspose.words.ai/).

### Formatos Suportados <sup>25.2</sup>

A partir da versão 25.2, foi adicionada a compatibilidade com o novo formato de carregamento MsWorks para os documentos de trabalho Microsoft.

### Converter, carregar e guardar documentos

#### Melhoria da poupança para os formatos HTML e SVG <sup>25.1</sup>

Salvar nos formatos HTML e SVG foi aprimorado adicionando propriedades **IdPrefix** e **RemoveJavaScriptFromLinks** às classes [HtmlFixedSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlfixedsaveoptions/) e [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/).

#### Defina a Resolução da imagem e o modo de saída OfficeMath ao Salvar para Markdown <sup>25.1</sup>

- Uma nova opção [ImageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imageresolution/) foi adicionada à classe [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) para definir a resolução da imagem.
- Uma nova opção [OfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_officemathexportmode/) e uma enumeração [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownofficemathexportmode/) foram adicionadas à classe [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) para definir o modo de saída OfficeMath.

### Renderização

#### Melhor Controlo Tipográfico <sup>25.2</sup>

A propriedade [NumberSpacing](https://reference.aspose.com/words/cpp/aspose.words/font/get_numberspacing/) foi adicionada para melhorar o controlo Tipográfico.

### Outros

- PDF a estrutura lógica foi melhorada com suporte para os campos TOA, BIBLIOGRAPHY e INDEX. <sup>25.2</sup>
- O método [AddSingleLevelList](https://reference.aspose.com/words/cpp/aspose.words.lists/listcollection/addsinglelevellist/) foi introduzido para melhorar o tratamento de listas. <sup>25.2</sup>

{{% alert color="primary" %}}

Saiba mais sobre [Aspose.Words para C++ 25.1 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-1-release-notes/).

Saiba mais sobre [Aspose.Words para C++ 25.2 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-2-release-notes/).

{{% /alert %}}

## Aspose.Words para C++ 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 introduz group shape inserção e StructuredDocumentTag inserção via DocumentBuilder, melhora a renderização do gráfico radial com graduações, melhora as assinaturas digitais com XAdES-EPES suporte, adiciona Markdown reconhecimento de sublinhado e fornece acesso a separadores de notas de rodapé/notas de fim.

O Aspose.Words 24.10 apresenta um suporte melhorado de controlo ActiveX com criação de CommandButton, novo controlo de visibilidade de formas, capacidade de agrupar formas, exportação de Markdown melhorada para tabelas, formatação de gráficos para gráficos de pizza e donut, melhor manuseamento de codificação Big5 e suporte para fontes taiwanesas desatualizadas.

Aspose.Words 24.11 introduz o resumo de documentos com AI, opções de renderização aprimoradas, acesso aprimorado às propriedades do documento e legendas de controle ActiveX.

O Aspose.Words 24.12 apresenta um posicionamento de etiquetas de dados personalizável, tradução de texto com tecnologia de IA da Google, opções de limpeza de direct mail melhoradas e novas classes de processamento LowCode.

### AI - recursos alimentados

#### Resumo de documentos utilizando OpenAI e Google <sup>24.11</sup>

O suporte para sumarização de documentos usando modelos de linguagem generativa **OpenAI** e **Google** foi integrado adicionando o namespace [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) com seus membros públicos.

#### Tradução de texto utilizando os modelos de linguagem generativa do Google <sup>24/12</sup>

A capacidade de traduzir texto utilizando os modelos de linguagem generativa do Google foi implementada no Aspose.Words adicionando o método [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/ ) e a enumeração [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) para [Aspose.Words.AI](https://reference.aspose.com/ palavras/net/aspose.words.ai/) namespace.

### Código baixo <sup>24.12</sup>

Novas classes LowCode como [Comparer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/net/ aspose.words.lowcode/mailmerger/), [Substituidor](https://reference.aspose.com/words/net/aspose.words.lowcode/replacer/), [Divisor](https://reference.aspose. com/words/net/aspose.words.lowcode/splitter/) etc.

### Renderização e impressão

#### Graduações em gráficos radiais

A renderização de graduações em gráficos radiais foi implementada.

#### ActiveX Controlos do botão de comando <sup>24.10</sup>

A capacidade de criar controlos ActiveX CommandButton foi introduzida adicionando um novo método público [InsertForms2OleControl](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertforms2olecontrol/) e uma nova classe pública **Forms2OleControl**.

#### Controlar a visibilidade da forma <sup>24.10</sup>

Foi adicionada uma nova propriedade pública [Hidden](https://reference.aspose.com/words/cpp/aspose.words.drawing/shapebase/get_hidden/) para controlar a visibilidade das formas.

#### Alterações nos gráficos de pizza e de rosca <sup>24.10</sup>

Foram adicionadas várias novas propriedades públicas para formatar gráficos de pizza e de rosca.

#### Controlar a renderização das bordas do campo do formulário de escolha PDF <sup>24.11</sup>

Uma nova opção para controlar a renderização de PDF fronteiras de campo de formulário de escolha foi implementada adicionando uma nova opção pública [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/get_renderchoiceformfieldborder/).

#### Obter e definir códigos de formato para dados do Gráfico <sup>24.11</sup>

A capacidade de obter e definir códigos de formato para dados de gráfico foi adicionada implementando a propriedade [FormatCode](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/bubblesizecollection/get_formatcode/) nas classes [ChartXValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartyvaluecollection/) e [BubbleSizeCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/bubblesizecollection/).

#### Renderizar gráficos de histograma com caixas e rótulos <sup>24.11</sup>

A renderização do Gráfico de histograma foi melhorada, permitindo um número especificado de caixas e rótulos.

#### Personalizar o posicionamento dos rótulos de dados <sup>24.12</sup>

A capacidade de personalizar o posicionamento dos rótulos de dados foi adicionada com a introdução de novas propriedades ao [ChartDataLabel](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabel/) e [ ChartDataLabelCollection ](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/) classes.

### Converter, carregar e guardar documentos

#### Sublinhar a formatação ao carregar ficheiros Markdown

A opção de reconhecer a formatação de sublinhado ao carregar documentos Markdown foi incorporada adicionando uma nova propriedade pública **ImportUnderlineFormatting**.

#### Exportar tabelas como HTML ao guardar no Markdown <sup>24.10</sup>

Uma opção para exportar tabelas como HTML ao guardar documentos no formato Markdown foi implementada adicionando uma nova propriedade pública [ExportAsHtml](https://reference.aspose.com/words/net/aspose.words. saving/markdownsaveoptions/exportashtml/) e uma enumeração [MarkdownExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownexportashtml/).

#### Exportar PDF com estrutura lógica actualizada <sup>24.11</sup>

PDF a exportação foi melhorada através da inclusão de propriedades de título de tabela como PDF títulos de elementos de estrutura lógica.

### Mala direta e relatórios

#### Remover tabelas vazias durante a correspondência em série <sup>24.12</sup>

Foi adicionada uma nova opção **RemoveEmptyTables** à enumeração [MailMergeCleanupOptions](https://reference.aspose.com/words/cpp/aspose.words.mailmerging/mailmergecleanupoptions/) para refinar a saída da mala direta.

### Assinaturas Digitais

#### Assinar documentos com XAdES-EPES

A capacidade de assinar documentos com XAdES-EPES Nível XML-DSig assinaturas foi introduzido adicionando uma nova propriedade pública **XmlDsigLevel** e uma nova enumeração pública **XmlDsigLevel**.

### Outros

* Um novo método público [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/) foi adicionado a group shapes.
* Um novo método público [InsertStructuredDocumentTag](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertstructureddocumenttag/) foi adicionado para inserir **StructuredDocumentTags** em um documento.
* O acesso público aos separadores de notas de rodapé/notas de fim foi proporcionado pela adição de algumas classes e propriedades públicas.
* A capacidade de agrupar formas individuais, agrupar formas e agrupar directamente formas e formas de grupo foi introduzida adicionando o método [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/). <sup>24.10</sup>
* O manuseamento da codificação Big5 para tabelas cmap TrueType foi melhorado. <sup>24.10</sup>
* O suporte para fontes desatualizadas de Taiwan foi melhorado. <sup>24.10</sup>
* Para acessar as propriedades do documento estendido, propriedades somente leitura foram adicionadas à classe [BuiltInDocumentProperties](https://reference.aspose.com/words/cpp/aspose.words.properties/builtindocumentproperties/). <sup>24.11</sup>
* A definição de legendas para controlos ActiveX foi activada adicionando um novo setter público à propriedade **Forms2OleControl.Caption**. <sup>24.11</sup>

{{% alert color="primary" %}}

Saiba mais sobre [Aspose.Words para C++ 24.9 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-9-release-notes/).

Saiba mais sobre [Aspose.Words para C++ 24.10 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-10-release-notes/).

Saiba mais sobre [Aspose.Words para C++ 24.11 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-11-release-notes/).

Saiba mais sobre [Aspose.Words para C++ 24.12 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words para C++ 24.5, 24.6, 24.7

Aspose.Words 24.5 expande as opções para assemblies, melhora os recursos de renderização e expande algumas outras opções.

Aspose.Words 24.6 melhora as opções de renderização, melhora a funcionalidade de pesquisa e comparação e expande vários outros recursos.

Aspose.Words 24.7 altera a forma como trabalha com ActiveX, expande as capacidades de renderização, bem como exporta para os formatos Markdown e XLSX.

### Formatos Suportados

A partir da versão 24.7, a exportação para PDF/UA-2 é suportada para garantir a acessibilidade aos utilizadores com deficiência.

### Renderização e impressão

#### Alterações nos gráficos, formas e desenhos <sup>24.5</sup>

- A renderização de efeitos DrawingML para gráficos SVG, estendendo a funcionalidade anterior limitada a imagens, foi implementada.
- Foi introduzido o suporte para a criação de gráficos combinados e para o ajuste de propriedades, tais como a largura do intervalo, a sobreposição e a escala de bolhas nos grupos de séries, adicionando-se as classes **ChartSeriesGroup** e **ChartSeriesGroupCollection** e a propriedade **SeriesGroups**.
- A funcionalidade para manipular o efeito SoftEdge das formas foi implementada adicionando a classe **SoftEdgeFormat**.
- A capacidade de modificar ajustar valores de formas foi implementada adicionando as classes públicas **AdjustmentCollection** e **Adjustment** e a propriedade **Adjustments**.

#### Alterações nos gráficos, formas e desenhos <sup>24.6</sup>

- As capacidades de gráficos foram melhoradas. Agora você pode criar uma variedade maior de gráficos, incluindo *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* gráficos, *Box & Whisker* gráficos, *Waterfalls* e *Funnels*. Isto permite-lhe visualizar os seus dados de uma forma mais diversificada e informativa.
- O controlo das cores para a formatação das Sombras foi melhorado. Você pode obter um controle mais preciso sobre a aparência de seus documentos acessando cores de sombra.
- O aumento de desempenho para a renderização em segundo plano foi melhorado. Você pode acelerar significativamente a renderização de fundos contendo pequenos elementos graças à tecnologia nativa de ladrilhos.
- Foram adicionados gradientes realistas para formas. Agora você pode criar DML formas com gradientes não lineares, imitando o estilo visual de Microsoft Word para uma aparência mais polida.

#### Personalização Do Rótulo Dos Dados Do Gráfico <sup>24.7</sup>

Foi adicionada a capacidade de personalizar rótulos de dados do gráfico, como **Orientation** e **Rotation**.

#### Estilo De Número personalizado para níveis de Lista <sup>24.7</sup>

Foi adicionado um setter para a propriedade pública [CustomNumberStyleFormat](https://reference.aspose.com/words/cpp/aspose.words.lists/listlevel/get_customnumberstyleformat/). Agora você pode definir um estilo de número personalizado para níveis de lista.

#### Mudanças no trabalho com ActiveX <sup>24.7</sup>

- As propriedades dos objetos ActiveX agora podem ser modificadas, dando a você mais controle sobre seu comportamento.
- Foi adicionada a capacidade de modificar o valor do controlo ActiveX do botão de opção para permitir a interacção dinâmica.
- A capacidade de alternar uma caixa de seleção ActiveX para "marcada" ou "desmarcada" foi adicionada.

### Carregar e guardar documentos

#### Exportando Links para o formato Markdown <sup>24.7</sup>

A capacidade de controlar a exportação de links no formato Markdown foi adicionada através da implementação da propriedade [LinkExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_linkexportmode/).

### Pesquisar e comparar

#### Opções Avançadas De Comparação <sup>24.6</sup>

Foi adicionada a capacidade de simplificar os fluxos de trabalho de análise de dados com uma funcionalidade de comparação melhorada. Isso inclui uma nova opção **IgnoreStoreItemId** e uma interface redesenhada para comparações avançadas.

### Outros

- A função para eliminar páginas vazias de um documento foi implementada adicionando o método [RemoveBlankPages](https://reference.aspose.com/words/cpp/aspose.words/document/removeblankpages/). <sup>24.5</sup>
- A capacidade de verificar a presença de VBA macros sem carregar um documento foi fornecida adicionando a propriedade **HasMacros**. <sup>24.5</sup>
- Uma nova propriedade **DateTimeUtc** foi adicionada-isto fornece um carimbo de data / hora mais preciso para os comentários, melhorando a organização e a rastreabilidade. <sup>24.6</sup>
- O formato datetime agora é detectado automaticamente para exportação contínua para o formato XLSX. <sup>24.7</sup>
- A propriedade pública [IsProtected](https://reference.aspose.com/words/cpp/aspose.words.vba/vbaproject/get_isprotected/), que permite verificar se um projeto VBA está protegido, foi adicionada. <sup>24.7</sup>

{{% alert color="primary" %}}

Saiba mais sobre [Aspose.Words para C++ 24.5 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-5-release-notes/).

Saiba mais sobre [Aspose.Words para C++ 24.6 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-6-release-notes/).

Saiba mais sobre [Aspose.Words para C++ 24.7 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-7-release-notes/).

{{% /alert %}}

## Aspose.Words Para C++ 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 melhora a experiência em torno do gerenciamento de cores de traços, aprimora OLE objetos, bem como introduz novas fontes bibliográficas public API.

Aspose.Words 24.2 gráficos expandidos API e gestão de estilos. Esta versão de Aspose.Words também introduziu a capacidade de especificar SvgSaveOptions durante a renderização, controle mais flexível Carregando Markdown arquivos e trabalhando com texto de referência para notas de rodapé e notas de fim.

Aspose.Words 24.3 introduz a emulação de operações de varredura binária para WMF metarquivos e também continua a expandir os gráficos API.

Aspose.Words 24.4 melhora algumas opções de renderização, bem como melhora o trabalho com assinaturas digitais.

### Renderização e impressão

#### Controlo Da Cor Do Traçado <sup>24.1</sup>

A classe [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) foi estendida com um conjunto de novas propriedades públicas relacionadas ao gerenciamento de cores de traçado: [ForeThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_forethemecolor/) e [BackThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_foretintandshade/) e [BackTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backtintandshade/).

#### DrawingML Charts API Extensão <sup>24.2 / 24.3 / 24.4</sup>

O **DrawingML Charts API** continua a ser expandido.

#### Incorporar fontes declaradas em @font-face Regras <sup>24.4</sup>

Adicionada a capacidade de incorporar fontes declaradas nas regras @font-face nas definições de fonte do documento resultante foi introduzida adicionando uma nova propriedade [SupportFontFaceRules](https://reference.aspose.com/words/cpp/aspose.words.loading/htmlloadoptions/get_supportfontfacerules/).

#### Trabalhar com formatação de brilho e reflexão <sup>24.4</sup>

A capacidade de trabalhar com formatação de brilho e reflexão para um objeto de desenho foi implementada.

### Carregar e guardar documentos

#### Especifique SvgSaveOptions Durante A Renderização <sup>24.2</sup>

A capacidade de especificar [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/) durante a renderização foi adicionada usando o [ShapeRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) e [OfficeMathRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) métodos.

#### Preservar linhas vazias ao carregar ficheiros Markdown <sup>24.2</sup>

A capacidade de preservar linhas vazias ao carregar arquivos Markdown foi adicionada.

### Outros

- A capacidade de modificar o texto do controlo `TextBox` OLE foi introduzida adicionando uma nova propriedade **Text** à nova classe **TextBoxControl**. <sup>24.1</sup>
- A bibliografia Sources public API foi implementada através da adição de um novo namespace [Aspose.Words.Bibliography](https://reference.aspose.com/words/cpp/aspose.words.bibliography/) com as suas novas classes e enumerações, e através da adição de uma nova propriedade [Bibliography](https://reference.aspose.com/words/cpp/aspose.words/document/get_bibliography/) à classe [Document](https://reference.aspose.com/words/cpp/aspose.words/document/). <sup>24.1</sup>
- Novas propriedades públicas [Priority](https://reference.aspose.com/words/cpp/aspose.words/style/get_priority/), [UnhideWhenUsed](https://reference.aspose.com/words/cpp/aspose.words/style/get_unhidewhenused/) e [SemiHidden](https://reference.aspose.com/words/cpp/aspose.words/style/get_semihidden/) para gerenciamento de estilo aprimorado foram adicionadas à classe [Style](https://reference.aspose.com/words/cpp/aspose.words/style/). <sup>24.2</sup>
- A funcionalidade para recuperar o texto real da marca de referência para notas de rodapé e notas de fim foi melhorada com a propriedade [ActualReferenceMark](https://reference.aspose.com/words/cpp/aspose.words.notes/footnote/get_actualreferencemark/) e o método [UpdateActualReferenceMarks](https://reference.aspose.com/words/cpp/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
- A emulação de operações de varredura binária para metarquivos WMF foi implementada. <sup>24.3</sup>
- A capacidade de definir opções de assinatura para documentos dentro de **SaveOptions** foi habilitada adicionando uma nova classe **DigitalSignatureDetails** com novos membros públicos, bem como adicionando novas propriedades às classes [OoxmlSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/docsaveoptions/) e [OdtSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

Saiba mais sobre [Aspose.Words para C++ 24.1 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-1-release-notes/).

Saiba mais sobre [Aspose.Words para C++ 24.2 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-2-release-notes/).

Saiba mais sobre [Aspose.Words para C++ 24.3 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-3-release-notes/).

Saiba mais sobre [Aspose.Words para C++ 24.4 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words Para C++ 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 expande as opções de renderização, emulação de renderização de metarquivo e opções de salvamento de markdown.

Aspose.Words 23.10 melhora a renderização, expande as opções para carregar e salvar documentos e permite que os usuários mesclem documentos de novas maneiras.

Aspose.Words 23.11 melhora o trabalho com revisões, XLSX formato e fontes na legenda do gráfico com opções adicionais.

Aspose.Words 23.12 introduz novas propriedades e enumerações para trabalhar com documentos PDF e OOXML, bem como suporte para imagens WebP.

### Renderização e impressão

#### Personalização de títulos de eixos em gráficos DrawingML <sup>23.9</sup>

A capacidade de personalizar títulos de eixos em gráficos DrawingML foi introduzida pela implementação de uma nova propriedade public class **ChartAxisTitle** e [Title](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartaxis/get_title/).

#### Determinação da posição Vertical das fontes num parágrafo <sup>23.9</sup>

Agora é possível definir a posição vertical das fontes dentro de um parágrafo usando a nova propriedade public [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/paragraphformat/get_baselinealignment/) e a nova enumeração [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/baselinealignment/).

#### Controlo Da Cor Do Primeiro Plano <sup>23.10</sup>

A capacidade de recuperar a cor de primeiro plano sem modificadores foi adicionada às classes [Fill](https://reference.aspose.com/words/cpp/aspose.words.drawing/fill/) e [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) através da propriedade **BaseForeColor**.

#### Expansão da funcionalidade dos gráficos <sup>23.10</sup>

A funcionalidade das classes [ChartDataPointCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartseries/) e [ChartFormat](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartformat/) foi expandida com novos métodos e propriedades.

#### Ajustar e ajustar automaticamente uma imagem numa forma <sup>23.10</sup>

Uma maneira simples de ajustar e ajustar automaticamente uma imagem dentro de uma forma específica foi fornecida através do novo método [FitImageToShape](https://reference.aspose.com/words/cpp/aspose.words.drawing/imagedata/fitimagetoshape/).

#### Formatação de fonte padrão para entradas de legenda de gráfico DrawingML <sup>23.11</sup>

A capacidade de especificar a formatação de fonte padrão para entradas de legenda de gráficos DrawingML foi adicionada através da propriedade [Font](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartlegend/get_font/). Este recurso facilita uma aparência mais simplificada e consistente para os elementos do gráfico, melhorando a estética geral do documento.

#### Especificar o Layout da Página ao Abrir PDF No Reader <sup>23.12</sup>

A capacidade de especificar o layout de página a ser usado ao abrir um documento em um leitor PDF foi adicionada através da introdução de uma nova propriedade **PageLayout** à classe [PdfSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/) e da introdução de uma nova enumeração **PdfPageLayout**.

### Carregar e guardar documentos

#### Especificando um nome de pasta para construir a imagem URIs em Markdown <sup>23.9</sup>

A classe [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) foi expandida incluindo a propriedade [ImagesFolderAlias](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imagesfolderalias/), que permite especificar o nome da pasta usada para construir a imagem URIs escrita no documento Markdown.

#### Reduzir PDF Tamanho Da Saída <sup>23.10</sup>

Várias otimizações de renderização PDF para reduzir o tamanho da saída ao utilizar as configurações [OptimizeOutput](https://reference.aspose.com/words/cpp/aspose.words.saving/fixedpagesaveoptions/get_optimizeoutput/) foram implementadas.

#### Reconhecer hiperligações ao carregar TXT documentos <sup>23.10</sup>

O recurso para reconhecer hiperlinks ao carregar documentos TXT foi implementado adicionando uma nova propriedade [DetectHyperlinks](https://reference.aspose.com/words/cpp/aspose.words.loading/txtloadoptions/get_detecthyperlinks/).

### Outros

- A emulação de renderização de metarquivo para determinar o tamanho da rasterização foi implementada, especificamente para WMF Largura da caneta e EMF Largura da caneta cosmética. Para isso, a propriedade **ScaleWmfFontsToMetafileSize** foi substituída pela propriedade [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpage/) e a propriedade [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpageresolution/) foi adicionada. <sup>23.9</sup>
* Foi introduzido um método simplificado para inserir um documento noutro documento na posição actual do cursor utilizando o método [InsertDocumentInline](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertdocumentinline/). <sup>23.10</sup>
* A capacidade de aceder e modificar propriedades de estilo foi adicionada através da introdução da nova propriedade [Locked](https://reference.aspose.com/words/cpp/aspose.words/style/get_locked/). <sup>23.10</sup>
* Um parâmetro de tipo genérico foi adicionado aos métodos da classe [CompositeNode](https://reference.aspose.com/words/cpp/aspose.words/compositenode/). <sup>23.10</sup>
* Uma forma de controlar quando uma determinada revisão deve ser aceite/rejeitada ou não foi implementada utilizando os métodos [Accept](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/accept/) e [Reject](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/reject/). Esta melhoria confere aos utilizadores um controlo mais rigoroso sobre o processo de revisão. <sup>23.11</sup>
* A capacidade de escrever todas as secções de um documento na mesma folha de cálculo XLSX foi fornecida através do novo tipo de enumeração [XlsxSectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsectionmode/) e da propriedade new [SectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsaveoptions/get_sectionmode/). <sup>23.11</sup>
* Uma maneira de controlar como as extensões de formato ZIP64 serão usadas para documentos OOXML foi implementada por meio da nova propriedade Zip64Mode da classe `OoxmlSaveOptions` e da nova enumeração Zip64Mode. <sup>23.12</sup>
* Foi introduzido o suporte para a imagem WebP. Observe que esse recurso está disponível apenas para .NetStandart E.NET6 + versões. <sup>23.12</sup>

{{% alert color="primary" %}}

Saiba mais sobre [Aspose.Words para C++ 23.9 Notas De Lançamento](/words/cpp/aspose-words-for-cpp-23-9-release-notes/).
Saiba mais sobre [Aspose.Words para C++ 23.10 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-10-release-notes/).
Saiba mais sobre [Aspose.Words para C++ 23.11 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-11-release-notes/).
Saiba mais sobre [Aspose.Words para C++ 23.12 Notas De Lançamento](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-12-release-notes/).

{{% /alert %}}

## Ver Também

{{% alert color="primary" %}}

Esta página contém as últimas notícias de lançamento dos últimos 2 anos. Para obter detalhes sobre versões anteriores, consulte o [Notas De Lançamento](/words/cpp/release-notes/) páginas nas secções relevantes.

{{% /alert %}}
