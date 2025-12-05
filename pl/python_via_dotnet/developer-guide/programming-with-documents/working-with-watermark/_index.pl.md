---
title: Praca ze znakiem wodnym w Python
second_title: Aspose.Words dla Python via .NET
articleTitle: Praca ze znakiem wodnym
linktitle: Praca ze znakiem wodnym
description: "Tworzenie i zarządzanie znakami wodnymi w dokumencie za pomocą Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /pl/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

W tym temacie omówiono programową pracę ze znakiem wodnym przy użyciu Aspose.Words. Znak wodny to obraz tła wyświetlany za tekstem w dokumencie. Znak wodny może zawierać tekst lub obraz reprezentowany przez klasę [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Spróbuj online**

Możesz wypróbować tę funkcjonalność z naszym [Darmowy znak wodny dokumentu online](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Jak dodać Znak wodny do dokumentu

W Microsoft Word znak wodny można łatwo wstawić do dokumentu za pomocą polecenia Wstaw Znak wodny. Aspose.Words zapewnia klasę [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) do dodawania lub usuwania znaku wodnego w dokumentach. Aspose.Words zapewnia wyliczenie [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) definiujące trzy możliwe typy znaków wodnych ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) i [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) do pracy.

### Dodaj Tekstowy Znak Wodny

Poniższy przykład kodu pokazuje, jak wstawić tekstowy znak wodny do dokumentu, definiując [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) przy użyciu metody [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### Dodaj Znak Wodny Obrazu

Poniższy przykład kodu pokazuje, jak wstawić znak wodny obrazu do dokumentu, definiując [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) przy użyciu metody [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

Znak wodny obrazu można wstawić jako obraz, ciąg lub strumień.

Znak wodny można również wstawić za pomocą klasy kształtu. Bardzo łatwo jest wstawić dowolny kształt lub obraz do nagłówka lub stopki, a tym samym utworzyć znak wodny dowolnego możliwego typu.

Poniższy przykład kodu wstawia znak wodny do dokumentu Word:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

Możesz pobrać plik szablonu tego przykładu z [tutaj](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Usuń znak wodny z dokumentu

Klasa [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) zapewnia metodę usuwania, aby usunąć znak wodny z dokumentu.

Poniższy przykład kodu pokazuje, jak usunąć znak wodny z dokumentów:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

Jeśli znaki wodne są dodawane za pomocą obiektu klasy [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/), aby usunąć znak wodny z dokumentu, musisz ustawić tylko nazwę kształtu znaku wodnego podczas wstawiania, a następnie usunąć kształt znaku wodnego za pomocą przypisanej nazwy.

Poniższy przykład kodu pokazuje, jak ustawić nazwę kształtu znaku wodnego i usunąć go z dokumentu:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## Dodaj znak wodny w komórce tabeli

Czasami musisz wstawić znak wodny / obraz do komórki tabeli i wyświetlić go poza tabelą, możesz użyć właściwości [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/). Ta Właściwość pobiera lub ustawia flagę wskazującą, czy kształt jest wyświetlany wewnątrz tabeli, czy poza nią. Zauważ, że ta właściwość działa tylko wtedy, gdy zoptymalizujesz dokument dla Microsoft Word 2010 przy użyciu metody [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

Poniższy przykład kodu pokazuje, jak korzystać z tej właściwości:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
