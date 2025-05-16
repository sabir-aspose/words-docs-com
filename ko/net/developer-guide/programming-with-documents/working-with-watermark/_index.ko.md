---
title: C#의 워터마크 작업
second_title: Aspose.Words.NET
articleTitle: 워터마크 작업
linktitle: 워터마크 작업
description: "C#을 사용한 문서 워터마크 조작."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ko/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

이 항목에서는Aspose.Words을 사용하여 워터마크로 프로그래밍 방식으로 작업하는 방법에 대해 설명합니다. 워터마크는 문서의 텍스트 뒤에 표시되는 배경 이미지입니다. 워터마크는[Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/)클래스로 표시되는 텍스트나 이미지를 포함할 수 있습니다.

{{% alert color="primary" %}}

**온라인 시도**

당신은 우리의 이 기능을 시도할 수 있습니다 [무료 온라인 문서 워터 마크](https://products.aspose.app/words/watermark).

{{% /alert %}}

## 문서에 워터마크 추가

Microsoft Word에서 워터마크 삽입 명령을 사용하여 문서에 워터마크를 쉽게 삽입할 수 있습니다. Aspose.Words는 문서에서 워터마크를 추가하거나 제거할[watermark](https://reference.aspose.com/words/net/aspose.words/watermark/)클래스를 제공합니다. Aspose.Words는 사용할 수 있는 세 가지 유형의 워터마크(텍스트,이미지 및 없음)를 정의하는[WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)열거형을 제공합니다.

### 텍스트 워터마크 추가

다음 코드 예제에서는[SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext)메서드를 사용하여[TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/)을 정의하여 문서에 텍스트 워터마크를 삽입하는 방법을 보여 줍니다:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### 이미지 워터마크 추가

다음 코드 예제에서는[SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage)메서드를 사용하여[ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/)을 정의하여 문서에 이미지 워터마크를 삽입하는 방법을 보여 줍니다:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

이미지 워터 마크는 이미지,문자열 또는 스트림으로 삽입 할 수 있습니다.

워터 마크는 또한 모양 클래스를 사용하여 삽입 할 수 있습니다. 머리글이나 바닥 글에 어떤 모양이나 이미지를 삽입하여 상상할 수있는 유형의 워터 마크를 만드는 것은 매우 쉽습니다.

다음 코드 예제에서는Word문서에 워터마크를 삽입합니다:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

이 예제의 샘플 파일은 다음에서 다운로드할 수 있습니다 [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## 문서에서 워터마크 제거

[Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/)클래스는 문서에서 워터마크를 제거하는 제거 방법을 제공합니다.

다음 코드 예제에서는 문서에서 워터마크를 제거하는 방법을 보여 줍니다:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

워터 마크가[Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/)클래스 객체를 사용하여 추가 된 경우 다음 삽입하는 동안 워터 마크 모양의 이름을 설정 한 다음 할당 된 이름으로 워터 마크 모양을 제거해야 문서에서 워터 마크를 제거합니다.

다음 코드 예제에서는 워터마크 모양의 이름을 설정하고 문서에서 제거하는 방법을 보여 줍니다:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## 테이블 셀에 워터마크 추가

때때로 당신은 테이블의 셀에 워터 마크/이미지를 삽입하고 테이블 외부에 표시해야,당신은[IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/)속성을 사용할 수 있습니다. 이 속성은 셰이프가 테이블 내부 또는 테이블 외부에 표시되는지 여부를 나타내는 플래그를 가져오거나 설정합니다. 이 속성은[OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/)방법을 사용하여Microsoft Word2010 에 대한 문서를 최적화할 때만 작동합니다.

다음 코드 예제에서는 이 속성을 사용하는 방법을 보여 줍니다:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
