---
title: Práce s vodoznakem v Python
second_title: Aspose.Words pro Python via .NET
articleTitle: Práce s vodoznakem
linktitle: Práce s vodoznakem
description: "Vytvářejte a spravujte vodoznaky v dokumentu pomocí Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Toto téma pojednává o tom, jak programově pracovat s vodoznakem pomocí Aspose.Words. Vodoznak je obrázek na pozadí, který se zobrazuje za textem v dokumentu. Vodoznak může obsahovat text nebo obrázek reprezentovaný třídou [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Vyzkoušejte online**

Tuto funkci můžete vyzkoušet pomocí našeho [Zdarma online vodoznak dokumentu](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Jak přidat vodoznak do dokumentu

V Microsoft Word lze vodoznak snadno vložit do dokumentu pomocí příkazu Vložit vodoznak. Aspose.Words poskytuje třídu [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) pro přidání nebo odebrání vodoznaku v dokumentech. Aspose.Words poskytuje výčet [WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/) definující tři možné typy vodoznaků ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text), [IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image) a [NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none)) pro práci.

### Přidat Vodoznak Textu

Následující příklad kódu ukazuje, jak vložit textový vodoznak do dokumentu definováním [TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/) pomocí metody [set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### Přidat Vodoznak Obrázku

Následující příklad kódu ukazuje, jak vložit vodoznak obrázku do dokumentu definováním [ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/) pomocí metody [set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

Vodoznak obrázku lze vložit jako obrázek, řetězec nebo stream.

Vodoznak lze také vložit pomocí třídy tvarů. Je velmi snadné vložit jakýkoli tvar nebo obrázek do záhlaví nebo zápatí a vytvořit tak vodoznak jakéhokoli představitelného typu.

Následující příklad kódu vloží vodoznak do dokumentu Word:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

Soubor šablony tohoto příkladu si můžete stáhnout z [nízko](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Odstranění vodoznaku z dokumentu

Třída [Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/) poskytuje metodu remove pro odstranění vodoznaku z dokumentu.

Následující příklad kódu ukazuje, jak odstranit vodoznak z dokumentů:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

Pokud jsou vodoznaky přidány pomocí objektu třídy [Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/), pak pro odstranění vodoznaku z dokumentu musíte během vkládání nastavit pouze název tvaru vodoznaku a poté odstranit tvar vodoznaku přiřazeným názvem.

Následující příklad kódu ukazuje, jak nastavit název tvaru vodoznaku a odstranit jej z dokumentu:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## Přidání vodoznaku do buňky tabulky

Někdy je třeba vložit vodoznak / obrázek do buňky tabulky a zobrazit jej mimo tabulku, můžete použít vlastnost [is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/). Tato vlastnost získá nebo nastaví příznak označující, zda je obrazec zobrazen uvnitř tabulky nebo mimo ni. Všimněte si, že tato vlastnost funguje pouze při optimalizaci dokumentu pro Microsoft Word 2010 pomocí metody [optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

Následující příklad kódu ukazuje, jak tuto vlastnost používat:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
