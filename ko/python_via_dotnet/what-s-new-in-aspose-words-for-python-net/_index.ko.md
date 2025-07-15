---
title: 새로운 기능
second_title: Python via .NET에 대한 Aspose.Words
articleTitle: Python via .NET에 대한Aspose.Words의 새로운 기능
linktitle: Python via .NET에 대한Aspose.Words의 새로운 기능
type: docs
description: "Python via .NET에 대한Aspose.Words은 매일 확장되고 향상됩니다. 이 페이지에서 제품의 거대하고 가장 흥미로운 기능에 대해 배울 수 있습니다."
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ko/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-06-23-21-02-49
---

이 페이지는 최근 릴리스에서 소개 된 가장 흥미로운 새로운Aspose.Words기능에 대해 설명합니다.

## Aspose.WordsPython via .NET25.5,25.6

Aspose.Words25.5 새로운 스타일 옵션을 사용하여 차트 사용자 정의를 향상시키고 빈 단락 처리 방법을 제어하여Markdown내보내기를 개선합니다.

Aspose.Words25.6 고급 이미지 내보내기 옵션,향상된MathML처리 및 더 나은 차트 표현을 도입하여 렌더링 정밀도 및 시각화 기능을 향상시킵니다.

### 문서 변환,로드 및 저장

#### 빈 단락을Markdown으로 내보내기 <sup>25.5</sup>

빈 단락을Markdown로 내보내는 방법을 제어하는 기능은**MarkdownEmptyParagraphExportMode**열거형과**empty_paragraph_export_mode**속성을 추가하여 도입되었습니다.

#### 여러 페이지 문서를 래스터 이미지 형식으로 내보내기 <sup>25.6</sup>

다중 페이지 문서를 래스터 이미지 형식(예:PNG및JPEG)으로[customizable layouts](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/)(수평,수직 또는 격자)으로 내보내는 기능은 이미지 내보내기 기능을 확장하여 도입되었습니다.

### 렌더링

#### 차트 스타일 설정 <sup>25.5</sup>

**ChartStyle**열거형과**style**속성을 추가하여 차트 스타일을 설정하는 기능이 도입되었습니다.

#### MathML식에서 커넥터 라인 렌더링 <sup>25.6</sup>

MathML식에서 커넥터 라인의 렌더링은 수학 공식의보다 정확하고 시각적으로 일관된 표시를 보장하기 위해 구현되었습니다.

#### 폭포 차트의 범례 렌더링 <sup>25.6</sup>

["Waterfall" charts](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriestype/)에 대한 범례 렌더링이 도입되어 데이터 투명성을 높이고 이러한 차트의 해석 가능성을 향상시킵니다.

### 다른

* 여러 슬래시가 포함된 수학 공식을 래핑하는 기능이 향상되어 레이아웃 선명도와 공식 가독성이 향상되었습니다. <sup>25.6</sup>

{{% alert color="primary" %}}

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET25.5 릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-5-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET25.6 릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words에 대한Python를 통해.NET 25.1, 25.2, 25.3, 25.4

Aspose.Words25.1AI전원 문법 검사를 도입하고HTML,SVG및Markdown형식에 대한 고급 옵션을 사용하여 문서 저장을 향상시킵니다.

Aspose.Words25.2는AnthropicAI모델로 텍스트 요약을 도입하고,MsWorks형식 지원을 추가하고,타이포그래피 제어를 향상시키고,PDF구조 및 목록 처리를 향상시킵니다.

Aspose.Words25.3는UpdateAmbiguousTextFont속성으로AI전원 문법 검사기 및 글꼴 선택을 향상시키고PDF첨부 파일 내보내기를 향상시킵니다.

Aspose.Words25.4새 용지 크기에 대한 지원을 도입하고 고급HTML내보내기 제어를 활성화하며 워터마크 처리를 개선합니다.

### AI-전원 기능

#### 문서AI문법 검사

* OpenAI생성 모델을 사용하여 제공된 문서의 문법을 확인하는 기능은 새로운[check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/)방법을 추가하여 도입되었습니다. <sup>25.1</sup>
* AI전원 문법 검사 기능은[AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/)열거형에서 사용할 수 있는 모든 모델을 지원하도록 업데이트되었습니다. <sup>25.3</sup>

#### Anthropic생성 언어 모델을 사용한 요약 <sup>25.2</sup>

Anthropic생성 언어 모델을 사용하는 텍스트 요약은 새로운 공용 클래스[AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/)을 도입하여 활성화되었습니다.

### 지원되는 형식 <sup>25.2</sup>

버전25.2에서 시작하여Microsoft작업 문서에 대한 새로운MsWorks로드 형식과의 호환성이 추가되었습니다.

### 문서 변환,로드 및 저장

#### HTML및SVG형식으로 저장 개선 <sup>25.1</sup>

[HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/)및[SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/)클래스 모두에**id_prefix**및**remove_java_script_from_links**속성을 추가하여HTML및SVG형식으로 저장하는 것이 향상되었습니다.

#### Markdown에 저장할 때 이미지 해상도 및OfficeMath출력 모드 설정 <sup>25.1</sup>

* [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)클래스에 새로운[image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/)옵션이 추가되어 이미지 해상도를 설정합니다.
* 새로운[office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/)옵션과[MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/)열거형이[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)클래스에 추가되어OfficeMath출력 모드를 설정합니다.

### 렌더링

#### 향상된 타이포그래피 제어 <sup>25.2</sup>

향상된 타이포그래피 제어를 위해[number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/)속성이 추가되었습니다.

#### 모호한 문자에 대한 글꼴 선택 제어 <sup>25.3</sup>

사용 된 문자 코드에 따라 글꼴 선택을 제어하기 위해[SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/)클래스에 새 공용 속성[update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/)이 추가되었습니다.

#### 용지 크기 옵션 <sup>25.4</sup>

[PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/)열거형에 새 값을 추가하여JISB4및JISB5용지 크기를 사용할 수 있는 기능이 도입되었습니다.

#### HTML출력 제어 <sup>25.4</sup>

HTML내보내기 중에 하이퍼링크URLs에서JavaScript을 제거하는 기능은[RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/)속성을 추가하여 도입되었습니다.

### 다른

* PDF논리 구조는TOA,BIBLIOGRAPHY및INDEX필드를 지원하여 개선되었습니다. <sup>25.2</sup>
* [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate)메서드는 향상된 목록 처리를 위해 도입되었습니다. <sup>25.2</sup>
* PDF첨부 파일의 내보내기를 개선하기 위해**EmbedAttachments**를 대체할 새 속성[attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/)이 추가되었습니다. 또한PDF/A버전 첨부 파일을 지원하기 위해[PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/)열거형에 새 값이 추가되었습니다. 또한 첨부 파일은 이제 암호화로 지원됩니다. <sup>25.3</sup>
* 스트림에서 이미지 워터마크를 설정하는 기능은[SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions)메서드에 새로운 오버로드를 추가하여 도입되었습니다. <sup>25.4</sup>

{{% alert color="primary" %}}

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET25.1릴리스 노트](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET25.2릴리스 노트](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET25.3릴리스 노트](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET25.4릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words에 대한Python를 통해.NET 24.9, 24.10, 24.11, 24.12

Aspose.Words24.9DocumentBuilder을 통한group shape삽입 및StructuredDocumentTag삽입을 도입하고,눈금으로 방사형 차트 렌더링을 향상시키고,XAdES-EPES지원을 통해 디지털 서명을 개선하고,Markdown밑줄 인식을 추가하고,각주/미주 구분 기호에 대한 액세스를 제공합니다.

Aspose.Words24.10CommandButton생성,새로운 모양 가시성 제어,group shapes기능,향상된Markdown테이블 내보내기,Pie및Doughnut차트에 대한 차트 서식 지정,더 나은 빅 5 인코딩 처리 및 오래된 대만 글꼴 지원을 통해 향상된ActiveX제어 지원을 소개합니다.

Aspose.Words24.11는AI전원이 공급되는 문서 요약,향상된 렌더링 옵션,문서 속성에 대한 향상된 액세스 및ActiveX제어 캡션을 소개합니다.

Aspose.Words24.12사용자 정의 데이터 레이블 배치,구글AI전원 텍스트 번역 및 향상된 새로운LowCode처리 클래스를 소개합니다.

### AI-전원 기능

#### OpenAI및 구글을 사용한 문서 요약 <sup>24.11</sup>

**OpenAI**및**Google**생성 언어 모델을 사용하는 문서 요약 지원은[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)네임스페이스를 공용 멤버와 추가하여 통합되었습니다.

#### 구글의 생성 언어 모델을 사용하여 텍스트 번역 <sup>24.12</sup>

구글의 생성 언어 모델을 사용하여 텍스트를 번역하는 기능은Aspose.Words에서[translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/)메소드와[Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/)열거를[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/)네임스페이스에 추가하여 구현되었습니다.

### Low Code <sup>24.12</sup>

같은 새로운LowCode클래스[Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) 그 밖의 문서 처리에 대한 단순성과 유연성 사이의 완벽한 균형을 이루는 일련의 방법을 제공하여 도입되었습니다.

### 렌더링 및 인쇄

#### 방사형 차트의 눈금 <sup>24.9</sup>

방사형 차트에 눈금의 렌더링이 구현되었습니다.

#### CommandButtonActiveX컨트롤 <sup>24.10</sup>

CommandButtonActiveX컨트롤을 만드는 기능은 새로운 공용 메서드[insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/)과 새로운 공용 클래스[Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/)을 추가하여 도입되었습니다.

#### 형상 가시성 제어 <sup>24.10</sup>

모양의 가시성을 제어하기 위해 새로운 공용 속성[hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/)이 추가되었습니다.

#### Pie및Doughnut차트의 변경 사항 <sup>24.10</sup>

Pie및Doughnut차트 형식에 몇 가지 새로운 공용 속성이 추가되었습니다.

#### PDF선택 양식 필드 테두리의 렌더링 제어 <sup>24.11</sup>

PDF선택 양식 필드 테두리의 렌더링을 제어하는 새로운 옵션이 새로운 공개 옵션[render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/)을 추가하여 구현되었습니다.

#### 차트 데이터에 대한 형식 코드 가져오기 및 설정 <sup>24.11</sup>

[ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/),[ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/)및[BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/)클래스에서[format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/)속성을 구현하여 차트 데이터에 대한 형식 코드를 가져오고 설정할 수 있는 기능이 추가되었습니다.

#### 빈 및 레이블이 있는 히스토그램 차트 렌더링 <sup>24.11</sup>

지정된 수의 빈과 레이블을 허용하여 히스토그램 차트 렌더링이 개선되었습니다.

#### 데이터 레이블 배치 사용자 지정 <sup>24.12</sup>

[ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/)및[ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/)클래스에 새 속성을 도입하여 데이터 레이블의 배치를 사용자 지정할 수 있는 기능이 추가되었습니다.

### 문서 변환,로드 및 저장

#### Markdown파일을 로드할 때 밑줄 서식 지정 <sup>24.9</sup>

Markdown문서를 로드할 때 밑줄 서식을 인식하는 옵션은 새 공용 속성[import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/)을 추가하여 통합되었습니다.

#### Markdown에 저장할 때 테이블을HTML로 내보내기 <sup>24.10</sup>

문서를Markdown형식으로 저장할 때 테이블을HTML로 내보내는 옵션은 새로운 공용 속성[export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/)과 열거형[MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/)을 추가하여 구현되었습니다.

#### 업데이트된 논리 구조로PDF내보내기 <sup>24.11</sup>

PDF내보내기는 테이블 제목 속성을PDF논리 구조 요소 제목으로 포함하여 향상되었습니다.

### 디지털 서명

#### XAdES-EPES로 문서에 서명 <sup>24.9</sup>

XAdES-EPES레벨XML-DSig서명으로 문서에 서명하는 기능은 새로운 공용 속성[xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/)과 새로운 공용 열거[XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/)을 추가하여 도입되었습니다.

### 다른

* Group shapes에 새 공용 메서드[insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/)이 추가되었습니다. <sup>24.9</sup>
* **StructuredDocumentTags**을 문서에 삽입하기 위한 새로운 공용 메서드[insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/)이 추가되었습니다. <sup>24.9</sup>
* 각주/미주 구분 기호에 대한 공개 액세스는 몇 가지 공개 클래스 및 속성을 추가하여 제공되었습니다. <sup>24.9</sup>
* 개별 모양을 그룹화하고,group shapes을 함께 그룹화하고,두 모양과group shapes을 직접 그룹화하는 기능은[insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist)방법을 추가하여 도입되었습니다. <sup>24.10</sup>
* TrueType에 대한 빅 5 인코딩 처리가 개선되었습니다. <sup>24.10</sup>
* 오래된 대만 글꼴에 대한 지원이 향상되었습니다. <sup>24.10</sup>
* 확장 문서 속성에 액세스하려면 읽기 전용 속성이[BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/)클래스에 추가되었습니다. <sup>24.11</sup>
* [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/)속성에 새 공용 세터를 추가하여ActiveX컨트롤에 대한 캡션 설정이 활성화되었습니다. <sup>24.11</sup>

{{% alert color="primary" %}}

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.9릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.10릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.11릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.12릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words에 대한Python를 통해.NET 24.5, 24.6, 24.7, 24.8

Aspose.Words24.5어셈블리에 대한 옵션을 확장하고 렌더링 기능을 개선하며 일부 다른 옵션을 확장합니다.

Aspose.Words24.6렌더링 옵션을 개선하고 검색 및 비교 기능을 향상시키며 다른 여러 기능을 확장합니다.

Aspose.Words24.7ActiveX작업 방식을 변경하고 렌더링 기능을 확장하며Markdown및XLSX형식으로 내보냅니다.

Aspose.Words24.8축 레이블을 정밀하게 제어하여 차트 사용자 정의를 강화하고 글꼴 관리를 확장하며 문서 구조 처리를 개선하고HTML/XAML내보내기,PDF기능,문서 변환 및 디지털 서명을 위한 새로운 기능을 추가합니다.

### 지원되는 형식

버전24.7부터PDF/UA-2으로 내보내기를 지원하여 장애가 있는 사용자의 접근성을 보장합니다.

### 렌더링 및 인쇄

#### 차트,도형 및DrawingML의 변경 사항 <sup>24.5</sup>

* SVG그래픽에 대한DrawingML효과 렌더링,이미지로 제한된 이전 기능 확장,구현되었습니다.
* [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/)및[ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/)클래스와[series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/)속성을 추가하여 콤보 차트를 만들고 계열 그룹 내에서 간격 너비,겹침 및 거품 배율과 같은 속성을 조정하는 데 대한 지원이 도입되었습니다.
* [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/)클래스를 추가하여 도형의SoftEdge효과를 조작하는 기능이 구현되었습니다.
* 도형의 조정 값을 수정하는 기능은**AdjustmentCollection**및**Adjustment**공용 클래스와[adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/)속성을 추가하여 구현되었습니다.

#### 차트,도형 및 도면의 변화 <sup>24.6</sup>

- 차트 기능이 향상되었습니다. 이제 다음을 포함하여 더 다양한 차트를 만들 수 있습니다*Treemaps*, *Sunbursts*, *Histograms*, *Pareto* 차트,*Box & Whisker*차트,*Waterfalls*및*Funnels*. 이것은 당신이 더 다양하고 유익한 방법으로 데이터를 시각화 할 수 있습니다.
- 그림자 서식에 대한 색상 제어가 개선되었습니다. 그림자 색상에 액세스하여 문서의 모양을 보다 정확하게 제어할 수 있습니다.
- 배경 렌더링에 대한 성능 향상이 향상되었습니다. 기본 타일링 기술 덕분에 작은 요소가 포함 된 배경의 렌더링 속도를 크게 높일 수 있습니다.
- 모양에 대한 현실적인 그라디언트가 추가되었습니다. 이제 더 세련된 모양을 위해Microsoft Word의 시각적 스타일을 모방하여 비선형 그라디언트로DML도형을 만들 수 있습니다.

#### 차트 데이터 레이블 사용자 정의 <sup>24.7</sup>

**Orientation**및**Rotation**과 같은 차트 데이터 레이블을 사용자 지정할 수 있는 기능이 추가되었습니다.

#### 목록 수준에 대한 사용자 지정 번호 스타일링 <sup>24.7</sup>

공용 재산[custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/)에 대한 세터가 추가되었습니다. 이제 목록 수준에 대한 사용자 지정 숫자 스타일을 정의할 수 있습니다.

#### ActiveX작업 변경 <sup>24.7</sup>

- 이제ActiveX개체의 속성을 수정할 수 있으므로 동작을 더 잘 제어할 수 있습니다.
- 동적 상호 작용을 활성화하기 위해 라디오 버튼ActiveX컨트롤의 값을 수정하는 기능이 추가되었습니다.
- ActiveXcheckbox을"선택됨"또는"선택 취소됨"으로 전환할 수 있는 기능이 추가되었습니다.

#### 차트 축 눈금 레이블 방향 및 회전 제어 <sup>24.8</sup>

차트 축 눈금 레이블의 방향과 회전에 대한 정밀한 제어 기능이 추가되어 차트를 더욱 편리하게 사용자 지정할 수 있습니다. [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) 클래스가 새로운 [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) 및 [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/) 속성으로 확장되었습니다.

#### 백슬래시를 엔 기호로 바꾸기 <sup>24.8</sup>

백슬래시 문자를 엔 기호로 바꾸기 위한 역 호환HTML및XAML내보내기가 개선되었습니다. 이를 위해**replace_backslash_with_yen_sign**속성이[HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/)및[XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/)클래스에 추가되었습니다.

#### PDF로 내보낼 때SDT태그를 양식 필드 이름으로 사용 <sup>24.8</sup>

[PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/)클래스에 새[use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/)속성을 추가하여SDT태그를 양식 필드 이름으로 사용하기 위한 지원이 포함된PDF내보내기 기능이 향상되었습니다.

### 문서 변환,로드 및 저장

#### Markdown형식으로 링크 내보내기 <sup>24.7</sup>

[link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/)속성의 구현을 통해Markdown형식의 링크 내보내기를 제어하는 기능이 추가되었습니다.

#### LowCode 24.8 <sup>24.8</sup>

한 줄의 코드로 다양한 문서 유형을 변환하는 일련의 방법을 제공하도록 설계된 새로운[LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/)클래스가 도입되었습니다.

### 검색 및 비교

#### 고급 비교 옵션 <sup>24.6</sup>

향상된 비교 기능으로 데이터 분석 워크플로를 간소화할 수 있는 기능이 추가되었습니다. 여기에는 새로운[ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/)옵션과 고급 비교를 위한 재설계된 인터페이스가 포함됩니다.

### 다른

* 문서에서 빈 페이지를 제거하는 기능은[remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/)방법을 추가하여 구현되었습니다. <sup>24.5</sup>
* [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/)속성을 추가하여 문서를 로드하지 않고VBA매크로가 있는지 확인할 수 있습니다. <sup>24.5</sup>
* LINQ보고 엔진을 사용하여 문서를 삽입하는 동안 소스 번호 매기기를 유지하는 것이 지원됩니다. <sup>24.5</sup>
* 새로운[date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/)속성이 추가되었습니다.이 속성은 주석에 대한 보다 정확한 타임스탬프를 제공하여 조직 및 추적성을 향상시킵니다. <sup>24.6</sup>
* 이제XLSX형식으로 원활한 내보내기를 위해 날짜/시간 형식이 자동으로 감지됩니다. <sup>24.7</sup>
* VBA프로젝트가 보호되는지 여부를 확인할 수 있는 공용 속성[is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/)이 추가되었습니다. <sup>24.7</sup>
* 글꼴 정보는[FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/)및[PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/)클래스에 추가된**embedding_licensing_rights**속성으로 확장되었습니다. <sup>24.8</sup>
* 워터마크를 보존하면서 섹션 머리글과 바닥글을 효율적으로 지우는 방법이 문서 구조를 더 정확하게 작업하기 위해 추가되었습니다. 섹션 머리글과 바닥글을 지우려면 새 공용 메서드[clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default)을 사용합니다. <sup>24.8</sup>
* [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/)을 사용하여 XPS 문서의 디지털 서명이 활성화되었습니다. 이 목적을 위해 새 속성 [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/)이 추가되었습니다. <sup>24.8</sup>

{{% alert color="primary" %}}

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.5릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.6릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.7릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.8릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words에 대한Python를 통해.NET 24.1, 24.2, 24.3, 24.4

Aspose.Words24.1는 획 색상 관리 환경을 개선하고OLE개체를 향상시키며 새로운`Bibliography Sources`공용API을 소개합니다.

Aspose.Words24.2확장된 차트API및 스타일 관리. 이 버전의Aspose.Words은 또한 렌더링 중에SvgSaveOptions을 지정할 수 있는 기능을 도입했으며,Markdown파일을 더 유연하게 제어하고,각주와 끝표에 대한 참조 텍스트를 작업했습니다.

Aspose.Words24.3는WMF메타파일에 대한 새로운TIFF리더/라이터와 바이너리 래스터 연산의 에뮬레이션을 소개합니다. Aspose.Words24.3도API차트를 계속 확장합니다.

Aspose.Words24.4은 저장 형식,일부 렌더링 옵션을 향상시키고 디지털 서명 작업을 향상시킵니다.

### 지원되는 형식 <sup>24.4</sup>

현대**WebP**이미지 형식은 이제.NET Framework 4.6.2이상에 대해Aspose.Words에서 지원됩니다. 이제WebP이미지를 문서에 읽고 삽입할 수 있으며WebP형식으로 이미지를 저장할 수 있습니다.

WebP는 현재.NET Standard및.NET Framework브이4.6.2이상에서만 사용할 수 있습니다.

### 렌더링 및 인쇄

#### 스트로크 색상 제어 <sup>24.1</sup>

[Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/)클래스는 획 색상 관리와 관련된 새로운 공용 속성 세트([fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/)및[back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/),[fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/)및[back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/))로 확장되었습니다.

#### DrawingML차트API확장 <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API**은 계속 확장되고 있습니다.

#### @font-face규칙에 선언된 글꼴 포함 <sup>24.4</sup>

추가 결과 문서의 글꼴 정의에@font-face규칙에 선언 된 글꼴을 포함 할 수있는 기능은 새로운[support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/)속성을 추가하여 도입되었습니다.

#### 글로우 및 반사 서식 지정 작업 <sup>24.4</sup>

도면 객체에 대한 빛과 반사 포맷으로 작업할 수 있는 기능이 구현되었습니다.

### 문서 로드 및 저장

#### 렌더링하는 동안SvgSaveOptions지정 <sup>24.2</sup>

렌더링 중에[SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/)을 지정하는 기능이[ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/)를 사용하여 추가되었습니다.[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions)과[OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/)[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions)방법.

#### Markdown파일을 로드할 때 빈 줄 유지 <sup>24.2</sup>

Markdown파일을로드 할 때 빈 줄을 유지하는 기능이 추가되었습니다.

#### 새로운TIFF독자/작가 <sup>24.3</sup>

Aspose.Words에 대한 새로운TIFF리더/라이터가 개발되었습니다. Aspose.Words.NET 24.3에 대한JPEG및 이전JPEG압축 유형의TIFF이미지 읽기에 대한 지원이 추가되었으며 읽기 및 쓰기 작업의 품질도 크게 향상되었습니다.

### 다른

* `TextBox`OLE컨트롤의 텍스트를 수정하는 기능은 새로운**TextBoxControl**클래스에 새로운**Text**속성을 추가하여 도입되었습니다. <sup>24.1</sup>
* 공개 문헌 자료API는 새로운 클래스와 열거를 가진 새로운 네임스페이스[Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/)을 추가하고,[Document](https://reference.aspose.com/words/python-net/aspose.words/document/)클래스에 새로운[bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/)속성을 추가함으로써 구현되었다. <sup>24.1</sup>
* 향상된 스타일 관리를 위한 새로운 공용 속성[priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/),[unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/)및[semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/)이[Style](https://reference.aspose.com/words/python-net/aspose.words/style/)클래스에 추가되었습니다. <sup>24.2</sup>
* [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/)속성과[update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default)메서드를 사용하여 각주 및 미주에 대한 실제 참조 마크 텍스트를 검색하는 기능이 향상되었습니다. <sup>24.2</sup>
* WMF메타파일에 대한 이진 래스터 연산의 에뮬레이션이 구현되었습니다. <sup>24.3</sup>
* **SaveOptions**내의 문서에 대한 서명 옵션을 정의하는 기능은 새 공용 멤버와 함께 새[DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/)클래스를 추가하고[OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/),[DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/)및[OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/)클래스에 새 속성을 추가하여 활성화되었습니다. <sup>24.4</sup>

{{% alert color="primary" %}}

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.1릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.2릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.3릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET24.4릴리스 노트](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words에 대한Python을 통해.NET 23.9, 23.10, 23.11, 23.12

Aspose.Words23.9렌더링 옵션,메타파일 렌더링 에뮬레이션 및markdown저장 옵션을 확장합니다.

Aspose.Words23.10렌더링을 개선하고 문서 로드 및 저장 옵션을 확장하며 사용자가 새로운 방식으로 문서를 병합할 수 있도록 합니다.

Aspose.Words23.11추가 옵션을 사용하여 차트 범례의 개정판,XLSX형식 및 글꼴 작업을 향상시킵니다.

Aspose.Words23.12는PDF및OOXML문서 작업을 위한 새로운 속성과 열거를 소개하고WebP이미지를 지원합니다.

### 렌더링 및 인쇄

#### DrawingML차트에서 축 제목 사용자 지정 <sup>23.9</sup>

DrawingML차트에서 축 제목을 사용자 지정할 수 있는 기능은 새로운 공용 클래스[ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/)및[title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/)속성을 구현하여 도입되었습니다.

####  단락 내의 글꼴의 세로 위치 결정 <sup>23.9</sup>

이제 새 공용[baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/)속성과 새[BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/)열거형을 사용하여 단락 내의 글꼴의 세로 위치를 정의할 수 있습니다.

#### 전경색 제어 <sup>23.10</sup>

수정자 없이 전경색을 검색할 수 있는 기능이**BaseForeColor**속성을 통해[Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/)및[Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/)클래스에 추가되었습니다.

#### 차트의 기능 확장 <sup>23.10</sup>

[ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/),[ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/)및[ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/)클래스의 기능이 새로운 메서드 및 속성으로 확장되었습니다.

#### 이미지 자동 조정 및 모양에 맞추기 <sup>23.10</sup>

새로운[fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default)방법을 통해 특정 모양 내에서 이미지를 자동으로 조정하고 맞추는 간단한 방법이 제공되었습니다.

#### DrawingML차트 범례 항목의 기본 글꼴 서식 지정 <sup>23.11</sup>

[font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/)속성을 통해DrawingML차트의 범례 항목에 대한 기본 글꼴 서식을 지정하는 기능이 추가되었습니다. 이 기능은 전체 문서 미학을 개선,차트 요소에 대한보다 능률적이고 일관된 모양을 용이하게한다.

#### 리더에서PDF을 열 때 페이지 레이아웃 지정 <sup>23.12</sup>

PDF리더에서 문서를 열 때 사용할 페이지 레이아웃을 지정하는 기능은[PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/)클래스에 새로운[page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/)속성을 도입하고 새로운[PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/)열거형을 도입하여 추가되었습니다.

### 문서 로드 및 저장

#### Markdown에서 이미지URIs를 구성하는 폴더 이름 지정 <sup>23.9</sup>

[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)클래스는[images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/)속성을 포함하여 확장되었으며,Markdown문서에 작성된 이미지URIs를 구성하는 데 사용되는 폴더의 이름을 지정할 수 있습니다.

#### PDF출력 크기 줄이기 <sup>23.10</sup>

[optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/)설정을 사용할 때 출력 크기를 줄이기 위해 다양한PDF렌더링 최적화가 구현되었습니다.

#### TXT문서를 로드할 때 하이퍼링크 인식 <sup>23.10</sup>

TXT문서를 로드할 때 하이퍼링크를 인식하는 기능은 새로운[detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/)속성을 추가하여 구현되었습니다.

### 다른

- 특히WMF펜 너비와EMF화장품 펜 너비에 대해 래스터화 크기를 결정하기 위한 메타파일 렌더링 에뮬레이션이 구현되었습니다. 이를 위해**ScaleWmfFontsToMetafileSize**속성이[emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/)속성으로 대체되고[emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/)속성이 추가되었습니다. <sup>23.9</sup>
- [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions)방법을 사용하여 현재 커서 위치에서 한 문서를 다른 문서에 삽입하는 간단한 방법이 도입되었습니다. <sup>23.10</sup>
- 새로운[locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/)속성을 도입하여 스타일 속성에 액세스하고 수정할 수 있는 기능이 추가되었습니다. <sup>23.10</sup>
- [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/)클래스의 메서드에 제네릭 형식 매개 변수가 추가되었습니다. <sup>23.10</sup>
- 동일한XLSX워크시트에 문서의 모든 섹션을 쓸 수 있는 기능은 새[XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/)열거형 유형과 새[section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/)속성을 통해 제공되었습니다. <sup>23.11</sup>
* ZIP64형식 확장이OOXML문서에 사용되는 방법을 제어하는 방법은`OoxmlSaveOptions`클래스의 새 압축 64 모드 속성과 새 압축 64 모드 열거를 통해 구현되었습니다. <sup>23.12</sup>
* WebP이미지에 대한 지원이 도입되었습니다. 이 기능은 만 사용할 수 있습니다.NetStandart및.NET6+버전. <sup>23.12</sup>

{{% alert color="primary" %}}

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET23.9릴리스 노트](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET23.10릴리스 노트](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET23.11릴리스 노트](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

에 대해 자세히 알아보기 [Aspose.Words.NET 23.12릴리스 노트](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words에 대한Python를 통해.NET 23.5, 23.6, 23.7, 23.8

Aspose.Words23.5차트 시리즈 데이터 및ODT문서와 함께 작업 할 수있는 기능뿐만 아니라 머리글/바닥 글 및 텍스트 줄 바꿈을 개선 할 수있는 기능을 향상시킬 수 있습니다.

Aspose.Words23.6렌더링 옵션을 확장하고 새 내보내기 형식을 추가하고LINQ보고 및LowCode도구를 개선합니다.

Aspose.Words23.7보고 기능을 향상시키고 새 내보내기 형식을 추가하며 테이블 및 디지털 서명 작업에 대한 변경 사항을 소개합니다.

Aspose.Words23.8는 다양한 형식의 기능을 확장하고 렌더링을 개선하며 필드 작업을 위한 새로운 옵션을 추가합니다.

### 지원되는 형식

* 버전23.6부터 문서를XLSX형식으로 저장할 수 있습니다. 지금 당신은 엑셀 형식으로 문서를 변환 할 수 있습니다. <sup>23.6</sup>

* 버전23.7부터 문서 페이지 또는 도형을EPS형식으로 저장할 수 있습니다. <sup>23.7</sup>

### 새로운 형식 기능

- MOBI문서에 대한 목차(TOC)를 자동으로 생성하는 기능이 도입되었습니다. <sup>23.8</sup>
- [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions)생성자는[PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions)로 확장되었습니다. <sup>23.8</sup>
- EMF메타파일에 대한 수직 텍스트의 모양이 구현되었습니다. <sup>23.8</sup>

### 렌더링

#### 차트 시리즈 데이터 가져오기 및 수정 <sup>23.5</sup>

차트 시리즈 데이터를 가져오고 수정하는 기능은 다음을 추가하여 제공되었습니다.:

- 새로운 클래스: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- 새 열거형 유형:[ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/),[ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### 고급 타이포그래피 지원 <sup>23.6</sup>

WMF,EMF및EMF+렌더링의 고급 타이포그래피 지원이 추가되었습니다.

#### 페이지의 컬러 콘텐츠 <sup>23.6</sup>

페이지의 색상이 지정되었는지 여부를 나타내는 공용 속성[PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/)이 추가되었습니다.

#### 차트 데이터 레이블 서식 지정 <sup>23.6</sup>

차트 데이터 레이블에 대한 채우기,획 및 설명선 서식을 설정하는 기능이 구현되었습니다.

### Mail Merge및 보고

#### LINQ보고 엔진에 대한 동적HTML삽입 <sup>23.6</sup>

LINQ보고 엔진에 대한 동적HTML삽입의 새로운 방법이 추가되었습니다.

#### Mustache태그 지원 <sup>23.7</sup>

Mustache태그는 이제[MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/)및[MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/)메서드에서 지원됩니다.

#### 렌더링된 이미지의 크기 지정 <sup>23.8</sup>

렌더링된 이미지의 크기를 픽셀로 지정하기 위한 새로운 공용 속성[image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/)이 도입되었습니다.

#### JSON문자열 값–LINQ에 대한 공백 유지 <sup>23.8</sup>

LINQ보고 엔진에JSON문자열 값의 공백을 유지하는 옵션이 추가되었습니다.

### LowCode <sup>23.6</sup>

다른 유형의 문서를 단일 출력 문서로 병합하려는 새로운LowCode방법이 추가되었습니다.

### 다른

- 머리글/바닥글의 텍스트 줄 바꿈에 대한 지원이 구현되었습니다. <sup>23.5</sup>
- [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str)방법을 통해ODT문서에서 디지털 서명을 제거하는 기능이 추가되었습니다. <sup>23.5</sup>
- 음성 안내서[Run](https://reference.aspose.com/words/python-net/aspose.words/run/)의 기본 및 루비 텍스트를 얻기 위해 공공 재산[phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/)이 추가되었습니다. <sup>23.5</sup>
- 디지털 서명된 문서에서 바이트 배열로 디지털 서명 값을 검색하는 기능은 새로운[signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/)속성을 도입하여 추가되었습니다. <sup>23.7</sup>
- [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/)및[Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/)클래스는 새로운 공개 구성원으로 확장되었습니다.– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), 그리고[Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/) <sup>23.7</sup>

{{% alert color="primary" %}}

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET23.5릴리스 노트](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-5-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET23.6릴리스 노트](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-6-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET23.7릴리스 노트](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

에 대해 자세히 알아보기 [Aspose.WordsPython via .NET23.8릴리스 노트](/words/python-net/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## 또한 참조

{{% alert color="primary" %}}

이 페이지에는 지난 2 년간의 최신 릴리스 뉴스가 포함되어 있습니다. 이전 릴리스에 대한 자세한 내용은 [릴리스 노트'](https://releases.aspose.com/words/python/release-notes/) 관련 섹션의 페이지.

{{% /alert %}}
