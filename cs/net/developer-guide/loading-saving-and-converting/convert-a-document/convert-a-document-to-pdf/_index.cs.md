---
title: Převést Word do PDF v C#
second_title: Aspose.Words pro .NET
articleTitle: Konvertovat dokument do PDF
linktitle: Konvertovat dokument do PDF
description: "Převést Word do PDF v C#. Jednoduché příklady kódu pro konverzi DOCX do PDF. Podporuje všechny Word formáty a obrázky."
type: docs
weight: 10
url: /cs/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Schopnost snadno a spolehlivě převádět dokumenty z jednoho formátu do druhého je klíčová vlastnost Aspose.Words. PDF je jedním z nejoblíbenějších formátů pro převod – jedná se o formát s pevným rozložením, který zachovává původní vzhled dokumentu při vykreslování na různých platformách. Termín "vykreslování" se používá v Aspose.Words k popisu procesu konvertování dokumentu do formátu souboru, který je rozdělen na stránky nebo má koncept stránek.

## Převést Word dokument do PDF

Převod z Word do PDF je poměrně složitý proces, který vyžaduje několik fází výpočtů. Layout engine Aspose.Words napodobuje způsob, jakým funguje layout engine stránek Microsoft Word, čímž dosahuje toho, že výstupní PDF dokumenty vypadají co nejpodobnějí tomu, co vidíte v Microsoft Word.

S Aspose.Words můžete programově konvertovat dokument z Word formátů, jako je DOC nebo DOCX, do PDF bez použití Microsoft Office. Tento článek vysvětluje, jak tuto konverzi provést.

{{% alert color="primary" %}}

Všimněte si, že počet stránek v dokumentu ovlivňuje čas konverze.

{{% /alert %}}

### Převést DOCX nebo DOC do PDF

Konverze z DOC nebo DOCX formátu dokumentu do PDF formátu v Aspose.Words je velmi snadná a lze ji dosáhnout pouze dvěma řádky kódu, které:

1. Načtěte svůj dokument do objektu [Document](https://reference.aspose.com/words/net/aspose.words/document/) pomocí jednoho z jeho konstruktorů zadáním názvu dokumentu s jeho příponou formátu.
1. Zavolejte jednu z metod [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) na objektu **Document** a specifikujte požadovaný výstupní formát jako PDF zadáním názvu souboru s příponou ".PDF".

Následující příklad kódu ukazuje, jak transformovat dokument z DOCX do PDF pomocí metody [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Soubor šablony pro tento příklad si můžete stáhnout z [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Někdy je nutné specifikovat další možnosti, které mohou ovlivnit výsledek uložení dokumentu jako PDF. Tyto možnosti lze specifikovat pomocí třídy [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), která obsahuje vlastnosti určující, jak bude zobrazen PDF výstup.

Všimněte si, že stejnou technikou můžete konvertovat jakýkoli dokument s plovoucím rozložením do PDF formátu.

{{% /alert %}}

### Konvertovat do různých PDF standardů

Aspose.Words poskytuje výčet [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) pro podporu převodu DOC nebo DOCX do různých standardů PDF formátu (jako je PDF 1.7, PDF 1.5, atd.).

Následující příklad kódu ukazuje, jak převést dokument do PDF 1.7 pomocí [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) s dodržením PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Převést obrázky do PDF

Konverze do PDF není omezena na formáty Microsoft Word dokumentů. Jakýkoli formát podporovaný Aspose.Words, včetně programově vytvořených, může být také transformován do PDF. Například můžeme konvertovat jednostránkové obrázky, jako jsou JPEG, PNG, BMP, EMF nebo WMF, stejně jako vícestránkové obrázky, jako jsou TIFF a GIF, do PDF.

Následující příklad kódu ukazuje, jak převést JPEG a TIFF obrázky do PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Pro správnou funkcionalitu tohoto kódu musíte přidat reference na Aspose.Words a `System.Drawing` do vašeho projektu.

## Snížit velikost PDF výstupu

Při ukládání do PDF můžete specifikovat, zda chcete optimalizovat výstup. K tomu musíte nastavit příznak [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) na true, a pak budou odstraněna redundantní vnořená a prázdná plátna, sousední glyfy se stejným formátováním budou zřetězeny.

Následující příklad kódu ukazuje, jak optimalizovat výstup:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Použití vlastnosti **OptimizeOutput** může ovlivnit přesnost zobrazení obsahu.

{{% /alert %}}

## Viz také

- Článek [Vykreslování](/words/cs/net/rendering/) pro více informací o formátech s pevnou stránkou a plovoucím rozložením
- Článek [Převod do formátu s pevnou stránkou](/words/cs/net/converting-to-fixed-page-format/#what-is-a-page-layout) pro více informací o rozložení stránky
- Článek [Specifikace možností vykreslování při konvertování do PDF](/words/cs/net/specify-rendering-options-when-converting-to-pdf/) pro více informací o použití třídy `PdfSaveOptions`
- Článek [Poznejte funkce konverze do PDF/A a PDF/UA](/words/cs/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) popisující, který PDF standard a příslušné ISO pro PDF standardy podporuje Aspose.Words
- Článek [Který PDF standard je lepší zvolit](/words/cs/net/which-pdf-standard-is-better-to-choose/) pro určení, které PDF standardy dávají smysl pro které případy

- Článek [Práce s PDF/A nebo PDF/UA](/words/cs/net/working-with-pdfa-or-pdfua/) popisuje požadavky na obsah dokumentu ve formátech PDF/A a PDF/UA – především požadavky na strukturu a písma

- Článek [Upozornění na problémy s přístupností při ukládání do PDF/A a PDF/UA](/words/cs/net/warnings-when-saving-to-pdfa-and-pdfua/) popisuje, jaké požadavky na přístupnost obsahu ukládají PDF/A a PDF/UA
