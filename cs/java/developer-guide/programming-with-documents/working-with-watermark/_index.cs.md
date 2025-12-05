---
title: Práce s vodoznakem v Java
second_title: Aspose.Words pro Java
articleTitle: Práce s vodoznakem
linktitle: Práce s vodoznakem
type: docs
description: "Manipulace s vodoznakem dokumentu pomocí Java."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cs/java/working-with-watermark/
timestamp: 2025-04-22-08-07-04
---

Toto téma pojednává o tom, jak programově pracovat s vodoznakem pomocí Aspose.Words. Vodoznak je obrázek na pozadí, který se zobrazuje za textem v dokumentu. Vodoznak může obsahovat text nebo obrázek reprezentovaný třídou [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/).

{{% alert color="primary" %}}

**Vyzkoušejte online**

Tuto funkci můžete vyzkoušet pomocí našeho [Zdarma online vodoznak dokumentu](https://products.aspose.app/words/watermark).

{{% /alert %}}

## Přidání vodoznaku do dokumentu

V Microsoft Word lze vodoznak snadno vložit do dokumentu pomocí příkazu Vložit vodoznak. Aspose.Words poskytuje třídu [watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) pro přidání nebo odebrání vodoznaku v dokumentech. Aspose.Words poskytuje výčet [WatermarkType ](https://reference.aspose.com/words/java/com.aspose.words/watermarktype/)definující tři možné typy vodoznaků (Text, obrázek a žádný), se kterými lze pracovat.

### Přidat Vodoznak Textu

Následující příklad kódu ukazuje, jak vložit textový vodoznak do dokumentu definováním [TextWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/textwatermarkoptions/) pomocí metody [SetText](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setText-java.lang.String):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddTextWatermarkWithSpecificOptions.java" >}}

### Přidat Vodoznak Obrázku

Následující příklad kódu ukazuje, jak vložit vodoznak obrázku do dokumentu definováním [ImageWatermarkOptions](https://reference.aspose.com/words/java/com.aspose.words/imagewatermarkoptions/) pomocí metody [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.awt.image.BufferedImage):

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-AddImageWatermarkWithSpecificOptions.java" >}}

Vodoznak obrázku lze vložit jako obrázek, řetězec nebo stream.

Vodoznak lze také vložit pomocí třídy tvarů. Je velmi snadné vložit jakýkoli tvar nebo obrázek do záhlaví nebo zápatí a vytvořit tak vodoznak jakéhokoli představitelného typu.

Následující příklad kódu vloží vodoznak do dokumentu Word:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-AddWatermarkToADocument-AddWatermarkToADocument.java" >}}

{{% alert color="primary" %}}

Ukázkový soubor tohoto příkladu si můžete stáhnout z [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Document.doc).

{{% /alert %}}


## Odstranění vodoznaku z dokumentu

Třída [Watermark](https://reference.aspose.com/words/java/com.aspose.words/watermark/) poskytuje metodu `Remove` k odstranění vodoznaku z dokumentu.

Následující příklady kódu ukazují, jak odstranit vodoznak z dokumentů:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkWithWatermark-RemoveWatermarkFromDocument.java" >}}

Chcete-li odstranit vodoznak z dokumentu, musíte během vkládání nastavit pouze název obrazce vodoznaku a poté odebrat obrazec vodoznaku přiřazeným názvem.

Následující příklad kódu ukazuje, jak nastavit název tvaru vodoznaku a odstranit jej z dokumentu:

{{< highlight csharp >}}

// Set name to be able to remove it afterwards
watermark.Name("WaterMark");
{{< /highlight >}}

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-images-RemoveWatermark-RemoveWatermark.java" >}}

## Přidání vodoznaku do buňky tabulky

Někdy je třeba vložit vodoznak / obrázek do buňky tabulky a zobrazit jej mimo tabulku, můžete použít vlastnost [IsLayoutInCell](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#isLayoutInCell-boolean). Tato vlastnost získá nebo nastaví příznak označující, zda je obrazec zobrazen uvnitř tabulky nebo mimo ni. Všimněte si, že tato vlastnost funguje pouze při optimalizaci dokumentu pro Microsoft Word 2010 pomocí metody [OptimizeFor](https://reference.aspose.com/words/java/com.aspose.words/compatibilityoptions/#optimizeFor-int).

Následující příklad kódu ukazuje, jak tuto vlastnost používat:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-programming_documents-Shapes-WorkingWithShapes-SetShapeLayoutInCell.java" >}}
