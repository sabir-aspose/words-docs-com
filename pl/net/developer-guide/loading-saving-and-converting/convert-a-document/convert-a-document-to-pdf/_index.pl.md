---
title: Konwertować Word do PDF w C#
second_title: Aspose.Words dla .NET
articleTitle: Przekształcić dokument do PDF
linktitle: Przekształcić dokument do PDF
description: "Konwertować Word do PDF w C#. Proste przykłady kodu do konwersji DOCX do PDF. Obsługuje wszystkie formaty Word i obrazy."
type: docs
weight: 10
url: /pl/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

Możliwość łatwego i niezawodnego konwertowania dokumentów z jednego formatu na inny jest kluczową funkcją Aspose.Words. PDF jest jednym z najpopularniejszych formatów do konwersji – to format o stałym układzie, który zachowuje oryginalny wygląd dokumentu podczas renderowania na różnych platformach. Termin "renderowanie" jest używany w Aspose.Words do opisania procesu przekształcania dokumentu do formatu pliku, który jest paginowany lub ma koncepcję stron.

## Konwertować dokument Word do PDF

Konwersja z Word do PDF to dość skomplikowany proces, który wymaga kilku etapów obliczeń. Silnik układu Aspose.Words naśladuje sposób działania silnika układu stron Microsoft Word, dzięki czemu wyjściowe dokumenty PDF wyglądają jak najbardziej zbliżone do tego, co można zobaczyć w Microsoft Word.

Za pomocą Aspose.Words możesz programowo przekształcić dokument z formatów Word, takich jak DOC lub DOCX, do PDF bez używania Microsoft Office. Ten artykuł wyjaśnia, jak przeprowadzić tę konwersję.

{{% alert color="primary" %}}

Zauważ, że liczba stron w dokumencie wpływa na czas konwersji.

{{% /alert %}}

### Konwertować DOCX lub DOC do PDF

Przekształcanie z formatu dokumentu DOC lub DOCX do formatu PDF w Aspose.Words jest bardzo proste i można to osiągnąć za pomocą zaledwie dwóch linijek kodu, które:

1. Załaduj swój dokument do obiektu [Document](https://reference.aspose.com/words/net/aspose.words/document/) używając jednego z jego konstruktorów przez podanie nazwy dokumentu z rozszerzeniem jego formatu.
1. Wywołaj jedną z metod [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) na obiekcie **Document** i określ żądany format wyjściowy jako PDF, wprowadzając nazwę pliku z rozszerzeniem ".PDF".

Poniższy przykład kodu pokazuje, jak konwertować dokument z DOCX do PDF używając metody [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

Możesz pobrać plik szablonu tego przykładu z [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx).

{{% alert color="primary" %}}

Czasami konieczne jest określenie dodatkowych opcji, które mogą wpłynąć na wynik zapisywania dokumentu jako PDF. Opcje te można określić za pomocą klasy [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/), zawierającej właściwości, które określają sposób wyświetlania wyjścia PDF.

Zauważ, że tą samą techniką możesz zamieniać dowolny dokument w formacie flow-layout na format PDF.

{{% /alert %}}

### Przekształcić do różnych standardów PDF

Aspose.Words zapewnia wyliczenie [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) do obsługi konwersji DOC lub DOCX do różnych standardów formatu PDF (takich jak PDF 1.7, PDF 1.5, itp.).

Poniższy przykład kodu demonstruje, jak konwertować dokument do PDF 1.7 używając [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) ze zgodnością z PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## Konwertować obrazy do PDF

Konwersja do PDF nie jest ograniczona do formatów dokumentów Microsoft Word. Dowolny format obsługiwany przez Aspose.Words, włączając te utworzone programowo, może być również przekształcony do PDF. Na przykład, możemy konwertować jednostronicowe obrazy, takie jak JPEG, PNG, BMP, EMF, lub WMF, jak również wielostronicowe obrazy, takie jak TIFF i GIF, do PDF.

Poniższy przykład kodu pokazuje, jak zamieniać obrazy JPEG i TIFF na PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

Aby ten kod działał, musisz dodać referencje do Aspose.Words i `System.Drawing` w swoim projekcie.

## Zmniejszenie rozmiaru wyjścia PDF

Podczas zapisywania do PDF możesz określić, czy chcesz optymalizować wyjście. W tym celu musisz ustawić flagę [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) na true, a wtedy nadmiarowe zagnieżdżone i puste płótna zostaną usunięte, sąsiednie glyfy z tym samym formatowaniem zostaną połączone.

Poniższy przykład kodu pokazuje, jak optymalizować wyjście:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

Używanie właściwości **OptimizeOutput** może wpłynąć na dokładność wyświetlania treści.

{{% /alert %}}

## Zobacz również

- Artykuł [Renderowanie](/words/pl/net/rendering/) aby uzyskać więcej informacji o formatach stałej strony i flow-layout
- Artykuł [Konwersja do formatu stałej strony](/words/net/converting-to-fixed-page-format/#what-is-a-page-layout) aby uzyskać więcej informacji o układzie strony
- Artykuł [Określanie opcji renderowania podczas przekształcania do PDF](/words/pl/net/specify-rendering-options-when-converting-to-pdf/) aby uzyskać więcej informacji o używaniu klasy `PdfSaveOptions`
- Artykuł [Poznaj funkcje konwersji do PDF/A i PDF/UA](/words/pl/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) opisujący, który standard PDF i odpowiednie ISO dla standardów PDF są obsługiwane przez Aspose.Words
- Artykuł [Który standard PDF lepiej wybrać](/words/pl/net/which-pdf-standard-is-better-to-choose/) do określenia, które standardy PDF mają sens dla których przypadków

- Artykuł [Praca z PDF/A lub PDF/UA](/words/pl/net/working-with-pdfa-or-pdfua/) opisuje wymagania dotyczące zawartości dokumentu w formatach PDF/A i PDF/UA – głównie wymagania dotyczące struktury i czcionek

- Artykuł [Ostrzeżenia o problemach z dostępnością podczas zapisywania do PDF/A i PDF/UA](/words/pl/net/warnings-when-saving-to-pdfa-and-pdfua/) opisuje, jakie wymagania dostępności treści nakładają PDF/A i PDF/UA
