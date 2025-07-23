---
title: C#에서 워드를 PDF로 변환
second_title: Aspose.Words for .NET
articleTitle: 문서를 PDF로 변경
linktitle: 문서를 PDF로 변경
description: "C#에서 워드를 PDF로 변환. DOCX에서 PDF로 변환하는 간단한 코드 예제. 모든 워드 형식과 이미지를 지원합니다."
type: docs
weight: 10
url: /ko/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

문서를 한 형식에서 다른 형식으로 쉽고 안정적으로 변환하는 기능은 Aspose.Words의 핵심 기능입니다. PDF는 변환에서 가장 인기 있는 형식 중 하나입니다 – 다양한 플랫폼에서 렌더링할 때 문서의 원래 모양을 보존하는 고정 레이아웃 형식입니다. "렌더링"이라는 용어는 Aspose.Words에서 문서를 페이지로 나누어진 파일 형식이나 페이지 개념을 가진 파일 형식으로 변환하는 과정을 설명하는 데 사용됩니다.

## 워드 문서를 PDF로 변환

워드에서 PDF로의 변환은 여러 계산 단계가 필요한 상당히 복잡한 과정입니다. Aspose.Words 레이아웃 엔진은 Microsoft Word의 페이지 레이아웃 엔진의 작동 방식을 모방하여 PDF 출력 문서가 Microsoft Word에서 볼 수 있는 것과 최대한 유사하게 만듭니다.

Aspose.Words를 사용하면 Microsoft Office를 사용하지 않고도 DOC이나 DOCX와 같은 워드 형식에서 프로그래밍 방식으로 문서를 PDF로 변경할 수 있습니다. 이 문서에서는 이 변환을 수행하는 방법을 설명합니다.

{{% alert color="primary" %}}

문서의 페이지 수가 변환 시간에 영향을 미친다는 점에 주의하세요.

{{% /alert %}}

### DOCX 또는 DOC를 PDF로 변환

Aspose.Words에서 DOC 또는 DOCX 문서 형식을 PDF 형식으로 변경하는 것은 매우 간단하며 다음과 같은 두 줄의 코드로 수행할 수 있습니다:

1. 형식 확장자가 있는 문서 이름을 지정하여 생성자 중 하나를 사용해 문서를 [Document](https://reference.aspose.com/words/net/aspose.words/document/) 객체에 로드합니다.
1. **Document** 객체에서 [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) 메서드 중 하나를 호출하고 ".PDF" 확장자를 가진 파일 이름을 입력하여 원하는 출력 형식을 PDF로 지정합니다.

다음 코드 예제는 [Save](https://reference.aspose.com/words/net/aspose.words/document/save/) 메서드를 사용하여 문서를 DOCX에서 PDF로 변환하는 방법을 보여줍니다:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

이 예제의 템플릿 파일은 [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx)에서 다운로드할 수 있습니다.

{{% alert color="primary" %}}

때로는 문서를 PDF로 저장하는 결과에 영향을 줄 수 있는 추가 옵션을 지정해야 할 수도 있습니다. 이러한 옵션은 PDF 출력이 어떻게 표시될지 결정하는 속성을 포함하는 [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) 클래스를 사용하여 지정할 수 있습니다.

같은 기술로 흐름 레이아웃 형식의 모든 문서를 PDF 형식으로 전환할 수 있다는 점에 주의하세요.

{{% /alert %}}

### 다양한 PDF 표준으로 변환

Aspose.Words는 DOC 또는 DOCX를 다양한 PDF 형식 표준(PDF 1.7, PDF 1.5 등)으로 변환하는 것을 지원하는 [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) 열거형을 제공합니다.

다음 코드 예제는 PDF17 규격을 준수하는 [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)를 사용하여 문서를 PDF 1.7로 변환하는 방법을 보여줍니다:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## 이미지를 PDF로 변환

PDF로의 변환은 Microsoft Word 문서 형식에 국한되지 않습니다. 프로그래밍 방식으로 생성된 것을 포함하여 Aspose.Words에서 지원하는 모든 형식도 PDF로 전환할 수 있습니다. 예를 들어, JPEG, PNG, BMP, EMF, WMF와 같은 단일 페이지 이미지뿐만 아니라 TIFF, GIF와 같은 다중 페이지 이미지도 PDF로 변환할 수 있습니다.

다음 코드 예제는 JPEG 및 TIFF 이미지를 PDF로 변경하는 방법을 보여줍니다:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

이 코드가 작동하려면 프로젝트에 Aspose.Words 및 `System.Drawing`에 대한 참조를 추가해야 합니다.

## PDF 출력 크기 줄이기

PDF로 저장할 때 출력을 최적화할지 여부를 지정할 수 있습니다. 이를 위해 [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) 플래그를 true로 설정해야 하며, 그러면 중복되는 중첩된 빈 캔버스가 제거되고 동일한 서식을 가진 인접한 문자가 연결됩니다.

다음 코드 예제는 출력을 최적화하는 방법을 보여줍니다:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

**OptimizeOutput** 속성을 사용하면 콘텐츠 표시의 정확도에 영향을 줄 수 있습니다.

{{% /alert %}}

## 참고 항목

- [렌더링](/words/ko/net/rendering/) 문서에서 고정 페이지 및 흐름 레이아웃 형식에 대한 자세한 정보
- [고정 페이지 형식으로 변환](/words/ko/net/converting-to-fixed-page-format/#what-is-a-page-layout) 문서에서 페이지 레이아웃에 대한 자세한 정보
- [PDF로 변환할 때 렌더링 옵션 지정](/words/ko/net/specify-rendering-options-when-converting-to-pdf/) 문서에서 `PdfSaveOptions` 클래스 사용에 대한 자세한 정보
- [PDF/A 및 PDF/UA로의 변환 기능 알아보기](/words/ko/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) 문서에서 Aspose.Words가 지원하는 PDF 표준 및 PDF 표준의 관련 ISO에 대한 설명
- [어떤 PDF 표준을 선택하는 것이 좋은지](/words/ko/net/which-pdf-standard-is-better-to-choose/) 문서에서 어떤 PDF 표준이 어떤 경우에 적합한지 결정하는 방법

- [PDF/A 또는 PDF/UA로 작업](/words/ko/net/working-with-pdfa-or-pdfua/) 문서에서 PDF/A 및 PDF/UA 형식의 문서 콘텐츠 요구사항 설명 - 주로 구조 및 글꼴 요구사항

- [PDF/A 및 PDF/UA로 저장할 때 접근성 문제 경고](/words/ko/net/warnings-when-saving-to-pdfa-and-pdfua/) 문서에서 PDF/A 및 PDF/UA가 부과하는 콘텐츠 접근성 요구사항 설명
