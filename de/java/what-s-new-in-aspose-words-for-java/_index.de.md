---
title: Was ist neu
second_title: Aspose.Words für Java
articleTitle: Was ist neu in Aspose.Words für Java
linktitle: Was ist neu in Aspose.Words für Java
type: docs
description: "Aspose.Words für Java erweitert und verbessert sich täglich. Auf dieser Seite erfahren Sie mehr über die großen und interessantesten Funktionen des Produkts."
weight: 2
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /de/java/what-s-new-in-aspose-words-for-java/
timestamp: 2025-06-23-21-02-49
---

Diese Seite beschreibt die interessantesten neuen Aspose.Words Funktionen, die in den letzten Versionen eingeführt wurden.

## Aspose.Words für Java 25.5, 25.6

Aspose.Words 25.5 verbessert die Diagrammanpassung mit neuen Stiloptionen und verbessert den Markdown-Export, indem es die Kontrolle darüber bietet, wie leere Absätze behandelt werden.

Aspose.Words 25.6 verbessert die Rendergenauigkeit und die Visualisierungsfunktionen durch die Einführung erweiterter Bildexportoptionen, verbesserter MathML -Handhabung und besserer Diagrammdarstellung.

### Dokumente konvertieren, laden und speichern

#### Leere Absätze nach Markdown exportieren <sup>25.5</sup>

Die Möglichkeit zu steuern, wie leere Absätze nach Markdown exportiert werden, wurde durch Hinzufügen der [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownemptyparagraphexportmode/)-Aufzählung und der [EmptyParagraphExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getEmptyParagraphExportMode)-Eigenschaft eingeführt.

#### Exportieren Sie mehrseitige Dokumente in Rasterbildformate <sup>25.6</sup>

Die Möglichkeit, mehrseitige Dokumente in Rasterbildformate (wie PNG und JPEG) mit [customizable layouts](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/) - Horizontal, Vertikal oder Raster – zu exportieren, wurde durch die Erweiterung der Bildexportfunktionalität eingeführt.

### Rendering

#### Festlegen des Diagrammstils <sup>25.5</sup>

Die Möglichkeit, den Diagrammstil festzulegen, wurde durch Hinzufügen der [ChartStyle](https://reference.aspose.com/words/java/com.aspose.words/chartstyle/)-Aufzählung und der [Style](https://reference.aspose.com/words/java/com.aspose.words/chart/#getStyle)-Eigenschaft eingeführt.

#### Verbindungslinien in MathML -Ausdrücken rendern <sup>25.6</sup>

Die Darstellung von Verbindungslinien in MathML-Ausdrücken wurde implementiert, um eine genauere und visuell konsistentere Anzeige mathematischer Formeln zu gewährleisten.

#### Rendering von Legenden für Wasserfalldiagramme <sup>25.6</sup>

Die Darstellung von Legenden für ["Waterfall" charts](https://reference.aspose.com/words/java/com.aspose.words/chartseriestype/) wurde eingeführt, um die Datentransparenz zu erhöhen und die Interpretierbarkeit dieser Diagramme zu verbessern.

### Andere

* Die Möglichkeit, mathematische Formeln mit mehreren Schrägstrichen zu umbrechen, wurde verbessert, um die Layoutklarheit und die Lesbarkeit von Formeln zu verbessern. <sup>25.6</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für Java 25.5 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-5-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 25.6 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words für Java 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 führt eine AI-basierte Grammatikprüfung ein und verbessert das Speichern von Dokumenten mit erweiterten Optionen für die Formate HTML, SVG und Markdown.

Aspose.Words 25.2 führt die Textzusammenfassung mit Anthropic AI-Modellen ein, fügt MsWorks-Formatunterstützung hinzu, verbessert die typografische Steuerung und verbessert die PDF-Struktur und die Listenbehandlung.

Aspose.Words 25.3 verbessert eine AI-basierte Grammatikprüfung und Schriftauswahl mit der UpdateAmbiguousTextFont-Eigenschaft sowie den Export von PDF-Anhängen.

Aspose.Words 25.4 bietet Unterstützung für neue Papierformate, ermöglicht eine erweiterte HTML Exportkontrolle, verbessert die Handhabung von Wasserzeichen und verbessert die Benutzerfreundlichkeit von LowCode API.

### AI-betriebene Funktionen

#### Dokument AI Grammatikprüfung

* Die Möglichkeit, die Grammatik des bereitgestellten Dokuments mithilfe generativer OpenAI -Modelle zu überprüfen, wurde durch Hinzufügen einer neuen [CheckGrammar](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#checkGrammar-com.aspose.words.Document-com.aspose.words.CheckGrammarOptions) -Methode eingeführt. <sup>25.1</sup>
* Die AI-basierte Grammatikprüfungsfunktion wurde aktualisiert, um alle in der [AiModelType](https://reference.aspose.com/words/java/com.aspose.words/aimodeltype/) -Aufzählung verfügbaren Modelle zu unterstützen. <sup>25.3</sup>

#### Zusammenfassung mit Anthropic generativen Sprachmodellen <sup>25.2</sup>

Die Textzusammenfassung mit Anthropic generativen Sprachmodellen wurde durch die Einführung einer neuen öffentlichen Klasse [AnthropicAiModel](https://reference.aspose.com/words/java/com.aspose.words/anthropicaimodel/) ermöglicht.

### Low Code

#### Low Code API Benutzerfreundlichkeit <sup>25.4</sup>

Die Benutzerfreundlichkeit von **LowCode API** wurde erheblich verbessert, wodurch die Dokumentenverarbeitung vereinfacht und der Bedarf an sich wiederholendem Code verringert wird.

### Unterstützte Formate <sup>25.2</sup>

Ab Version 25.2 wurde die Kompatibilität mit dem neuen MsWorks Ladeformat für Microsoft Werksdokumente hinzugefügt.

### Dokumente konvertieren, laden und speichern

#### Verbessertes Speichern in den Formaten HTML und SVG <sup>25.1</sup>

Das Speichern in den Formaten HTML und SVG wurde verbessert, indem den Klassen [HtmlFixedSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlfixedsaveoptions/) und [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/) Eigenschaften **IdPrefix** und **RemoveJavaScriptFromLinks** hinzugefügt wurden.

#### Stellen Sie die Bildauflösung und den OfficeMath -Ausgabemodus beim Speichern auf Markdown ein <sup>25.1</sup>

* Der Klasse [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) wurde eine neue Option [ImageResolution](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImageResolution) hinzugefügt, um die Bildauflösung festzulegen.
* Eine neue [OfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getOfficeMathExportMode) -Option und [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownofficemathexportmode/) -Aufzählung wurden der [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) -Klasse hinzugefügt, um den OfficeMath -Ausgabemodus festzulegen.
* Die Möglichkeit, ein Bildwasserzeichen aus einem Stream zu setzen, wurde eingeführt, indem der [SetImage](https://reference.aspose.com/words/java/com.aspose.words/watermark/#setImage-java.io.InputStream-com.aspose.words.ImageWatermarkOptions) -Methode eine neue Überladung hinzugefügt wurde. <sup>25.4</sup>

### Rendering

#### Verbesserte typografische Kontrolle <sup>25.2</sup>

Die Eigenschaft [NumberSpacing](https://reference.aspose.com/words/java/com.aspose.words/font/#getNumberSpacing) wurde für eine verbesserte typografische Kontrolle hinzugefügt.

#### Steuern der Schriftauswahl für mehrdeutige Zeichen <sup>25.3</sup>

Der Klasse [SaveOptions](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/) wurde eine neue öffentliche Eigenschaft [UpdateAmbiguousTextFont](https://reference.aspose.com/words/java/com.aspose.words/saveoptions/#getUpdateAmbiguousTextFont) hinzugefügt, um die Schriftauswahl entsprechend dem verwendeten Zeichencode zu steuern.

#### Optionen für das Papierformat <sup>25.4</sup>

Die Möglichkeit, die Papierformate JIS B4 und JIS B5 zu verwenden, wurde eingeführt, indem der [PaperSize](https://reference.aspose.com/words/java/com.aspose.words/papersize/)-Aufzählung neue Werte hinzugefügt wurden.

#### HTML Ausgabesteuerung <sup>25.4</sup>

Die Möglichkeit, JavaScript während des HTML-Exports aus dem Hyperlink URLs zu entfernen, wurde durch Hinzufügen der Eigenschaft [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/#getRemoveJavaScriptFromLinks) eingeführt.

### Andere

* PDF logische Struktur wurde mit Unterstützung für TOA, BIBLIOGRAPHY und INDEX Felder verbessert. <sup>25.2</sup>
* Die [AddSingleLevelList](https://reference.aspose.com/words/java/com.aspose.words/listcollection/#addSingleLevelList-int) -Methode wurde für eine verbesserte Listenbehandlung eingeführt. <sup>25.2</sup>
* Eine neue Eigenschaft [AttachmentsEmbeddingMode](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getAttachmentsEmbeddingMode) wurde hinzugefügt, um **EmbedAttachments** zu ersetzen, um den Export von PDF-Anhängen zu verbessern. Außerdem wurden der [PdfCompliance](https://reference.aspose.com/words/java/com.aspose.words/pdfcompliance/) -Aufzählung neue Werte hinzugefügt, um Anhänge der PDF/A -Version zu unterstützen. Außerdem werden Anhänge jetzt mit Verschlüsselung unterstützt. <sup>25.3</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für Java 25.1 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-1-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 25.2 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-2-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 25.3 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-3-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 25.4 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2025/aspose-words-for-java-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words für Java 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 führt die Einfügung von group shape und StructuredDocumentTag über DocumentBuilder ein, verbessert die Darstellung von Radialdiagrammen mit Graduierungen, verbessert digitale Signaturen mit XAdES-EPES-Unterstützung, fügt die Unterstreichungserkennung von Markdown hinzu und bietet Zugriff auf Fußnoten-/Endnotentrennzeichen.

Aspose.Words 24.10 führt eine erweiterte ActiveX-Steuerungsunterstützung mit CommandButton -Erstellung, eine neue Steuerung der Formsichtbarkeit, die Möglichkeit zu group shapes, einen verbesserten Markdown-Export für Tabellen, Diagrammformatierung für Pie- und Doughnut-Diagramme, eine bessere Big5-Codierungsbehandlung und Unterstützung für veraltete taiwanesische Schriftarten ein.

Aspose.Words 24.11 führt die AI-basierte Dokumentzusammenfassung, erweiterte Renderoptionen, verbesserten Zugriff auf Dokumenteigenschaften und ActiveX-Steueruntertitelung ein.

Aspose.Words 24.12 führt eine anpassbare Platzierung von Datenetiketten, eine von Google AI unterstützte Textübersetzung, erweiterte Mail Merge Bereinigungsoptionen und neue LowCode Verarbeitungsklassen ein.

### AI-betriebene Funktionen

#### Dokumentzusammenfassung mit OpenAI und Google <sup>24.11</sup>

Unterstützung für Dokumentzusammenfassungen mit generativen Sprachmodellen **OpenAI** und **Google** wurde integriert.

#### Textübersetzung mit den generativen Sprachmodellen von Google <sup>24.12</sup>

Die Möglichkeit, Text mit den generativen Sprachmodellen von Google zu übersetzen, wurde in Aspose.Words implementiert, indem die [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) -Methode und die [Language](https://reference.aspose.com/words/java/com.aspose.words/language/) -Aufzählung hinzugefügt wurden.

### Low Code <sup>24.12</sup>

Neue LowCode Klassen wie [Comparer](https://reference.aspose.com/words/java/com.aspose.words/comparer/), [MailMerger](https://reference.aspose.com/words/java/com.aspose.words/mailmerger/), [Replacer](https://reference.aspose.com/words/java/com.aspose.words/replacer/), [Splitter](https://reference.aspose.com/words/java/com.aspose.words/splitter/) usw. wurde eingeführt und bietet eine Reihe von Methoden, die die perfekte Balance zwischen Einfachheit und Flexibilität für die Dokumentenverarbeitung finden.

### Rendern und Drucken

#### Graduierungen auf Radialdiagrammen <sup>24.9</sup>

Die Darstellung von Abstufungen auf Radialdiagrammen wurde implementiert.

#### CommandButton ActiveX Bedienelemente <sup>24.10</sup>

Die Möglichkeit, CommandButton ActiveX-Steuerelemente zu erstellen, wurde durch Hinzufügen einer neuen öffentlichen Methode [InsertForms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertForms2OleControl-com.aspose.words.Forms2OleControl) und einer neuen öffentlichen Klasse [Forms2OleControl](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/) eingeführt.

#### Sichtbarkeit der Form steuern <sup>24.10</sup>

Eine neue öffentliche Eigenschaft [Hidden](https://reference.aspose.com/words/java/com.aspose.words/shapebase/#getHidden) wurde hinzugefügt, um die Sichtbarkeit von Formen zu steuern.

#### Änderungen in den Diagrammen Pie und Doughnut <sup>24.10</sup>

Dem Formatieren von Pie- und Doughnut-Diagrammen wurden mehrere neue öffentliche Eigenschaften hinzugefügt.

#### Steuern Sie das Rendern von PDF-Auswahlformularfeldrändern <sup>24.11</sup>

Eine neue Option zur Steuerung der Darstellung von PDF-Auswahlformularfeldrändern wurde implementiert, indem eine neue öffentliche Option [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getRenderChoiceFormFieldBorder) hinzugefügt wurde.

#### Formatcodes für Diagrammdaten abrufen und festlegen <sup>24.11</sup>

Die Möglichkeit, Formatcodes für Diagrammdaten abzurufen und festzulegen, wurde hinzugefügt, indem die Eigenschaft [FormatCode](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/#getFormatCode) in den Klassen [ChartXValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/java/com.aspose.words/chartyvaluecollection/) und [BubbleSizeCollection](https://reference.aspose.com/words/java/com.aspose.words/bubblesizecollection/) implementiert wurde.

#### Histogrammdiagramme mit Bins und Beschriftungen rendern <sup>24.11</sup>

Die Darstellung von Histogrammdiagrammen wurde verbessert, indem eine bestimmte Anzahl von Behältern und Beschriftungen zugelassen wurde.

### Dokumente konvertieren, laden und speichern

#### Formatierung beim Laden von Markdown-Dateien unterstreichen <sup>24.9</sup>

Die Option, Unterstreichungsformatierungen beim Laden von Markdown-Dokumenten zu erkennen, wurde durch Hinzufügen einer neuen öffentlichen Eigenschaft [ImportUnderlineFormatting](https://reference.aspose.com/words/java/com.aspose.words/markdownloadoptions/#getImportUnderlineFormatting) integriert.

#### Tabellen beim Speichern in Markdown als HTML exportieren <sup>24.10</sup>

Eine Option zum Exportieren von Tabellen als HTML beim Speichern von Dokumenten im Markdown-Format wurde implementiert, indem eine neue öffentliche Eigenschaft [ExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getExportAsHtml) und eine Aufzählung [MarkdownExportAsHtml](https://reference.aspose.com/words/java/com.aspose.words/markdownexportashtml/) hinzugefügt wurden.

#### Export PDF mit aktualisierter logischer Struktur <sup>24.11</sup>

Der PDF-Export wurde verbessert, indem Tabellentiteleigenschaften als Titel für logische PDF-Strukturelemente aufgenommen wurden.

### Mail Merge und Berichterstattung

#### Leere Tabellen während Mail Merge entfernen <sup>24.12</sup>

Der [MailMergeCleanupOptions](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/)-Aufzählung wurde eine neue **RemoveEmptyTables**-Option hinzugefügt, um die Mail Merge-Ausgabe zu verfeinern.

### Digitale Signaturen

#### Dokumente mit XAdES-EPES signieren <sup>24.9</sup>

Die Möglichkeit, Dokumente mit XAdES-EPES Level XML-DSig Signaturen zu signieren, wurde durch Hinzufügen einer neuen öffentlichen Eigenschaft [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/signoptions/#getXmlDsigLevel) und einer neuen öffentlichen Aufzählung [XmlDsigLevel](https://reference.aspose.com/words/java/com.aspose.words/xmldsiglevel/) eingeführt

### Andere

* Eine neue öffentliche Methode [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-com.aspose.words.Shape...) wurde zu group shapes hinzugefügt. <sup>24.9</sup>
* Eine neue öffentliche Methode [InsertStructuredDocumentTag](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertStructuredDocumentTag-int) wurde hinzugefügt, um **StructuredDocumentTags** in ein Dokument einzufügen. <sup>24.9</sup>
* Der öffentliche Zugriff auf Fußnoten- / Endnotentrennzeichen wurde durch Hinzufügen einiger öffentlicher Klassen und Eigenschaften ermöglicht. <sup>24.9</sup>
* Die Möglichkeit, einzelne Formen group shapes zu gruppieren und sowohl Formen als auch group shapes direkt zu gruppieren, wurde durch Hinzufügen der [InsertGroupShape](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertGroupShape-double-double-double-double-com.aspose.words.ShapeBase...) -Methode eingeführt. <sup>24.10</sup>
* Die Handhabung der Big5-Codierung für TrueType cmap-Tabellen wurde verbessert. <sup>24.10</sup>
* Die Unterstützung für veraltete taiwanesische Schriftarten wurde verbessert. <sup>24.10</sup>
* Um auf erweiterte Dokumenteigenschaften zuzugreifen, wurden der Klasse [BuiltInDocumentProperties](https://reference.aspose.com/words/java/com.aspose.words/builtindocumentproperties/) schreibgeschützte Eigenschaften hinzugefügt. <sup>24.11</sup>
* Das Festlegen von Beschriftungen für ActiveX-Steuerelemente wurde aktiviert, indem der Eigenschaft [Forms2OleControl.Caption](https://reference.aspose.com/words/java/com.aspose.words/forms2olecontrol/#getCaption) ein neuer öffentlicher Setter hinzugefügt wurde. <sup>24.11</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für Java 24.9 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-9-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 24.10 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-10-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 24.11 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-11-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 24.12 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words für Java 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 erweitert die Optionen für Assemblys, verbessert die Renderfunktionen und erweitert einige andere Optionen.

Aspose.Words 24.6 verbessert die Renderoptionen, erweitert die Such- und Vergleichsfunktionen und erweitert mehrere andere Funktionen.

Aspose.Words 24.7 ändert die Arbeitsweise mit ActiveX, erweitert die Renderfunktionen sowie den Export in die Formate Markdown und XLSX.

Aspose.Words 24.8 verbessert die Diagrammanpassung mit präziser Kontrolle über Achsenbeschriftungen, erweitert die Schriftartverwaltung, verbessert die Handhabung der Dokumentstruktur und fügt neue Funktionen für HTML/XAML-Export, PDF-Funktionalität, Dokumentkonvertierung und digitale Signaturen hinzu.

### Unterstützte Formate

Ab Version 24.7 wird der Export nach PDF/UA-2 unterstützt, um die Zugänglichkeit für Benutzer mit Behinderungen zu gewährleisten.

### Rendern und Drucken

#### Änderungen in Diagrammen, Formen und DrawingML <sup>24.5</sup>

- DrawingML Effektrendering für SVG Grafiken, das die bisherige, auf Bilder beschränkte Funktionalität erweitert, wurde implementiert.
- Unterstützung für das Erstellen von Kombinationsdiagrammen und das Anpassen von Eigenschaften wie Spaltenbreite, Überlappung und Blasenskalierung innerhalb von Reihengruppen wurde eingeführt, indem die Klassen [ChartSeriesGroup](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroup/) und [ChartSeriesGroupCollection](https://reference.aspose.com/words/java/com.aspose.words/chartseriesgroupcollection/) sowie die Eigenschaft [SeriesGroups](https://reference.aspose.com/words/java/com.aspose.words/chart/#getSeriesGroups) hinzugefügt wurden.
- Die Funktionalität zum Manipulieren des SoftEdge -Effekts von Formen wurde durch Hinzufügen der [SoftEdgeFormat](https://reference.aspose.com/words/java/com.aspose.words/softedgeformat/) -Klasse implementiert.
- Die Möglichkeit, Anpassungswerte von Formen zu ändern, wurde durch Hinzufügen der öffentlichen Klassen [AdjustmentCollection](https://reference.aspose.com/words/java/com.aspose.words/adjustmentcollection/) und [Adjustment](https://reference.aspose.com/words/java/com.aspose.words/adjustment/) und der Eigenschaft [Adjustments](https://reference.aspose.com/words/java/com.aspose.words/shape/#getAdjustments) implementiert.

#### Änderungen in Diagrammen, Formen und Zeichnungen <sup>24.6</sup>

- Die Diagrammfunktionen wurden verbessert. Sie können jetzt eine größere Auswahl an Diagrammen erstellen, einschließlich *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* diagramme, *Box & Whisker* Diagramme, *Waterfalls* und *Funnels*. So können Sie Ihre Daten vielfältiger und informativer visualisieren.
- Die Farbsteuerung für die Schattenformatierung wurde verbessert. Sie können das Erscheinungsbild Ihrer Dokumente genauer steuern, indem Sie auf Schattenfarben zugreifen.
- Die Leistungssteigerung für das Hintergrundrendern wurde verbessert. Dank der nativen Kacheltechnologie können Sie das Rendern von Hintergründen mit kleinen Elementen erheblich beschleunigen.
- Realistische Verläufe für Formen wurden hinzugefügt. Sie können jetzt DML -Formen mit nichtlinearen Verläufen erstellen, die den visuellen Stil von Microsoft Word nachahmen, um ein polierteres Aussehen zu erzielen.

#### Anpassung der Diagrammdatenetiketten <sup>24.7</sup>

Die Möglichkeit, Diagrammdatenbeschriftungen wie **Orientation** und **Rotation** anzupassen, wurde hinzugefügt.

#### Benutzerdefiniertes Nummernstyling für Listenebenen <sup>24.7</sup>

Ein Setter für die öffentliche Eigenschaft [CustomNumberStyleFormat](https://reference.aspose.com/words/java/com.aspose.words/listlevel/#getCustomNumberStyleFormat) wurde hinzugefügt. Sie können jetzt einen benutzerdefinierten Nummernstil für Listenebenen definieren.

#### Änderungen bei der Arbeit mit ActiveX <sup>24.7</sup>

* Die Eigenschaften von ActiveX-Objekten können jetzt geändert werden, sodass Sie mehr Kontrolle über ihr Verhalten haben.
* Die Möglichkeit, den Wert des Optionsfelds ActiveX zu ändern, um eine dynamische Interaktion zu ermöglichen, wurde hinzugefügt.
* Die Möglichkeit, eine ActiveX checkbox auf "aktiviert" oder "deaktiviert" umzuschalten, wurde hinzugefügt.

#### Kontrolle über die Ausrichtung und Drehung der Tick-Beschriftungen der Diagrammachse <sup>24.8</sup>

Eine präzise Steuerung der Ausrichtung und Drehung von Teilstrichbeschriftungen der Diagrammachse wurde hinzugefügt, um die Diagrammanpassung komfortabler zu gestalten – die Klasse [AxisTickLabels](https://reference.aspose.com/words/java/com.aspose.words/axisticklabels/) wurde um die neuen Eigenschaften **Orientation** und **Rotation** erweitert.

#### Ersetzen des umgekehrten Schrägstrichs durch das Yen-Zeichen <sup>24.8</sup>

Der abwärtskompatible HTML- und XAML-Export zum Ersetzen des Backslash-Zeichens durch das Yen-Zeichen wurde verbessert. Um dies zu erreichen, wurde den Klassen [HtmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/htmlsaveoptions/) und [XamlFlowSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/) die Eigenschaft **ReplaceBackslashWithYenSign** hinzugefügt.

#### SDT-Tags als Formularfeldnamen beim Export nach PDF verwenden <sup>24.8</sup>

Der PDF-Export mit Unterstützung für die Verwendung von SDT-Tags als Formularfeldnamen wurde verbessert, indem der [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/)-Klasse eine neue **UseSdtTagAsFormFieldName**-Eigenschaft hinzugefügt wurde.

### Dokumente konvertieren, laden und speichern

#### Exportieren von Links in das Markdown -Format <sup>24.7</sup>

Die Möglichkeit, den Export von Links im Format Markdown zu steuern, wurde durch die Implementierung der Eigenschaft [LinkExportMode](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getLinkExportMode) hinzugefügt.

#### LowCode 24.8 <sup>24.8</sup>

Es wurde eine neue **LowCode.Converter** -Klasse eingeführt, die eine Reihe von Methoden zum Konvertieren verschiedener Dokumenttypen mit einer einzigen Codezeile bereitstellt.

### Suchen und vergleichen

#### Erweiterte Vergleichsoptionen <sup>24.6</sup>

Die Möglichkeit, Datenanalyse-Workflows mit verbesserten Vergleichsfunktionen zu rationalisieren, wurde hinzugefügt. Dies beinhaltet eine neue [IgnoreStoreItemId](https://reference.aspose.com/words/java/com.aspose.words/advancedcompareoptions/#getIgnoreStoreItemId) -Option und eine neu gestaltete Oberfläche für erweiterte Vergleiche.

### Andere

* Die Funktion zum Entfernen leerer Seiten aus einem Dokument wurde durch Hinzufügen der [RemoveBlankPages](https://reference.aspose.com/words/java/com.aspose.words/document/#removeBlankPages) -Methode implementiert. <sup>24.5</sup>
* Die Möglichkeit, das Vorhandensein von VBA Makros zu überprüfen, ohne ein Dokument zu laden, wurde durch Hinzufügen der Eigenschaft [HasMacros](https://reference.aspose.com/words/java/com.aspose.words/fileformatinfo/#hasMacros) bereitgestellt. <sup>24.5</sup>
* Die Beibehaltung der Quellennummerierung beim Einfügen eines Dokuments mit der LINQ Reporting Engine wird jetzt unterstützt. <sup>24.5</sup>
* Eine neue [DateTimeUtc](https://reference.aspose.com/words/java/com.aspose.words/comment/#getDateTimeUtc) -Eigenschaft wurde hinzugefügt - dies bietet einen genaueren Zeitstempel für Kommentare, was die Organisation und Rückverfolgbarkeit verbessert. <sup>24.6</sup>
* Die LINQ Reporting Engine wurde verbessert. Das selektive Entfernen leerer Absätze und die Definition benutzerdefinierter Nachrichten für fehlende Objektmitglieder wurden vorgenommen, was zu saubereren und informativeren Berichten führt. <sup>24.6</sup>
* Das Datums-/Uhrzeitformat wird jetzt automatisch für den nahtlosen Export in das XLSX-Format erkannt. <sup>24.7</sup>
* Die öffentliche Eigenschaft [IsProtected](https://reference.aspose.com/words/java/com.aspose.words/vbaproject/#isProtected), mit der Sie überprüfen können, ob ein VBA-Projekt geschützt ist, wurde hinzugefügt. <sup>24.7</sup>
* Die Schriftarteninformationen wurden um die Eigenschaft **EmbeddingLicensingRights** erweitert, die den Klassen [FontInfo](https://reference.aspose.com/words/java/com.aspose.words/fontinfo/) und [PhysicalFontInfo](https://reference.aspose.com/words/java/com.aspose.words/physicalfontinfo/) hinzugefügt wurde. <sup>24.8</sup>
* Es wurde eine Möglichkeit hinzugefügt, Kopf- und Fußzeilen von Abschnitten effizient zu löschen und gleichzeitig Wasserzeichen beizubehalten, um genauer mit der Dokumentstruktur zu arbeiten. Verwenden Sie die neue öffentliche Methode **ClearHeadersFooters**, um Kopf- und Fußzeilen von Abschnitten zu löschen. <sup>24.8</sup>
* Das digitale Signieren von XPS-Dokumenten mit [XpsSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/xpssaveoptions/) wurde aktiviert - zu diesem Zweck wurde eine neue Eigenschaft **DigitalSignatureDetails** hinzugefügt. <sup>24.8</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für Java 24.5 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-5-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 24.6 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-6-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 24.7 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-7-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 24.8 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words für Java 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 verbessert die Erfahrung mit der Verwaltung von Strichfarben, verbessert OLE Objekte und LINQ Berichte und führt eine neue öffentliche Literaturquelle API ein.

Aspose.Words 24.2 erweiterte Diagramme API, Stilverwaltung und LINQ Optionen. Diese Version von Aspose.Words führte auch die Möglichkeit ein, SvgSaveOptions während des Renderns anzugeben, das Laden von Markdown -Dateien flexibler zu steuern und mit Referenztext für Fußnoten und Endnoten zu arbeiten.

Aspose.Words 24.3 führt einen neuen TIFF Lese-/Schreibvorgang und eine Emulation von binären Raster-Operationen für WMF Metadateien ein. Aspose.Words 24.3 erweitert auch weiterhin die Diagramme API.

Aspose.Words 24.4 verbessert Speicherformate, einige Renderoptionen sowie die Arbeit mit digitalen Signaturen.

### Unterstützte Formate <sup>24.4</sup>

Das moderne **WebP**-Bildformat wird jetzt in Aspose.Words unterstützt. Sie können jetzt WebP -Bilder lesen und in Dokumente einfügen sowie Bilder im WebP -Format speichern.

### Rendern und Drucken

#### Strichfarbensteuerung <sup>24.1</sup>

Die Klasse [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) wurde um eine Reihe neuer öffentlicher Eigenschaften erweitert, die sich auf die Verwaltung von Strichfarben beziehen: [ForeThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeThemeColor) und [BackThemeColor](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackThemeColor), [ForeTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getForeTintAndShade) und [BackTintAndShade](https://reference.aspose.com/words/java/com.aspose.words/stroke/#getBackTintAndShade).

#### DrawingML Diagramme API Erweiterung <sup>24.2 / 24.3 / 24.4</sup>

Die **DrawingML Charts API** wird weiterhin erweitert.

#### Schriftarten einbetten, die in @font-face -Regeln deklariert sind <sup>24.4</sup>

Es wurde eine Möglichkeit hinzugefügt, in @font-face -Regeln deklarierte Schriftarten in die Schriftdefinitionen des resultierenden Dokuments einzubetten, indem eine neue [SupportFontFaceRules](https://reference.aspose.com/words/java/com.aspose.words/htmlloadoptions/#getSupportFontFaceRules) -Eigenschaft hinzugefügt wurde.

#### Arbeiten mit Glüh- und Reflexionsformatierung <sup>24.4</sup>

Die Möglichkeit, mit Glüh- und Reflexionsformatierungen für ein Zeichenobjekt zu arbeiten, wurde implementiert.

### Laden und Speichern von Dokumenten

#### Geben Sie beim Rendern SvgSaveOptions an <sup>24.2</sup>

Die Möglichkeit, [SvgSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/svgsaveoptions/) während des Renderns anzugeben, wurde mit [ShapeRenderer](https://reference.aspose.com/words/java/com.aspose.words/shaperenderer/) hinzugefügt.[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) und [OfficeMathRenderer](https://reference.aspose.com/words/java/com.aspose.words/officemathrenderer/).[Save](https://reference.aspose.com/words/java/com.aspose.words/noderendererbase/#save-java.io.OutputStream-com.aspose.words.SvgSaveOptions) Methoden.

#### Leere Zeilen beim Laden von Markdown -Dateien beibehalten <sup>24.2</sup>

Die Möglichkeit, leere Zeilen beim Laden von Markdown -Dateien beizubehalten, wurde hinzugefügt.

#### Ein neuer TIFF Leser/Schreiber <sup>24.3</sup>

Ein neuer TIFF Leser / Schreiber für Aspose.Words für .NET Standard, .NET 6 und höher wurde entwickelt. Aspose.Words für .NET 24.3 Unterstützung für das Lesen von TIFF -Bildern mit JPEG - und alten JPEG -Komprimierungstypen wurde hinzugefügt und die Qualität von Lese- und Schreiboperationen wurde erheblich verbessert.

### Andere

* Die Möglichkeit, den Text des `TextBox` OLE-Steuerelements zu ändern, wurde eingeführt, indem der neuen [TextBoxControl](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/)-Klasse eine neue [Text](https://reference.aspose.com/words/java/com.aspose.words/textboxcontrol/#getText)-Eigenschaft hinzugefügt wurde. 24.1 <sup>24.1</sup>
* Die Bibliographiequellen public API wurde implementiert, indem einige neue hinzugefügt wurden [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/bibliography/), [Source](https://reference.aspose.com/words/java/com.aspose.words/source/), [ContributorCollection](https://reference.aspose.com/words/java/com.aspose.words/contributorcollection/), [Contributor](https://reference.aspose.com/words/java/com.aspose.words/contributor/), [Corporate](https://reference.aspose.com/words/java/com.aspose.words/corporate/), [PersonCollection](https://reference.aspose.com/words/java/com.aspose.words/personcollection/) und [Person](https://reference.aspose.com/words/java/com.aspose.words/person/) -Klassen und einer [SourceType](https://reference.aspose.com/words/java/com.aspose.words/sourcetype/) -Aufzählung sowie durch Hinzufügen einer neuen [Bibliography](https://reference.aspose.com/words/java/com.aspose.words/document/#getBibliography) -Eigenschaft zur [Document](https://reference.aspose.com/words/java/com.aspose.words/document/)-Klasse. <sup>24.1</sup>
* Es wurde ein API bereitgestellt, um den Zugriff auf Typelemente mithilfe der Vorlagensyntax für die LINQ-Berichts-Engine zu beschränken. <sup>24.1</sup>
* Der Klasse [Style](https://reference.aspose.com/words/net/aspose.words/style/) wurden neue öffentliche Eigenschaften [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) und [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) für eine verbesserte Stilverwaltung hinzugefügt. <sup>24.2</sup>
* Die Funktionalität zum Abrufen des tatsächlichen Referenzmarkentexts für Fußnoten und Endnoten wurde um die Eigenschaft [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) und die Methode [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/) erweitert. <sup>24.2</sup>
* Die Kompatibilität mit `Word 2016`-Karten für `LINQ Reporting Engine` wurde aktiviert. <sup>24.2</sup>
* Die Emulation von binären Raster-Operationen für WMF-Metadateien wurde implementiert. <sup>24.3</sup>
* Die Möglichkeit, Signaturoptionen für Dokumente innerhalb von **SaveOptions** zu definieren, wurde durch Hinzufügen einer neuen [DigitalSignatureDetails](https://reference.aspose.com/words/java/com.aspose.words/digitalsignaturedetails/)-Klasse mit neuen öffentlichen Mitgliedern sowie durch Hinzufügen neuer Eigenschaften zu den Klassen [OoxmlSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/docsaveoptions/) und [OdtSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/odtsaveoptions/) aktiviert. <sup>24.4</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für Java 24.1 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-1-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 24.2 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-2-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 24.3 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-3-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 24.4 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2024/aspose-words-for-java-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words für Java 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 erweitert Renderoptionen, Metadatei-Rendering-Emulation und markdown Speicheroptionen.

Aspose.Words 23.10 verbessert die Darstellung, erweitert die Optionen zum Laden und Speichern von Dokumenten und ermöglicht Benutzern das Zusammenführen von Dokumenten auf neue Weise.

Aspose.Words 23.11 erweitert die Arbeit mit Revisionen, XLSX-Format und Schriftarten in Diagrammlegenden um zusätzliche Optionen.

Aspose.Words 23.12 führt neue Eigenschaften und Aufzählungen für die Arbeit mit PDF-Dokumenten, Unterstützung für WebP-Bilder und aktualisierte Hüpfburgbibliothek ein.

### Rendern und Drucken

#### Achsentitel in DrawingML-Diagrammen anpassen <sup>23.9</sup>

Die Möglichkeit, Achsentitel in DrawingML-Diagrammen anzupassen, wurde durch die Implementierung einer neuen öffentlichen Klasse [ChartAxisTitle](https://reference.aspose.com/words/java/com.aspose.words/chartaxistitle/) und [Title](https://reference.aspose.com/words/java/com.aspose.words/chartaxis/#getTitle)-Eigenschaft eingeführt.

#### Bestimmen der vertikalen Position von Schriftarten innerhalb eines Absatzes <sup>23.9</sup>

Es ist jetzt möglich, die vertikale Position von Schriftarten innerhalb eines Absatzes mithilfe der neuen public [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/paragraphformat/#getBaselineAlignment) -Eigenschaft und der neuen [BaselineAlignment](https://reference.aspose.com/words/java/com.aspose.words/baselinealignment/) -Aufzählung zu definieren.

#### Vordergrundfarbsteuerung <sup>23.10</sup>

Die Möglichkeit, die Vordergrundfarbe ohne Modifikatoren abzurufen, wurde den Klassen [Fill](https://reference.aspose.com/words/java/com.aspose.words/fill/) und [Stroke](https://reference.aspose.com/words/java/com.aspose.words/stroke/) über die Eigenschaft **BaseForeColor** hinzugefügt.

#### Erweiterung der Funktionalität von Diagrammen <sup>23.10</sup>

Die Funktionalität der Klassen [ChartDataPointCollection](https://reference.aspose.com/words/java/com.aspose.words/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/java/com.aspose.words/chartseries/) und [ChartFormat](https://reference.aspose.com/words/java/com.aspose.words/chartformat/) wurde um neue Methoden und Eigenschaften erweitert.

#### Automatisches Anpassen und Anpassen eines Bildes an eine Form <sup>23.10</sup>

Eine einfache Möglichkeit, ein Bild automatisch anzupassen und in eine bestimmte Form einzupassen, wurde durch die neue [FitImageToShape](https://reference.aspose.com/words/java/com.aspose.words/imagedata/#fitImageToShape) -Methode bereitgestellt.

#### Standardschriftartformatierung für DrawingML Diagrammlegenden-Einträge <sup>23.11</sup>

Die Möglichkeit, die Standardschriftformatierung für Legendeneinträge von DrawingML-Diagrammen festzulegen, wurde über die Eigenschaft **Font** hinzugefügt. Diese Funktion ermöglicht ein schlankeres und einheitlicheres Erscheinungsbild für Diagrammelemente und verbessert die Gesamtästhetik des Dokuments.

#### Seitenlayout beim Öffnen von PDF in Reader angeben <sup>23.12</sup>

Die Möglichkeit, das Seitenlayout anzugeben, das beim Öffnen eines Dokuments in einem PDF -Reader verwendet werden soll, wurde durch die Einführung einer neuen [PageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/#getPageLayout)-Eigenschaft für die [PdfSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/pdfsaveoptions/)-Klasse und die Einführung einer neuen [PdfPageLayout](https://reference.aspose.com/words/java/com.aspose.words/pdfpagelayout/)-Aufzählung hinzugefügt.

### Laden und Speichern von Dokumenten

#### Angeben eines Ordnernamens zum Erstellen des Bildes URIs in Markdown <sup>23.9</sup>

Die Klasse [MarkdownSaveOptions](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/) wurde um die Eigenschaft [ImagesFolderAlias](https://reference.aspose.com/words/java/com.aspose.words/markdownsaveoptions/#getImagesFolderAlias) erweitert, mit der der Name des Ordners angegeben werden kann, der zum Erstellen des in das Markdown -Dokument geschriebenen Bildes URIs verwendet wird.

#### PDF Ausgabegröße reduzieren <sup>23.10</sup>

Verschiedene PDF -Rendering-Optimierungen zur Reduzierung der Ausgabegröße bei Verwendung von [OptimizeOutput](https://reference.aspose.com/words/java/com.aspose.words/fixedpagesaveoptions/#getOptimizeOutput) -Einstellungen wurden implementiert.

#### Erkennen von Hyperlinks beim Laden von TXT-Dokumenten <sup>23.10</sup>

Die Funktion zum Erkennen von Hyperlinks beim Laden von TXT-Dokumenten wurde durch Hinzufügen einer neuen [DetectHyperlinks](https://reference.aspose.com/words/java/com.aspose.words/txtloadoptions/#getDetectHyperlinks)-Eigenschaft implementiert.

### Andere

- Die Metadatei-Rendering-Emulation zur Bestimmung der Rastergröße wurde speziell für WMF Stiftbreite und EMF kosmetische Stiftbreite implementiert. Um dies zu erreichen, wurde die Eigenschaft **ScaleWmfFontsToMetafileSize** durch die Eigenschaft [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPage) ersetzt und die Eigenschaft [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/java/com.aspose.words/metafilerenderingoptions/#getEmulateRenderingToSizeOnPageResolution) hinzugefügt. <sup>23.9</sup>
- Mit der [InsertDocumentInline](https://reference.aspose.com/words/java/com.aspose.words/documentbuilder/#insertDocumentInline-com.aspose.words.Document-int-com.aspose.words.ImportFormatOptions) -Methode wurde eine vereinfachte Methode zum Einfügen eines Dokuments in ein anderes Dokument an der aktuellen Cursorposition eingeführt. <sup>23.10</sup>
- Die Möglichkeit, auf Stileigenschaften zuzugreifen und diese zu ändern, wurde durch die Einführung der neuen Eigenschaft [Locked](https://reference.aspose.com/words/java/com.aspose.words/style/#getLocked) hinzugefügt. <sup>23.10</sup>
- Den Methoden der Klasse [CompositeNode](https://reference.aspose.com/words/java/com.aspose.words/compositenode/) wurde ein generischer Typparameter hinzugefügt. <sup>23.10</sup>
- Mit den Methoden [Accept](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#accept-com.aspose.words.IRevisionCriteria) und [Reject](https://reference.aspose.com/words/java/com.aspose.words/revisioncollection/#reject-com.aspose.words.IRevisionCriteria) wurde eine Möglichkeit implementiert, zu steuern, wann eine bestimmte Revision akzeptiert / abgelehnt werden soll oder nicht. Diese Erweiterung gibt den Benutzern eine genauere Kontrolle über den Revisionsprozess. <sup>23.11</sup>
- Die Möglichkeit, alle Abschnitte eines Dokuments auf dasselbe XLSX-Arbeitsblatt zu schreiben, wurde durch den neuen [XlsxSectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsectionmode/)-Aufzählungstyp und die neue [SectionMode](https://reference.aspose.com/words/java/com.aspose.words/xlsxsaveoptions/#getSectionMode)-Eigenschaft bereitgestellt. <sup>23.11</sup>
- Unterstützung für WebP-Bilder wurde eingeführt. Bitte beachten Sie, dass diese Funktion nur für verfügbar ist.NetStandart und .NET6+ Versionen. <sup>23.12</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für Java 23.9 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-9-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 23.10 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-10-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 23.11 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-11-release-notes/).

Erfahren Sie mehr über [Aspose.Words für Java 23.12 Versionshinweise](https://releases.aspose.com/words/java/release-notes/2023/aspose-words-for-java-23-12-release-notes/).

{{% /alert %}}

## Siehe auch

{{% alert color="primary" %}}

Diese Seite enthält die neuesten Release-Nachrichten der letzten 2 Jahre. Einzelheiten zu früheren Versionen finden Sie in der [Versionshinweise'](https://releases.aspose.com/words/java/release-notes/) seiten in den entsprechenden Abschnitten.

{{% /alert %}}
