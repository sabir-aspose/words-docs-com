---
title: 다중 페이지 문서를Java의 이미지로 변환
second_title: Aspose.WordsJava
articleTitle: 여러 페이지 문서를 이미지로 변환
linktitle: 여러 페이지 문서를 이미지로 변환
type: docs
description: "여러 페이지 문서를 래스터 이미지로 내보내기(JPG, PNG, GIF, BMP, TIFF, WebP) Java를 사용한다."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ko/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Java의 경우Aspose.Words사용자가 여러 페이지 문서를 래스터 이미지로 내보낼 수 있습니다. 이것은 편집할 수 없는 용도로 문서의 미리보기,아카이브 또는 시각적 표현을 생성하는 데 유용할 수 있습니다.

## 다중 페이지 내보내기를 지원하는 형식은 무엇입니까?

Aspose.Words다음 래스터 이미지 형식으로 여러 페이지 내보내기를 지원합니다:

* 제페그
* 지프
* 페이지
* 비에
* 티프
* WebP

## 여러 페이지 문서를 이미지로 내보내는 방법

다중 페이지 문서를 이미지로 내보내는 기능은[MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/)클래스를 사용하여 구현됩니다.:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage)–지정된 페이지 중 첫 번째 페이지 만 저장
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float)-열 수를 지정하면서 페이지를 왼쪽에서 오른쪽 및 위에서 아래로 그리드로 정렬합니다
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float)-단일 출력에서 왼쪽에서 오른쪽으로 페이지를 수평으로 나란히 정렬합니다.
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float)-페이지를 하나의 출력으로 다른 페이지 아래에 세로로 정렬합니다.
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames)-각 페이지를 다중 프레임TIFF이미지에서 별도의 프레임으로 정렬하고TIFF이미지 형식에만 적용됩니다

다음 코드 예제에서는 다중 페이지DOCX문서를 가로 레이아웃으로JPEG이미지로 저장하는 방법을 보여 줍니다:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

출력 파일 페이지 모양([BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor),[BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor)및[BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth)지정)을 사용자 지정할 수도 있습니다.

다음 코드 예제에서는 다중 페이지DOCX문서를PNG이미지로 그리드 레이아웃으로 저장하는 방법을 보여 줍니다:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.PNG);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.setPageLayout(MultiPageLayout.grid(3, 10f, 10f));

// Customize the background and border.
options.getPageLayout().setBackColor(Color.lightGray);
options.getPageLayout().setBorderColor(Color.BLUE);
options.getPageLayout().setBorderWidth(2f);

doc.save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}