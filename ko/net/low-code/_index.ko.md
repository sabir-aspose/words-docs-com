---
title: Low Code
second_title: Aspose.Words.NET
articleTitle: LowCodeAPI을 사용하여 문서 작업
linktitle: Low Code
type: docs
description: "Low CodeAPI을 사용하여 비교,변환,분할,병합,찾기 및 바꾸기와 같은 문서 처리 작업을 단순화합니다. Aspose.WordsLowCodeAPI깨끗한 구문,빠른 결과 및 최소한의 코딩 노력."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ko/net/low-code/
timestamp: 2025-04-22-07-08-55
---

.NET에 대한Aspose.Words은[Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/)네임스페이스를 제공하여 일반적인 문서 처리 작업을 단순화합니다. 이API은 문서 비교,콘텐츠 추출,이미지 변환 및 텍스트 교체와 같은 높은 수준의 작업을 최소한의 노력으로 수행하려는 개발자를 위해 설계되었습니다.

LowCodeAPI는 세분화된 제어보다 빠른 구현이 더 중요한 시나리오에 이상적입니다. .NET에 대한Aspose.Words의LowCode기능을 자세히 살펴 보겠습니다.

{{% alert color="primary" %}}

LowCodeAPI에서는 문서 구조를 변경할 수 없습니다.

{{% /alert %}}

## LowCodeAPI에서 사용 가능한 기능

`Aspose.Words.LowCode`네임스페이스는 현재 다음을 지원합니다:

* **Converting**한 형식에서 다른 형식으로 문서
* **Comparing**문서
* **Mail merging**
* **Reporting**LINQ구문 기반
* **Merging**문서
* **Search and replace**
* **Digital signing**문서
* **Splitting**다른 기준을 사용하여 부분으로 문서
* **watermark**추가

{{% alert color="primary" %}}

Low Code이외의 각 기능에 대한 자세한 설명은 개발자 가이드 섹션에서 찾을 수 있습니다.

{{% /alert %}}

## 유창하고 유창하지 않은API

.NET의Aspose.Words은 유창하고 유창하지 않은APIs를 모두 지원하므로 개발자가 코딩 기본 설정 및 프로젝트 요구에 가장 적합한 스타일을 선택할 수 있습니다. 이 두 가지 유형의API이 어떻게 다른지 보기 위해 몇 가지 예를 살펴보겠습니다.

{{% alert color="primary" %}}

유창한API에서는 컨텍스트(예:ComparerContext또는ReplacerContext)를 통해 작업을 구성하고 실행할 수 있습니다. 이 컨텍스트에는 공통 옵션이 포함되어 있습니다. 모든 관련 메소드가 일관된 구성으로 작동하도록 보장하여API를 강력하고 복잡한 시나리오에서 쉽게 관리 할 수 있습니다.

{{% /alert %}}

### 문서 비교

`LowCode`을 사용하여 두 개의Word문서를 비교하고 결과를 저장합니다.

**비 유창한 예:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**유창한 예:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

미세 조정 된 비교를 위해`CompareOptions`을 전달할 수도 있습니다.

**비 유창한 예:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

CompareOptions options = new CompareOptions
{
    IgnoreFormatting = true,
    IgnoreCaseChanges = true
};

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc, options);
{{< /highlight >}}

**유창한 예:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

ComparerContext comparerContext = new ComparerContext();
comparerContext.CompareOptions.IgnoreCaseChanges = true;

Comparer.Create(comparerContext)
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.3.docx")
   .Execute();
{{< /highlight >}}

### 문서를 이미지로 변환

`LowCode`을 사용하여Word문서를PDF로 변환합니다.

**비 유창한 예:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**유창한 예:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### 텍스트 찾기 및 바꾸기

`LowCode`을 사용하여 전체 문서에서 텍스트를 빠르게 바꿀 수 있습니다.

**비 유창한 예:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**유창한 예:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";

ReplacerContext replacerContext = new ReplacerContext();
replacerContext.SetReplacement("ReplaceMe", "Replacement");

Replacer.Create(replacerContext)
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

## Aspose.WordsLow Code을 사용하는 이유

**Aspose.Words.LowCode**네임스페이스는 깨끗하고 읽기 쉬운 구문으로 높은 수준의 문서 처리 작업을 빠르게 구현하는 데 도움이 됩니다. Word문서로 작업 할 때 속도,단순성 및 유지 관리 가능한 코드가 필요한 개발자에게 특히 유용합니다.

고급 옵션을 탐색하려면 항상LowCodeAPIs를 전체Aspose.Words개체 모델과 결합할 수 있습니다. [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/)에서 더 많은Low Code예제를 참조하십시오.