---
title: Was ist neu
second_title: Aspose.Words für .NET
articleTitle: Was ist neu in Aspose.Words für .NET
linktitle: Was ist neu in Aspose.Words für .NET
type: docs
description: "Aspose.Words für .NET erweitert und verbessert sich täglich. Auf dieser Seite erfahren Sie mehr über die großen und interessantesten Funktionen des Produkts."
weight: 10
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /de/net/what-s-new-in-aspose-words-for-net/
timestamp: 2025-06-23-21-02-49
---

Diese Seite beschreibt die interessantesten neuen Aspose.Words Funktionen, die in den letzten Versionen eingeführt wurden.

## Aspose.Words für .NET 25.5, 25.6

Aspose.Words 25.5 verbessert die Diagrammanpassung mit neuen Stiloptionen und verbessert den Markdown-Export, indem es die Kontrolle darüber bietet, wie leere Absätze behandelt werden.

Aspose.Words 25.6 verbessert die Rendergenauigkeit und die Visualisierungsfunktionen durch die Einführung erweiterter Bildexportoptionen, verbesserter MathML -Handhabung und besserer Diagrammdarstellung.

### Dokumente konvertieren, laden und speichern

#### Leere Absätze nach Markdown exportieren <sup>25.5</sup>

Die Möglichkeit zu steuern, wie leere Absätze nach Markdown exportiert werden, wurde durch Hinzufügen der [MarkdownEmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownemptyparagraphexportmode/)-Aufzählung und der [EmptyParagraphExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/emptyparagraphexportmode/)-Eigenschaft eingeführt.

#### Exportieren Sie mehrseitige Dokumente in Rasterbildformate <sup>25.6</sup>

Die Möglichkeit, mehrseitige Dokumente in Rasterbildformate (wie PNG und JPEG) mit [customizable layouts](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/) - Horizontal, Vertikal oder Raster – zu exportieren, wurde durch die Erweiterung der Bildexportfunktionalität eingeführt.

### Rendering

#### Festlegen des Diagrammstils <sup>25.5</sup>

Die Möglichkeit, den Diagrammstil festzulegen, wurde durch Hinzufügen der [ChartStyle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartstyle/)-Aufzählung und der [Style](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/style/)-Eigenschaft eingeführt.

#### Verbindungslinien in MathML -Ausdrücken rendern <sup>25.6</sup>

Die Darstellung von Verbindungslinien in MathML-Ausdrücken wurde implementiert, um eine genauere und visuell konsistentere Anzeige mathematischer Formeln zu gewährleisten.

#### Rendering von Legenden für Wasserfalldiagramme <sup>25.6</sup>

Die Darstellung von Legenden für ["Waterfall" charts](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriestype/) wurde eingeführt, um die Datentransparenz zu erhöhen und die Interpretierbarkeit dieser Diagramme zu verbessern.

### Andere

* Die Möglichkeit, mathematische Formeln mit mehreren Schrägstrichen zu umbrechen, wurde verbessert, um die Layoutklarheit und die Lesbarkeit von Formeln zu verbessern. <sup>25.6</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für .NET 25.5 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-5-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 25.6 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-6-release-notes/).

{{% /alert %}}

## Aspose.Words für .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 führt eine AI-basierte Grammatikprüfung ein und verbessert das Speichern von Dokumenten mit erweiterten Optionen für die Formate HTML, SVG und Markdown.

Aspose.Words 25.2 führt die Textzusammenfassung mit Anthropic AI-Modellen ein, fügt MsWorks-Formatunterstützung hinzu, verbessert die typografische Steuerung und verbessert die PDF-Struktur und die Listenbehandlung.

Aspose.Words 25.3 verbessert eine AI-basierte Grammatikprüfung und Schriftauswahl mit der UpdateAmbiguousTextFont-Eigenschaft sowie den Export von PDF-Anhängen.

Aspose.Words 25.4 bietet Unterstützung für neue Papierformate, ermöglicht eine erweiterte HTML Exportkontrolle, verbessert die Handhabung von Wasserzeichen und verbessert die Benutzerfreundlichkeit von LowCode API.

### AI-betriebene Funktionen

#### Dokument AI Grammatikprüfung

* Die Möglichkeit, die Grammatik des bereitgestellten Dokuments mithilfe generativer OpenAI -Modelle zu überprüfen, wurde durch Hinzufügen einer neuen [CheckGrammar](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/checkgrammar/) -Methode eingeführt. <sup>25.1</sup>
* Die AI-basierte Grammatikprüfungsfunktion wurde aktualisiert, um alle in der [AiModelType](https://reference.aspose.com/words/net/aspose.words.ai/aimodeltype/) -Aufzählung verfügbaren Modelle zu unterstützen. <sup>25.3</sup>

#### Zusammenfassung mit Anthropic generativen Sprachmodellen <sup>25.2</sup>

Die Textzusammenfassung mit Anthropic generativen Sprachmodellen wurde durch die Einführung einer neuen öffentlichen Klasse [AnthropicAiModel](https://reference.aspose.com/words/net/aspose.words.ai/anthropicaimodel/) ermöglicht.

### Low Code

#### Low Code API Benutzerfreundlichkeit <sup>25.4</sup>

Die Benutzerfreundlichkeit von **LowCode API** wurde erheblich verbessert, wodurch die Dokumentenverarbeitung vereinfacht und der Bedarf an sich wiederholendem Code verringert wird.

### Unterstützte Formate <sup>25.2</sup>

Ab Version 25.2 wurde die Kompatibilität mit dem neuen MsWorks Ladeformat für Microsoft Werksdokumente hinzugefügt.

### Dokumente konvertieren, laden und speichern

#### Verbessertes Speichern in den Formaten HTML und SVG <sup>25.1</sup>

Das Speichern in den Formaten HTML und SVG wurde verbessert, indem den Klassen [HtmlFixedSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlfixedsaveoptions/) und [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/) Eigenschaften **IdPrefix** und **RemoveJavaScriptFromLinks** hinzugefügt wurden.

#### Stellen Sie die Bildauflösung und den OfficeMath -Ausgabemodus beim Speichern auf Markdown ein <sup>25.1</sup>

* Der Klasse [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) wurde eine neue Option [ImageResolution](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imageresolution/) hinzugefügt, um die Bildauflösung festzulegen.
* Eine neue [OfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/officemathexportmode/) -Option und [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownofficemathexportmode/) -Aufzählung wurden der [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) -Klasse hinzugefügt, um den OfficeMath -Ausgabemodus festzulegen.
* Die Möglichkeit, ein Bildwasserzeichen aus einem Stream zu setzen, wurde eingeführt, indem der [SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage_2) -Methode eine neue Überladung hinzugefügt wurde. <sup>25.4</sup>

### Rendering

#### Verbesserte typografische Kontrolle <sup>25.2</sup>

Die Eigenschaft [NumberSpacing](https://reference.aspose.com/words/net/aspose.words/font/numberspacing/) wurde für eine verbesserte typografische Kontrolle hinzugefügt.

#### Steuern der Schriftauswahl für mehrdeutige Zeichen <sup>25.3</sup>

Der Klasse [SaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/) wurde eine neue öffentliche Eigenschaft [UpdateAmbiguousTextFont](https://reference.aspose.com/words/net/aspose.words.saving/saveoptions/updateambiguoustextfont/) hinzugefügt, um die Schriftauswahl entsprechend dem verwendeten Zeichencode zu steuern.

#### Optionen für das Papierformat <sup>25.4</sup>

Die Möglichkeit, die Papierformate JIS B4 und JIS B5 zu verwenden, wurde eingeführt, indem der [PaperSize](https://reference.aspose.com/words/net/aspose.words/papersize/)-Aufzählung neue Werte hinzugefügt wurden.

#### HTML Ausgabesteuerung <sup>25.4</sup>

Die Möglichkeit, JavaScript während des HTML-Exports aus dem Hyperlink URLs zu entfernen, wurde durch Hinzufügen der Eigenschaft [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/removejavascriptfromlinks/) eingeführt.

### Andere

* PDF logische Struktur wurde mit Unterstützung für TOA, BIBLIOGRAPHY und INDEX Felder verbessert. <sup>25.2</sup>
* Die [AddSingleLevelList](https://reference.aspose.com/words/net/aspose.words.lists/listcollection/addsinglelevellist/) -Methode wurde für eine verbesserte Listenbehandlung eingeführt. <sup>25.2</sup>
* Eine neue Eigenschaft [AttachmentsEmbeddingMode](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/attachmentsembeddingmode/) wurde hinzugefügt, um **EmbedAttachments** zu ersetzen, um den Export von PDF-Anhängen zu verbessern. Außerdem wurden der [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) -Aufzählung neue Werte hinzugefügt, um Anhänge der PDF/A -Version zu unterstützen. Außerdem werden Anhänge jetzt mit Verschlüsselung unterstützt. <sup>25.3</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für .NET 25.1 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-1-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 25.2 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-2-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 25.3 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-3-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 25.4 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2025/aspose-words-for-net-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words für .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 führt die Einfügung von group shape und StructuredDocumentTag über DocumentBuilder ein, verbessert die Darstellung von Radialdiagrammen mit Graduierungen, verbessert digitale Signaturen mit XAdES-EPES-Unterstützung, fügt die Unterstreichungserkennung von Markdown hinzu und bietet Zugriff auf Fußnoten-/Endnotentrennzeichen.

Aspose.Words 24.10 führt eine erweiterte ActiveX-Steuerungsunterstützung mit CommandButton -Erstellung, eine neue Steuerung der Formsichtbarkeit, die Möglichkeit zu group shapes, einen verbesserten Markdown-Export für Tabellen, Diagrammformatierung für Pie- und Doughnut-Diagramme, eine bessere Big5-Codierungsbehandlung und Unterstützung für veraltete taiwanesische Schriftarten ein.

Aspose.Words 24.11 führt die AI-basierte Dokumentzusammenfassung, erweiterte Renderoptionen, verbesserten Zugriff auf Dokumenteigenschaften und ActiveX-Steueruntertitelung ein.

Aspose.Words 24.12 führt eine anpassbare Platzierung von Datenetiketten, eine von Google AI unterstützte Textübersetzung, erweiterte Mail Merge Bereinigungsoptionen und neue LowCode Verarbeitungsklassen ein.

### AI-betriebene Funktionen

#### Dokumentzusammenfassung mit OpenAI und Google <sup>24.11</sup>

Unterstützung für die Dokumentzusammenfassung mit generativen **OpenAI**- und **Google**-Sprachmodellen wurde integriert, indem der [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)-Namespace mit seinen öffentlichen Mitgliedern hinzugefügt wurde.

#### Textübersetzung mit den generativen Sprachmodellen von Google <sup>24.12</sup>

Die Möglichkeit, Text mit den generativen Sprachmodellen von Google zu übersetzen, wurde in Aspose.Words implementiert, indem die [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/)-Methode und die [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/)-Aufzählung zum [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/)-Namespace hinzugefügt wurden.

### Low Code <sup>24.12</sup>

Neue LowCode Klassen wie [Comparer](https://reference.aspose.com/words/net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/net/aspose.words.lowcode/splitter/) usw. wurde eingeführt und bietet eine Reihe von Methoden, die die perfekte Balance zwischen Einfachheit und Flexibilität für die Dokumentenverarbeitung finden.

### Rendern und Drucken

#### Graduierungen auf Radialdiagrammen <sup>24.9</sup>

Die Darstellung von Abstufungen auf Radialdiagrammen wurde implementiert.

#### CommandButton ActiveX Bedienelemente <sup>24.10</sup>

Die Möglichkeit, CommandButton ActiveX-Steuerelemente zu erstellen, wurde durch Hinzufügen einer neuen öffentlichen Methode [InsertForms2OleControl](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertforms2olecontrol/) und einer neuen öffentlichen Klasse [Forms2OleControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/) eingeführt.

#### Sichtbarkeit der Form steuern <sup>24.10</sup>

Eine neue öffentliche Eigenschaft [Hidden](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/hidden/) wurde hinzugefügt, um die Sichtbarkeit von Formen zu steuern.

#### Änderungen in den Diagrammen Pie und Doughnut <sup>24.10</sup>

Dem Formatieren von Pie- und Doughnut-Diagrammen wurden mehrere neue öffentliche Eigenschaften hinzugefügt.

#### Steuern Sie das Rendern von PDF-Auswahlformularfeldrändern <sup>24.11</sup>

Eine neue Option zur Steuerung der Darstellung von PDF-Auswahlformularfeldrändern wurde implementiert, indem eine neue öffentliche Option [RenderChoiceFormFieldBorder](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/renderchoiceformfieldborder/) hinzugefügt wurde.

#### Formatcodes für Diagrammdaten abrufen und festlegen <sup>24.11</sup>

Die Möglichkeit, Formatcodes für Diagrammdaten abzurufen und festzulegen, wurde hinzugefügt, indem die Eigenschaft [FormatCode](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/formatcode/) in den Klassen [ChartXValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartyvaluecollection/) und [BubbleSizeCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/bubblesizecollection/) implementiert wurde.

#### Histogrammdiagramme mit Bins und Beschriftungen rendern <sup>24.11</sup>

Die Darstellung von Histogrammdiagrammen wurde verbessert, indem eine bestimmte Anzahl von Behältern und Beschriftungen zugelassen wurde.

#### Anpassen der Platzierung von Datenbeschriftungen <sup>24.12</sup>

Die Möglichkeit, die Platzierung von Datenbeschriftungen anzupassen, wurde hinzugefügt, indem den Klassen [ChartDataLabel](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabel/) und [ChartDataLabelCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatalabelcollection/) neue Eigenschaften hinzugefügt wurden.

### Dokumente konvertieren, laden und speichern

#### Formatierung beim Laden von Markdown-Dateien unterstreichen <sup>24.9</sup>

Die Option, Unterstreichungsformatierungen beim Laden von Markdown-Dokumenten zu erkennen, wurde durch Hinzufügen einer neuen öffentlichen Eigenschaft [ImportUnderlineFormatting](https://reference.aspose.com/words/net/aspose.words.loading/markdownloadoptions/importunderlineformatting/) integriert.

#### Tabellen beim Speichern in Markdown als HTML exportieren <sup>24.10</sup>

Eine Option zum Exportieren von Tabellen als HTML beim Speichern von Dokumenten im Markdown-Format wurde implementiert, indem eine neue öffentliche Eigenschaft [ExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/exportashtml/) und eine Aufzählung [MarkdownExportAsHtml](https://reference.aspose.com/words/net/aspose.words.saving/markdownexportashtml/) hinzugefügt wurden.

#### Export PDF mit aktualisierter logischer Struktur <sup>24.11</sup>

Der PDF-Export wurde verbessert, indem Tabellentiteleigenschaften als Titel für logische PDF-Strukturelemente aufgenommen wurden.

### Mail Merge und Berichterstattung

#### Leere Tabellen während Mail Merge entfernen <sup>24.12</sup>

Der [MailMergeCleanupOptions](https://reference.aspose.com/words/net/aspose.words.mailmerging/mailmergecleanupoptions/)-Aufzählung wurde eine neue **RemoveEmptyTables**-Option hinzugefügt, um die Mail Merge-Ausgabe zu verfeinern.

### Digitale Signaturen

#### Dokumente mit XAdES-EPES signieren <sup>24.9</sup>

Die Möglichkeit, Dokumente mit XAdES-EPES Level XML-DSig Signaturen zu signieren, wurde eingeführt, indem eine neue öffentliche Eigenschaft [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/signoptions/xmldsiglevel/) und eine neue öffentliche Aufzählung [XmlDsigLevel](https://reference.aspose.com/words/net/aspose.words.digitalsignatures/xmldsiglevel/) hinzugefügt wurden.

### Andere

* Eine neue öffentliche Methode [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/) wurde zu group shapes hinzugefügt. <sup>24.9</sup>
* Eine neue öffentliche Methode [InsertStructuredDocumentTag](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertstructureddocumenttag/) wurde hinzugefügt, um **StructuredDocumentTags** in ein Dokument einzufügen. <sup>24.9</sup>
* Der öffentliche Zugriff auf Fußnoten- / Endnotentrennzeichen wurde durch Hinzufügen einiger öffentlicher Klassen und Eigenschaften ermöglicht. <sup>24.9</sup>
* Die Möglichkeit, einzelne Formen group shapes zu gruppieren und sowohl Formen als auch group shapes direkt zu gruppieren, wurde durch Hinzufügen der [InsertGroupShape](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertgroupshape/#insertgroupshape_1) -Methode eingeführt. <sup>24.10</sup>
* Die Handhabung der Big5-Codierung für TrueType cmap-Tabellen wurde verbessert. <sup>24.10</sup>
* Die Unterstützung für veraltete taiwanesische Schriftarten wurde verbessert. <sup>24.10</sup>
* Um auf erweiterte Dokumenteigenschaften zuzugreifen, wurden der Klasse [BuiltInDocumentProperties](https://reference.aspose.com/words/net/aspose.words.properties/builtindocumentproperties/) schreibgeschützte Eigenschaften hinzugefügt. <sup>24.11</sup>
* Das Festlegen von Beschriftungen für ActiveX-Steuerelemente wurde aktiviert, indem der Eigenschaft [Forms2OleControl.Caption](https://reference.aspose.com/words/net/aspose.words.drawing.ole/forms2olecontrol/caption/) ein neuer öffentlicher Setter hinzugefügt wurde. <sup>24.11</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für .NET 24.9 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-9-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 24.10 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-10-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 24.11 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-11-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 24.12 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words für .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 erweitert die Optionen für Assemblys, verbessert die Renderfunktionen und erweitert einige andere Optionen.

Aspose.Words 24.6 verbessert die Renderoptionen, erweitert die Such- und Vergleichsfunktionen und erweitert mehrere andere Funktionen.

Aspose.Words 24.7 ändert die Arbeitsweise mit ActiveX, erweitert die Renderfunktionen sowie den Export in die Formate Markdown und XLSX.

Aspose.Words 24.8 verbessert die Diagrammanpassung mit präziser Kontrolle über Achsenbeschriftungen, erweitert die Schriftartverwaltung, verbessert die Handhabung der Dokumentstruktur und fügt neue Funktionen für HTML/XAML-Export, PDF-Funktionalität, Dokumentkonvertierung und digitale Signaturen hinzu.

### Unterstützte Formate

Ab Version 24.7 wird der Export nach PDF/UA-2 unterstützt, um die Zugänglichkeit für Benutzer mit Behinderungen zu gewährleisten.

### Plattform <sup>24.5</sup>

.NET 7.0/8.0 Assemblys wurden in das Aspose.Words NuGet-Paket aufgenommen.

### Rendern und Drucken

#### Änderungen in Diagrammen, Formen und DrawingML <sup>24.5</sup>

* DrawingML Effektrendering für SVG Grafiken, das die bisherige, auf Bilder beschränkte Funktionalität erweitert, wurde implementiert.
* Unterstützung für das Erstellen von Kombinationsdiagrammen und das Anpassen von Eigenschaften wie Spaltenbreite, Überlappung und Blasenskalierung innerhalb von Reihengruppen wurde eingeführt, indem die Klassen [ChartSeriesGroup](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroup/) und [ChartSeriesGroupCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseriesgroupcollection/) sowie die Eigenschaft [SeriesGroups](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chart/seriesgroups/) hinzugefügt wurden.
* Die Funktionalität zum Manipulieren des SoftEdge -Effekts von Formen wurde durch Hinzufügen der [SoftEdgeFormat](https://reference.aspose.com/words/net/aspose.words.drawing/softedgeformat/) -Klasse implementiert.
* Die Möglichkeit, Anpassungswerte von Formen zu ändern, wurde durch Hinzufügen der öffentlichen Klassen [AdjustmentCollection](https://reference.aspose.com/words/net/aspose.words.drawing/adjustmentcollection/) und [Adjustment](https://reference.aspose.com/words/net/aspose.words.drawing/adjustment/) und der Eigenschaft [Adjustments](https://reference.aspose.com/words/net/aspose.words.drawing/shape/adjustments/) implementiert.

#### Änderungen in Diagrammen, Formen und Zeichnungen <sup>24.6</sup>

* Die Diagrammfunktionen wurden verbessert. Sie können jetzt eine größere Auswahl an Diagrammen erstellen, einschließlich *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* diagramme, *Box & Whisker* Diagramme, *Waterfalls* und *Funnels*. So können Sie Ihre Daten vielfältiger und informativer visualisieren.
* Die Farbsteuerung für die Schattenformatierung wurde verbessert. Sie können das Erscheinungsbild Ihrer Dokumente genauer steuern, indem Sie auf Schattenfarben zugreifen.
* Die Leistungssteigerung für das Hintergrundrendern wurde verbessert. Dank der nativen Kacheltechnologie können Sie das Rendern von Hintergründen mit kleinen Elementen erheblich beschleunigen.
* Realistische Verläufe für Formen wurden hinzugefügt. Sie können jetzt DML -Formen mit nichtlinearen Verläufen erstellen, die den visuellen Stil von Microsoft Word nachahmen, um ein polierteres Aussehen zu erzielen.

#### Anpassung der Diagrammdatenetiketten <sup>24.7</sup>

Die Möglichkeit, Diagrammdatenbeschriftungen wie **Orientation** und **Rotation** anzupassen, wurde hinzugefügt.

#### Benutzerdefiniertes Nummernstyling für Listenebenen <sup>24.7</sup>

Ein Setter für die öffentliche Eigenschaft [CustomNumberStyleFormat](https://reference.aspose.com/words/net/aspose.words.lists/listlevel/customnumberstyleformat/) wurde hinzugefügt. Sie können jetzt einen benutzerdefinierten Nummernstil für Listenebenen definieren.

#### Änderungen bei der Arbeit mit ActiveX <sup>24.7</sup>

* Die Eigenschaften von ActiveX-Objekten können jetzt geändert werden, sodass Sie mehr Kontrolle über ihr Verhalten haben.
* Die Möglichkeit, den Wert des Optionsfelds ActiveX zu ändern, um eine dynamische Interaktion zu ermöglichen, wurde hinzugefügt.
* Die Möglichkeit, eine ActiveX checkbox auf "aktiviert" oder "deaktiviert" umzuschalten, wurde hinzugefügt.

#### Kontrolle über die Ausrichtung und Drehung der Tick-Beschriftungen der Diagrammachse <sup>24.8</sup>

Eine präzise Steuerung der Ausrichtung und Drehung von Teilstrichbeschriftungen der Diagrammachse wurde hinzugefügt, um die Diagrammanpassung komfortabler zu gestalten – die Klasse [AxisTickLabels](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/) wurde um die neuen Eigenschaften [Orientation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/orientation/) und [Rotation](https://reference.aspose.com/words/net/aspose.words.drawing.charts/axisticklabels/rotation/) erweitert.

#### Ersetzen des umgekehrten Schrägstrichs durch das Yen-Zeichen <sup>24.8</sup>

Der abwärtskompatible HTML- und XAML-Export zum Ersetzen des Backslash-Zeichens durch das Yen-Zeichen wurde verbessert. Um dies zu erreichen, wurde den Klassen [HtmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions/) und [XamlFlowSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xamlflowsaveoptions/) die Eigenschaft **ReplaceBackslashWithYenSign** hinzugefügt.

#### SDT-Tags als Formularfeldnamen beim Export nach PDF verwenden <sup>24.8</sup>

Der PDF-Export mit Unterstützung für die Verwendung von SDT-Tags als Formularfeldnamen wurde verbessert, indem der [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)-Klasse eine neue [UseSdtTagAsFormFieldName](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/usesdttagasformfieldname/)-Eigenschaft hinzugefügt wurde.

### Dokumente konvertieren, laden und speichern

#### Exportieren von Links in das Markdown -Format <sup>24.7</sup>

Die Möglichkeit, den Export von Links im Format Markdown zu steuern, wurde durch die Implementierung der Eigenschaft [LinkExportMode](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/linkexportmode/) hinzugefügt.

#### LowCode 24.8 <sup>24.8</sup>

Es wurde eine neue [LowCode.Converter](https://reference.aspose.com/words/net/aspose.words.lowcode/converter/) -Klasse eingeführt, die eine Reihe von Methoden zum Konvertieren verschiedener Dokumenttypen mit einer einzigen Codezeile bereitstellt.

### Suchen und vergleichen

#### Erweiterte Vergleichsoptionen <sup>24.6</sup>
Die Möglichkeit, Datenanalyse-Workflows mit verbesserten Vergleichsfunktionen zu rationalisieren, wurde hinzugefügt. Dies beinhaltet eine neue [IgnoreStoreItemId](https://reference.aspose.com/words/net/aspose.words.comparing/advancedcompareoptions/ignorestoreitemid/) -Option und eine neu gestaltete Oberfläche für erweiterte Vergleiche.

### Andere

* Die Funktion zum Entfernen leerer Seiten aus einem Dokument wurde durch Hinzufügen der [RemoveBlankPages](https://reference.aspose.com/words/net/aspose.words/document/removeblankpages/) -Methode implementiert. <sup>24.5</sup>
* Die Möglichkeit, das Vorhandensein von VBA Makros zu überprüfen, ohne ein Dokument zu laden, wurde durch Hinzufügen der Eigenschaft [HasMacros](https://reference.aspose.com/words/net/aspose.words/fileformatinfo/hasmacros/) bereitgestellt. <sup>24.5</sup>
* Die Beibehaltung der Quellennummerierung beim Einfügen eines Dokuments mit der LINQ Reporting Engine wird jetzt unterstützt. <sup>24.5</sup>
* Eine neue [DateTimeUtc](https://reference.aspose.com/words/net/aspose.words/comment/datetimeutc/) -Eigenschaft wurde hinzugefügt - dies bietet einen genaueren Zeitstempel für Kommentare, was die Organisation und Rückverfolgbarkeit verbessert. <sup>24.6</sup>
* Die LINQ Reporting Engine wurde verbessert. Das selektive Entfernen leerer Absätze und die Definition benutzerdefinierter Nachrichten für fehlende Objektmitglieder wurden vorgenommen, was zu saubereren und informativeren Berichten führt. <sup>24.6</sup>
* Das Datums-/Uhrzeitformat wird jetzt automatisch für den nahtlosen Export in das XLSX-Format erkannt. <sup>24.7</sup>
* Die öffentliche Eigenschaft [IsProtected](https://reference.aspose.com/words/net/aspose.words.vba/vbaproject/isprotected/), mit der Sie überprüfen können, ob ein VBA-Projekt geschützt ist, wurde hinzugefügt. <sup>24.7</sup>
* Die Schriftarteninformationen wurden um die Eigenschaft **EmbeddingLicensingRights** erweitert, die den Klassen [FontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/fontinfo/) und [PhysicalFontInfo](https://reference.aspose.com/words/net/aspose.words.fonts/physicalfontinfo/) hinzugefügt wurde. <sup>24.8</sup>
* Es wurde eine Möglichkeit hinzugefügt, Kopf- und Fußzeilen von Abschnitten effizient zu löschen und gleichzeitig Wasserzeichen beizubehalten, um genauer mit der Dokumentstruktur zu arbeiten. Verwenden Sie die neue öffentliche Methode [ClearHeadersFooters](https://reference.aspose.com/words/net/aspose.words/section/clearheadersfooters/), um Kopf- und Fußzeilen von Abschnitten zu löschen. <sup>24.8</sup>
* Das digitale Signieren von XPS-Dokumenten mit [XpsSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/) wurde aktiviert - zu diesem Zweck wurde eine neue Eigenschaft [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/xpssaveoptions/digitalsignaturedetails/) hinzugefügt. <sup>24.8</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für .NET 24.5 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-5-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 24.6 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-6-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 24.7 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-7-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 24.8 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words für .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 verbessert die Erfahrung rund um die Verwaltung von Strichfarben, verbessert OLE Objekte und LINQ Berichte und führt ein neues `Bibliography Sources` öffentliches API ein.

Aspose.Words 24.2 erweiterte Diagramme API, Stilverwaltung und LINQ Optionen. Diese Version von Aspose.Words führte auch die Möglichkeit ein, SvgSaveOptions während des Renderns anzugeben, das Laden von Markdown -Dateien flexibler zu steuern und mit Referenztext für Fußnoten und Endnoten zu arbeiten.

Aspose.Words 24.3 führt einen neuen TIFF Lese-/Schreibvorgang und eine Emulation von binären Raster-Operationen für WMF Metadateien ein. Aspose.Words 24.3 erweitert auch weiterhin die Diagramme API.

Aspose.Words 24.4 verbessert Speicherformate, einige Renderoptionen sowie die Arbeit mit digitalen Signaturen.

### Unterstützte Formate <sup>24.4</sup>

Das moderne **WebP**-Bildformat wird jetzt in unterstützt Aspose.Words für .NET Framework 4.6.2 und höher. Sie können jetzt WebP -Bilder lesen und in Dokumente einfügen sowie Bilder im WebP -Format speichern.

Bitte beachten Sie, dass WebP derzeit nur in .NET Standard und .NET Framework v4.6.2 und höher verfügbar ist.

### Rendern und Drucken

#### Strichfarbensteuerung <sup>24.1</sup>

Die Klasse [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) wurde um eine Reihe neuer öffentlicher Eigenschaften erweitert, die sich auf die Verwaltung von Strichfarben beziehen: [ForeThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/forethemecolor/) und [BackThemeColor](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/foretintandshade/) und [BackTintAndShade](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/backtintandshade/).

#### DrawingML Diagramme API Erweiterung <sup>24.2 / 24.3 / 24.4</sup>

Die **DrawingML Charts API** wird weiterhin erweitert.

#### Schriftarten einbetten, die in @font-face -Regeln deklariert sind <sup>24.4</sup>

Es wurde eine Möglichkeit hinzugefügt, in @font-face -Regeln deklarierte Schriftarten in die Schriftdefinitionen des resultierenden Dokuments einzubetten, indem eine neue [SupportFontFaceRules](https://reference.aspose.com/words/net/aspose.words.loading/htmlloadoptions/supportfontfacerules/) -Eigenschaft hinzugefügt wurde.

#### Arbeiten mit Glüh- und Reflexionsformatierung <sup>24.4</sup>

Die Möglichkeit, mit Glüh- und Reflexionsformatierungen für ein Zeichenobjekt zu arbeiten, wurde implementiert.

### Laden und Speichern von Dokumenten

#### Geben Sie beim Rendern SvgSaveOptions an <sup>24.2</sup>

Die Möglichkeit, [SvgSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/svgsaveoptions/) während des Renderns anzugeben, wurde mit [ShapeRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/shaperenderer/) hinzugefügt.[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) und [OfficeMathRenderer](https://reference.aspose.com/words/net/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/net/aspose.words.rendering/noderendererbase/save/) methoden.

#### Leere Zeilen beim Laden von Markdown -Dateien beibehalten <sup>24.2</sup>

Die Möglichkeit, leere Zeilen beim Laden von Markdown -Dateien beizubehalten, wurde hinzugefügt.

#### Ein neuer TIFF Leser/Schreiber <sup>24.3</sup>

Ein neuer TIFF Leser / Schreiber für Aspose.Words für .NET Standard, .NET 6 und höher wurde entwickelt. Aspose.Words für .NET 24.3 Unterstützung für das Lesen von TIFF -Bildern mit JPEG - und alten JPEG -Komprimierungstypen wurde hinzugefügt und die Qualität von Lese- und Schreiboperationen wurde erheblich verbessert.

### Andere

* Die Möglichkeit, den Text des `TextBox` OLE-Steuerelements zu ändern, wurde eingeführt, indem der neuen [TextBoxControl](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/)-Klasse eine neue [Text](https://reference.aspose.com/words/net/aspose.words.drawing.ole/textboxcontrol/text/)-Eigenschaft hinzugefügt wurde. <sup>24.1</sup>
* Die öffentlichen Literaturquellen API wurden durch Hinzufügen eines neuen Namespace [Aspose.Words.Bibliography](https://reference.aspose.com/words/net/aspose.words.bibliography/) mit seinen neuen Klassen und Aufzählungen und durch Hinzufügen einer neuen [Bibliography](https://reference.aspose.com/words/net/aspose.words/document/bibliography/) -Eigenschaft zur [Document](https://reference.aspose.com/words/net/aspose.words/document/) -Klasse implementiert. <sup>24.1</sup>
* Es wurde ein API bereitgestellt, um den Zugriff auf Typmitglieder mithilfe der Vorlagensyntax für `LINQ Reporting Engine` zu beschränken. <sup>24.1</sup>
* Der Klasse [Style](https://reference.aspose.com/words/net/aspose.words/style/) wurden neue öffentliche Eigenschaften [Priority](https://reference.aspose.com/words/net/aspose.words/style/priority/), [UnhideWhenUsed](https://reference.aspose.com/words/net/aspose.words/style/unhidewhenused/) und [SemiHidden](https://reference.aspose.com/words/net/aspose.words/style/semihidden/) für eine verbesserte Stilverwaltung hinzugefügt. <sup>24.2</sup>
* Die Funktionalität zum Abrufen des tatsächlichen Referenzmarkentexts für Fußnoten und Endnoten wurde um die Eigenschaft [ActualReferenceMark](https://reference.aspose.com/words/net/aspose.words.notes/footnote/actualreferencemark/) und die Methode [UpdateActualReferenceMarks](https://reference.aspose.com/words/net/aspose.words/document/updateactualreferencemarks/) erweitert. <sup>24.2</sup>
* Die Kompatibilität mit `Word 2016`-Karten für `LINQ Reporting Engine` wurde aktiviert. <sup>24.2</sup>
* Die Emulation von binären Raster-Operationen für WMF-Metadateien wurde implementiert. <sup>24.3</sup>
* Die Möglichkeit, Signaturoptionen für Dokumente innerhalb von **SaveOptions** zu definieren, wurde durch Hinzufügen einer neuen [DigitalSignatureDetails](https://reference.aspose.com/words/net/aspose.words.saving/digitalsignaturedetails/)-Klasse mit neuen öffentlichen Mitgliedern sowie durch Hinzufügen neuer Eigenschaften zu den Klassen [OoxmlSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/docsaveoptions/) und [OdtSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/odtsaveoptions/) aktiviert. <sup>24.4</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für .NET 24.1 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-1-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 24.2 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-2-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 24.3 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-3-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 24.4 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2024/aspose-words-for-net-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words für .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 erweitert Renderoptionen, Metadatei-Rendering-Emulation und markdown Speicheroptionen.

Aspose.Words 23.10 verbessert die Darstellung, erweitert die Optionen zum Laden und Speichern von Dokumenten und ermöglicht Benutzern das Zusammenführen von Dokumenten auf neue Weise.

Aspose.Words 23.11 erweitert die Arbeit mit Revisionen, XLSX-Format und Schriftarten in Diagrammlegenden um zusätzliche Optionen.

Aspose.Words 23.12 führt neue Eigenschaften und Aufzählungen für die Arbeit mit PDF- und OOXML-Dokumenten sowie Unterstützung für WebP-Bilder ein.

### Rendern und Drucken

#### Achsentitel in DrawingML-Diagrammen anpassen <sup>23.9</sup>

Die Möglichkeit, Achsentitel in DrawingML-Diagrammen anzupassen, wurde durch die Implementierung einer neuen öffentlichen Klasse [ChartAxisTitle](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxistitle/) und [Title](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartaxis/title/)-Eigenschaft eingeführt.

#### Bestimmen der vertikalen Position von Schriftarten innerhalb eines Absatzes <sup>23.9</sup>

Es ist jetzt möglich, die vertikale Position von Schriftarten innerhalb eines Absatzes mithilfe der neuen public [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/paragraphformat/baselinealignment/) -Eigenschaft und der neuen [BaselineAlignment](https://reference.aspose.com/words/net/aspose.words/baselinealignment/) -Aufzählung zu definieren.

#### Vordergrundfarbsteuerung <sup>23.10</sup>

Die Möglichkeit, die Vordergrundfarbe ohne Modifikatoren abzurufen, wurde den Klassen [Fill](https://reference.aspose.com/words/net/aspose.words.drawing/fill/) und [Stroke](https://reference.aspose.com/words/net/aspose.words.drawing/stroke/) über die Eigenschaft **BaseForeColor** hinzugefügt.

#### Erweiterung der Funktionalität von Diagrammen <sup>23.10</sup>

Die Funktionalität der Klassen [ChartDataPointCollection](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartseries/) und [ChartFormat](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartformat/) wurde um neue Methoden und Eigenschaften erweitert.

#### Automatisches Anpassen und Anpassen eines Bildes an eine Form <sup>23.10</sup>

Eine einfache Möglichkeit, ein Bild automatisch anzupassen und in eine bestimmte Form einzupassen, wurde durch die neue [FitImageToShape](https://reference.aspose.com/words/net/aspose.words.drawing/imagedata/fitimagetoshape/) -Methode bereitgestellt.

#### Standardschriftartformatierung für DrawingML Diagrammlegenden-Einträge <sup>23.11</sup>

Die Möglichkeit, die Standardschriftformatierung für Legendeneinträge von DrawingML-Diagrammen festzulegen, wurde über die Eigenschaft [Font](https://reference.aspose.com/words/net/aspose.words.drawing.charts/chartlegend/font/) hinzugefügt. Diese Funktion ermöglicht ein schlankeres und einheitlicheres Erscheinungsbild für Diagrammelemente und verbessert die Gesamtästhetik des Dokuments.

#### Seitenlayout beim Öffnen von PDF in Reader angeben <sup>23.12</sup>

Die Möglichkeit, das Seitenlayout anzugeben, das beim Öffnen eines Dokuments in einem PDF -Reader verwendet werden soll, wurde durch die Einführung einer neuen [PageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/pagelayout/)-Eigenschaft für die [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/)-Klasse und die Einführung einer neuen [PdfPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/pdfpagelayout/)-Aufzählung hinzugefügt.

### Laden und Speichern von Dokumenten

#### Angeben eines Ordnernamens zum Erstellen des Bildes URIs in Markdown <sup>23.9</sup>

Die Klasse [MarkdownSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/) wurde um die Eigenschaft [ImagesFolderAlias](https://reference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/imagesfolderalias/) erweitert, mit der der Name des Ordners angegeben werden kann, der zum Erstellen des in das Markdown -Dokument geschriebenen Bildes URIs verwendet wird.

#### PDF Ausgabegröße reduzieren <sup>23.10</sup>

Verschiedene PDF -Rendering-Optimierungen zur Reduzierung der Ausgabegröße bei Verwendung von [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) -Einstellungen wurden implementiert.

#### Erkennen von Hyperlinks beim Laden von TXT-Dokumenten <sup>23.10</sup>

Die Funktion zum Erkennen von Hyperlinks beim Laden von TXT-Dokumenten wurde durch Hinzufügen einer neuen [DetectHyperlinks](https://reference.aspose.com/words/net/aspose.words.loading/txtloadoptions/detecthyperlinks/)-Eigenschaft implementiert.

### Andere

* Die Metadatei-Rendering-Emulation zur Bestimmung der Rastergröße wurde speziell für WMF Stiftbreite und EMF kosmetische Stiftbreite implementiert. Um dies zu erreichen, wurde die Eigenschaft **ScaleWmfFontsToMetafileSize** durch die Eigenschaft [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpage/) ersetzt und die Eigenschaft [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/net/aspose.words.saving/metafilerenderingoptions/emulaterenderingtosizeonpageresolution/) hinzugefügt. <sup>23.9</sup>
* Mit der [InsertDocumentInline](https://reference.aspose.com/words/net/aspose.words/documentbuilder/insertdocumentinline/) -Methode wurde eine vereinfachte Methode zum Einfügen eines Dokuments in ein anderes Dokument an der aktuellen Cursorposition eingeführt. <sup>23.10</sup>
* Die Möglichkeit, auf Stileigenschaften zuzugreifen und diese zu ändern, wurde durch die Einführung der neuen Eigenschaft [Locked](https://reference.aspose.com/words/net/aspose.words/style/locked/) hinzugefügt. <sup>23.10</sup>
* Den Methoden der Klasse [CompositeNode](https://reference.aspose.com/words/net/aspose.words/compositenode/) wurde ein generischer Typparameter hinzugefügt. <sup>23.10</sup>
* Mit den Methoden [Accept](https://reference.aspose.com/words/net/aspose.words/revisioncollection/accept/) und [Reject](https://reference.aspose.com/words/net/aspose.words/revisioncollection/reject/) wurde eine Möglichkeit implementiert, zu steuern, wann eine bestimmte Revision akzeptiert / abgelehnt werden soll oder nicht. Diese Erweiterung gibt den Benutzern eine genauere Kontrolle über den Revisionsprozess. <sup>23.11</sup>
* Die Möglichkeit, alle Abschnitte eines Dokuments auf dasselbe XLSX-Arbeitsblatt zu schreiben, wurde durch den neuen [XlsxSectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsectionmode/)-Aufzählungstyp und die neue [SectionMode](https://reference.aspose.com/words/net/aspose.words.saving/xlsxsaveoptions/sectionmode/)-Eigenschaft bereitgestellt. <sup>23.11</sup>
* Eine Möglichkeit zu steuern, wie ZIP64-Formaterweiterungen für OOXML-Dokumente verwendet werden, wurde durch die neue Zip64Mode-Eigenschaft der `OoxmlSaveOptions`-Klasse und die neue Zip64Mode-Aufzählung implementiert. <sup>23.12</sup>
* Unterstützung für WebP-Bilder wurde eingeführt. Bitte beachten Sie, dass diese Funktion nur für verfügbar ist.NetStandart und .NET6+ Versionen. <sup>23.12</sup>

{{% alert color="primary" %}}

Erfahren Sie mehr über [Aspose.Words für .NET 23.9 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-9-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 23.10 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-10-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 23.11 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-11-release-notes/).

Erfahren Sie mehr über [Aspose.Words für .NET 23.12 Versionshinweise](https://releases.aspose.com/words/net/release-notes/2023/aspose-words-for-net-23-12-release-notes/).

{{% /alert %}}

## Siehe auch

{{% alert color="primary" %}}

Diese Seite enthält die neuesten Release-Nachrichten der letzten 2 Jahre. Einzelheiten zu früheren Versionen finden Sie in der [Versionshinweise'](https://releases.aspose.com/words/net/release-notes/) seiten in den entsprechenden Abschnitten.

{{% /alert %}}
