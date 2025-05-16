---
title: Práce s vodoznakem v C#
second_title: Aspose.Words pro .NET
articleTitle: Práce s vodoznakem
linktitle: Práce s vodoznakem
description: "Manipulace s vodoznakem dokumentu pomocí C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /cs/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

Toto téma pojednává o tom, jak programově pracovat s vodoznakem pomocí Aspose.Words. Vodoznak je obrázek na pozadí, který se zobrazuje za textem v dokumentu. Vodoznak může obsahovat text nebo obrázek reprezentovaný třídou [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**Vyzkoušejte online**

Tuto funkci můžete vyzkoušet pomocí našeho [Zdarma online vodoznak dokumentu](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Přidání vodoznaku do dokumentu

V Microsoft Word lze vodoznak snadno vložit do dokumentu pomocí příkazu Vložit vodoznak. Aspose.Words poskytuje třídu [watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) pro přidání nebo odebrání vodoznaku v dokumentech. Aspose.Words poskytuje výčet [WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)definující tři možné typy vodoznaků (Text, obrázek a žádný), se kterými lze pracovat.

### Přidat Vodoznak Textu

Následující příklad kódu ukazuje, jak vložit textový vodoznak do dokumentu definováním [TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/) pomocí metody [SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### Přidat Vodoznak Obrázku

Následující příklad kódu ukazuje, jak vložit vodoznak obrázku do dokumentu definováním [ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/) pomocí metody [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

Vodoznak obrázku lze vložit jako obrázek, řetězec nebo stream.

Vodoznak lze také vložit pomocí třídy tvarů. Je velmi snadné vložit jakýkoli tvar nebo obrázek do záhlaví nebo zápatí a vytvořit tak vodoznak jakéhokoli představitelného typu.

Následující příklad kódu vloží vodoznak do dokumentu Word:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

Ukázkový soubor tohoto příkladu si můžete stáhnout z [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## Odstranění vodoznaku z dokumentu

Třída [Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/) poskytuje metodu remove pro odstranění vodoznaku z dokumentu.

Následující příklad kódu ukazuje, jak odstranit vodoznak z dokumentů:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

Pokud jsou vodoznaky přidány pomocí objektu třídy [Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/), pak pro odstranění vodoznaku z dokumentu musíte během vkládání nastavit pouze název tvaru vodoznaku a poté odstranit tvar vodoznaku přiřazeným názvem.

Následující příklad kódu ukazuje, jak nastavit název tvaru vodoznaku a odstranit jej z dokumentu:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## Přidání vodoznaku do buňky tabulky

Někdy je třeba vložit vodoznak / obrázek do buňky tabulky a zobrazit jej mimo tabulku, můžete použít vlastnost [IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/). Tato vlastnost získá nebo nastaví příznak označující, zda je obrazec zobrazen uvnitř tabulky nebo mimo ni. Všimněte si, že tato vlastnost funguje pouze při optimalizaci dokumentu pro Microsoft Word 2010 pomocí metody [OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

Následující příklad kódu ukazuje, jak tuto vlastnost používat:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
