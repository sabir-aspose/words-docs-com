---
title: מה חדש
second_title: Aspose.Words עבור C++
articleTitle: מה חדש ב Aspose.Words עבור C++
linktitle: מה חדש ב Aspose.Words עבור C++
type: docs
description: "Aspose.Words עבור C++ מתרחב ומשפר מדי יום. בדף זה תוכלו ללמוד על התכונות הענקיות והמעניינות ביותר של המוצר."
weight: 2
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /he/cpp/what-s-new-in-aspose-words-for-cpp/
timestamp: 2025-04-15-08-02-05
---

דף זה מתאר את התכונות החדשות המעניינות ביותר Aspose.Words שהוצגו במהדורות האחרונות.

## Aspose.Words עבור C++ 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 מציג AI - בדיקת דקדוק מופעלת ומשפר את שמירת המסמכים עם אפשרויות מתקדמות לפורמטים HTML, SVG ו Markdown.

Aspose.Words 25.2 מציג סיכום טקסט עם Anthropic AI מודלים, מוסיף MsWorks תמיכה בפורמט, משפר את השליטה הטיפוגרפית ומשפר PDF מבנה וטיפול ברשימה.

Aspose.Words 25.3 משפר בודק דקדוק מופעל AI ובחירת גופנים עם המאפיין UpdateAmbiguousTextFont, כמו גם משפר PDF ייצוא קבצים מצורפים.

Aspose.Words 25.4 מציג תמיכה בגדלי נייר חדשים, מאפשר בקרת ייצוא מתקדמת HTML, משפר את הטיפול בסימני מים ומשפר את השימושיות של LowCode API.

### AI - מופעל תכונות

#### מסמך AI בדיקת דקדוק

* היכולת לבדוק את הדקדוק של המסמך שסופק באמצעות מודלים גנראטיביים OpenAI הוצגה על ידי הוספת שיטה חדשה [CheckGrammar](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/checkgrammar/). <sup>25.1</sup>
* תכונת בדיקת הדקדוק המופעלת AI עודכנה כדי לתמוך בכל הדגמים הזמינים בספירה [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/). <sup>25.3</sup>

#### סיכום באמצעות מודלים של שפה גנראטיבית Anthropic <sup>25.2</sup>

סיכום טקסט באמצעות מודלים של שפה גנראטיבית Anthropic הופעל על ידי הצגת כיתה ציבורית חדשה [AnthropicAiModel](https://reference.aspose.com/words/cpp/aspose.words.ai/).

### Low Code

#### Low Code API שימושיות <sup>25.4</sup>

שיפורים משמעותיים בשימוש של **LowCode API** הוצגו, הפשטו את עיבוד המסמכים והפחיתו את הצורך בקוד חוזר.

### פורמטים נתמכים <sup>25.2</sup>

החל מהגרסה 25.2, נוספה תאימות לפורמט הטעינה החדש MsWorks עבור מסמכי עבודות Microsoft.

### המרה, טעינה ושמירה של מסמכים

#### חיסכון משופר ל HTML ו SVG פורמטים <sup>25.1</sup>

שמירה ל HTML ו SVG פורמטים שופרו על ידי הוספת **IdPrefix** ו **RemoveJavaScriptFromLinks** מאפיינים לשני המחלקות [HtmlFixedSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlfixedsaveoptions/) ו [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/).

#### הגדר רזולוציית תמונה ו OfficeMath מצב פלט בעת שמירה ל Markdown <sup>25.1</sup>

- אפשרות [ImageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imageresolution/) חדשה נוספה לכיתה [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) כדי להגדיר את רזולוציית התמונה.
- אפשרות [OfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_officemathexportmode/) חדשה ו [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownofficemathexportmode/) ספירה נוספה ונוספה לכיתה [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) כדי להגדיר OfficeMath מצב פלט.
- היכולת להגדיר סימן מים של תמונה מהזרם הוצגה על ידי הוספת עומס יתר חדש לשיטה [SetImage](https://reference.aspose.com/words/cpp/aspose.words/watermark/setimage/#watermarksetimageconst-systemsharedptrsystemiostream-const-systemsharedptrasposewordsimagewatermarkoptions-method). <sup>25.4</sup>

### עיבוד

#### שליטה טיפוגרפית משופרת <sup>25.2</sup>

המאפיין [NumberSpacing](https://reference.aspose.com/words/cpp/aspose.words/font/get_numberspacing/) נוסף לשליטה טיפוגרפית משופרת.

#### בחירת גופן שליטה עבור תווים מעורפלים <sup>25.3</sup>

נכס ציבורי חדש [UpdateAmbiguousTextFont](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/get_updateambiguoustextfont/) נוסף לכיתה [SaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/saveoptions/) כדי לשלוט בבחירת הגופן בהתאם לקוד התווים בו נעשה שימוש.

#### אפשרויות גודל נייר <sup>25.4</sup>

היכולת להשתמש בגדלי נייר JIS B4 ו JIS B5 הוצגה על ידי הוספת ערכים חדשים לספירה [PaperSize](https://reference.aspose.com/words/cpp/aspose.words/papersize/).

#### HTML פלט שליטה <sup>25.4</sup>

היכולת להסיר JavaScript מההיפר-קישור URLs במהלך HTML ייצוא הוצגה על ידי הוספת המאפיין [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/cpp/aspose.words.saving/htmlsaveoptions/get_removejavascriptfromlinks/).

### אחרים

* PDF המבנה הלוגי שופר עם תמיכה בשדות TOA, BIBLIOGRAPHY ו INDEX. <sup>25.2</sup>
* שיטת [AddSingleLevelList](https://reference.aspose.com/words/cpp/aspose.words.lists/listcollection/addsinglelevellist/) הוצגה לטיפול ברשימה משופרת. <sup>25.2</sup>
* נכס חדש [AttachmentsEmbeddingMode](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/get_attachmentsembeddingmode/) נוסף כדי להחליף **EmbedAttachments** כדי לשפר את הייצוא של הקבצים המצורפים PDF. כמו כן, ערכים חדשים נוספו לספירה [PdfCompliance](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfcompliance/) כדי לתמוך בקבצים מצורפים של גירסאות PDF/A. בנוסף, קבצים מצורפים נתמכים כעת בהצפנה. <sup>25.3</sup>

{{% alert color="primary" %}}

למידע נוסף על [Aspose.Words עבור C++ 25.1 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-1-release-notes/).

למידע נוסף על [Aspose.Words עבור C++ 25.2 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-2-release-notes/).

למידע נוסף על [Aspose.Words עבור C++ 25.3 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-3-release-notes/).

למידע נוסף על [Aspose.Words עבור C++ 25.4 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2025/aspose-words-for-cpp-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words עבור C++ 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 מציג group shape הכנסה ו StructuredDocumentTag הכנסה באמצעות DocumentBuilder, משפר את עיבוד התרשים הרדיאלי עם סיום הלימודים, משפר חתימות דיגיטליות עם XAdES-EPES תמיכה, מוסיף Markdown זיהוי קו תחתון ומספק גישה למפרידי הערת שוליים/הערת סיום.

Aspose.Words 24.10 מציג תמיכה משופרת ActiveX עם CommandButton יצירה, בקרת נראות צורה חדשה, יכולת group shapes, שיפור Markdown ייצוא לטבלאות, עיצוב תרשים עבור Pie ו Doughnut תרשימים, טיפול טוב יותר בקידוד ביג 5 ותמיכה בגופנים טייוואניים מיושנים.

Aspose.Words 24.11 מציג AI - סיכום מסמכים מופעל, אפשרויות עיבוד משופרות, גישה משופרת למאפייני מסמך ו ActiveX כיתוב בקרה.

Aspose.Words 24.12 מציג מיקום תווית נתונים הניתן להתאמה אישית, תרגום טקסט מופעל על ידי גוגל AI, אפשרויות ניקוי משופרות Mail Merge ושיעורי עיבוד חדשים LowCode.

### AI - מופעל תכונות

#### סיכום מסמכים באמצעות OpenAI וגוגל <sup>24.11</sup>

תמיכה בסיכום מסמכים באמצעות מודלים של שפות גנרטיביות **OpenAI** ו - **Google** הושלבה.

#### תרגום טקסט באמצעות מודלים של שפה גנראטיבית של גוגל <sup>24.12</sup>

היכולת לתרגם טקסט באמצעות מודלים של שפות גנראטיביות של גוגל הושמשה ב - Aspose.Words על ידי הוספת שיטת [Translate](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/translate/) והספירה [Language](https://reference.aspose.com/words/cpp/aspose.words.ai/language/) למרחב השמות [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/).

### Low Code <sup>24.12</sup>

חָדָשׁ LowCode שיעורים כמו [Comparer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/cpp/aspose.words.lowcode/merger/), [Replacer](https://reference.aspose.com/words/cpp/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/cpp/aspose.words.lowcode/splitter/) וכו'. הוצג, מציע סדרה של שיטות שמציגות את האיזון המושלם בין פשטות וגמישות לעיבוד מסמכים.

### עיבוד והדפסה

#### סיום לימודים בתרשימים רדיאליים <sup>24.9</sup>

עיבוד של סיום הלימודים על תרשימים רדיאליים יושם.

#### CommandButton ActiveX פקדים <sup>24.10</sup>

היכולת ליצור בקרות CommandButton ActiveX הוצגה על ידי הוספת שיטה ציבורית חדשה [InsertForms2OleControl](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertforms2olecontrol/) וכיתה ציבורית חדשה **Forms2OleControl**.

#### בקרת צורת נראות <sup>24.10</sup>

נכס ציבורי חדש [Hidden](https://reference.aspose.com/words/cpp/aspose.words.drawing/shapebase/get_hidden/) נוסף כדי לשלוט בנראות הצורות.

#### שינויים בתרשימים Pie ו Doughnut <sup>24.10</sup>

מספר נכסים ציבוריים חדשים נוספו לפורמט Pie ו Doughnut תרשימים.

#### שלוט בעיבוד של PDF גבולות שדה טופס בחירה <sup>24.11</sup>

אפשרות חדשה לשליטה בעיבוד של PDF גבולות שדה טופס בחירה יושמה על ידי הוספת אפשרות ציבורית חדשה **RenderChoiceFormFieldBorder**.

#### קבל והגדר קודי פורמט לנתוני תרשים <sup>24.11</sup>

היכולת לקבל ולהגדיר קודי פורמט לנתוני תרשים נוספה על ידי יישום המאפיין **FormatCode** בכיתות [ChartXValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartyvaluecollection/) ו - [BubbleSizeCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/bubblesizecollection/).

#### עיבוד תרשימי היסטוגרמה עם פחים ותוויות <sup>24.11</sup>

עיבוד תרשים היסטוגרמה שופר על ידי מתן אפשרות למספר מוגדר של פחים ותוויות.

#### התאם אישית את מיקום תוויות הנתונים <sup>24.12</sup>

היכולת להתאים אישית את מיקום תוויות הנתונים נוספה על ידי הצגת מאפיינים חדשים לכיתות [ChartDataLabel](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabel/) ו - [ChartDataLabelCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatalabelcollection/).

### המרה, טעינה ושמירה של מסמכים

#### קו תחתון עיצוב בעת טעינת Markdown קבצים <sup>24.9</sup>

האפשרות לזהות עיצוב קו תחתון בעת טעינת מסמכים Markdown שולבה על ידי הוספת נכס ציבורי חדש **ImportUnderlineFormatting**.

#### ייצוא טבלאות כ HTML בעת שמירה ל Markdown <sup>24.10</sup>

אפשרות לייצא טבלאות כ HTML בעת שמירת מסמכים בפורמט Markdown יושמה על ידי הוספת נכס ציבורי חדש [ExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_exportashtml/) וספירה [MarkdownExportAsHtml](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownexportashtml/).

#### ייצוא PDF עם מבנה לוגי מעודכן <sup>24.11</sup>

PDF הייצוא שופר על ידי הכללת מאפייני כותרת הטבלה כ PDF כותרות אלמנטים של מבנה לוגי.

### Mail Merge ודיווח

#### הסר טבלאות ריקות במהלך Mail Merge <sup>24.12</sup>

אפשרות **RemoveEmptyTables** חדשה נוספה לספירה [MailMergeCleanupOptions](https://reference.aspose.com/words/cpp/aspose.words.mailmerging/mailmergecleanupoptions/) כדי לחדד את הפלט Mail Merge.

### חתימות דיגיטליות

#### חתום על מסמכים עם XAdES-EPES <sup>24.9</sup>

היכולת לחתום על מסמכים עם חתימות XAdES-EPES רמה XML-DSig הוצגה על ידי הוספת נכס ציבורי חדש **XmlDsigLevel** ומספר ציבורי חדש **XmlDsigLevel**.

### אחרים

* שיטה ציבורית חדשה [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/) נוספה ל group shapes. <sup>24.9</sup>
* נוספה שיטה ציבורית חדשה [InsertStructuredDocumentTag](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertstructureddocumenttag/) כדי להוסיף **StructuredDocumentTags** למסמך. <sup>24.9</sup>
* גישה ציבורית למפרידי הערות שוליים / הערות קצה ניתנה על ידי הוספת כמה כיתות ציבוריות ונכסים. <sup>24.9</sup>
* היכולת לקבץ צורות בודדות, group shapes יחד, ולקבץ ישירות את שתי הצורות ו group shapes הוצגה על ידי הוספת שיטת [InsertGroupShape](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertgroupshape/). <sup>24.10</sup>
* טיפול בקידוד ביג 5 עבור TrueType טבלאות המפה שופר. <sup>24.10</sup>
* התמיכה בגופנים טייוואניים מיושנים שופרה. <sup>24.10</sup>
* כדי לגשת למאפייני מסמך מורחבים, נוספו מאפיינים לקריאה בלבד לכיתה **BuiltInDocumentProperties**. <sup>24.11</sup>
* הגדרת כיתובים עבור בקרות ActiveX הופעלה על ידי הוספת מגדיר ציבורי חדש למאפיין **Forms2OleControl.Caption**. <sup>24.11</sup>

{{% alert color="primary" %}}

למידע נוסף על [Aspose.Words עבור C++ 24.9 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-9-release-notes/).

למידע נוסף על [Aspose.Words עבור C++ 24.10 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-10-release-notes/).

למידע נוסף על [Aspose.Words עבור C++ 24.11 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-11-release-notes/).

למידע נוסף על [Aspose.Words עבור C++ 24.12 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words עבור C++ 24.5, 24.6, 24.7

Aspose.Words 24.5 מרחיב אפשרויות למכלולים, משפר את יכולות העיבוד ומרחיב כמה אפשרויות אחרות.

Aspose.Words 24.6 משפר את אפשרויות העיבוד, משפר את פונקציונליות החיפוש וההשוואה ומרחיב מספר תכונות אחרות.

Aspose.Words 24.7 משנה את אופן העבודה שלך עם ActiveX, מרחיב את יכולות העיבוד, כמו גם ייצוא לפורמטים Markdown ו - XLSX.

### פורמטים נתמכים

החל מהגרסה 24.7, ייצוא ל PDF/UA-2 נתמך כדי להבטיח נגישות למשתמשים עם מוגבלויות.

### עיבוד והדפסה

#### שינויים בתרשימים, צורות ו DrawingML <sup>24.5</sup>

- DrawingML עיבוד אפקטים עבור SVG גרפיקה, הרחבת הפונקציונליות הקודמת מוגבלת לתמונות, יושמה.
- תמיכה ביצירת תרשימי קומבו והתאמת מאפיינים כגון רוחב פער, חפיפה וסולם בועות בתוך קבוצות סדרות הוצגה על ידי הוספת הכיתות **ChartSeriesGroup** ו - **ChartSeriesGroupCollection** והמאפיין **SeriesGroups**.
- פונקציונליות לתפעל את אפקט SoftEdge של צורות יושמה על ידי הוספת הכיתה **SoftEdgeFormat**.
- היכולת לשנות את התאמת ערכי הצורות יושמה על ידי הוספת ה - **AdjustmentCollection** ו **Adjustment** כיתות ציבוריות ו **Adjustments** נכס.

#### שינויים בתרשימים, צורות וציור <sup>24.6</sup>

- יכולות התרשימים שופרו. כעת תוכל ליצור מגוון רחב יותר של תרשימים, כולל *Treemaps*, *Sunbursts*, *Histograms*, *Pareto* תרשימים, *Box & Whisker* תרשימים, *Waterfalls*, ו *Funnels*. זה מאפשר לך לדמיין את הנתונים שלך בצורה מגוונת ואינפורמטיבית יותר.
- בקרת צבע עבור עיצוב צל שופרה. אתה יכול להשיג שליטה מדויקת יותר על מראה המסמכים שלך על ידי גישה לצבעי צל.
- שיפור ביצועים עבור עיבוד רקע שופר. אתה יכול להאיץ משמעותית את עיבוד הרקעים המכילים אלמנטים קטנים הודות לטכנולוגיית ריצוף מקורית.
- נוספו שיפועים מציאותיים לצורות. כעת ניתן ליצור DML צורות עם שיפועים לא לינאריים, תוך חיקוי הסגנון הוויזואלי של Microsoft Word למראה מלוטש יותר.

#### תרשים נתונים תווית התאמה אישית <sup>24.7</sup>

נוספה היכולת להתאים אישית תוויות נתוני תרשים כגון **Orientation** ו **Rotation**.

#### עיצוב מספר מותאם אישית לרמות רשימה <sup>24.7</sup>

הוסף סטר לרכוש הציבורי [CustomNumberStyleFormat](https://reference.aspose.com/words/cpp/aspose.words.lists/listlevel/get_customnumberstyleformat/). עכשיו אתה יכול להגדיר סגנון מספר מותאם אישית עבור רמות רשימה.

#### שינויים בעבודה עם ActiveX <sup>24.7</sup>

- כעת ניתן לשנות את המאפיינים של ActiveX אובייקטים, מה שנותן לך שליטה רבה יותר על התנהגותם.
- היכולת לשנות את הערך של לחצן הבחירה ActiveX שליטה כדי לאפשר אינטראקציה דינמית נוספה.
- נוספה היכולת להחליף ActiveX checkbox ל "מסומן" או "לא מסומן".

### טעינה ושמירה של מסמכים

#### ייצוא קישורים לפורמט Markdown <sup>24.7</sup>

היכולת לשלוט בייצוא קישורים בפורמט Markdown נוספה באמצעות יישום המאפיין [LinkExportMode](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_linkexportmode/).

### חיפוש והשוואה

#### אפשרויות השוואה מתקדמות <sup>24.6</sup>

נוספה היכולת לייעל זרימות עבודה לניתוח נתונים עם פונקציונליות השוואה משופרת. זה כולל אפשרות **IgnoreStoreItemId** חדשה וממשק מעוצב מחדש להשוואות מתקדמות.

### אחרים

- הפונקציה לחיסול דפים ריקים ממסמך יושמה על ידי הוספת שיטת [RemoveBlankPages](https://reference.aspose.com/words/cpp/aspose.words/document/removeblankpages/). <sup>24.5</sup>
- היכולת לבדוק את נוכחותם של VBA פקודות מאקרו מבלי לטעון מסמך סופקה על ידי הוספת המאפיין **HasMacros**. <sup>24.5</sup>
- נכס חדש **DateTimeUtc** נוסף - זה מספק חותמת זמן מדויקת יותר להערות, שיפור הארגון ועקיבות. <sup>24.6</sup>
- פורמט זמן התאריך מזוהה כעת באופן אוטומטי לייצוא חלק לפורמט XLSX. <sup>24.7</sup>
- הנכס הציבורי [IsProtected](https://reference.aspose.com/words/cpp/aspose.words.vba/vbaproject/get_isprotected/), המאפשר לך לוודא אם פרויקט VBA מוגן, נוסף. <sup>24.7</sup>

{{% alert color="primary" %}}

למידע נוסף על [Aspose.Words עבור C++ 24.5 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-5-release-notes/).

למידע נוסף על [Aspose.Words עבור C++ 24.6 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-6-release-notes/).

למידע נוסף על [Aspose.Words עבור C++ 24.7 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-7-release-notes/).

{{% /alert %}}

## Aspose.Words עבור C++ 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 משפר את החוויה סביב ניהול צבעי שבץ, משפר OLE אובייקטים, כמו גם מציג ציבור מקורות ביבליוגרפיה חדש API.

Aspose.Words 24.2 תרשימים מורחבים API וניהול סגנון. גרסה זו של Aspose.Words הציגה גם את היכולת לציין SvgSaveOptions במהלך העיבוד, טעינת בקרה גמישה יותר Markdown קבצים ועבודה עם טקסט הפניה להערות שוליים והערות סיום.

Aspose.Words 24.3 מציג אמולציה של פעולות רסטר בינאריות עבור WMF מטא-קבצים וגם ממשיך להרחיב את התרשימים API.

Aspose.Words 24.4 משפר כמה אפשרויות עיבוד, כמו גם משפר את העבודה עם חתימות דיגיטליות.

### עיבוד והדפסה

#### בקרת צבע שבץ <sup>24.1</sup>

הכיתה [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) הורחבה עם קבוצה של נכסים ציבוריים חדשים הקשורים לניהול צבעי קו: [ForeThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_forethemecolor/) ו [BackThemeColor](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backthemecolor/), [ForeTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_foretintandshade/) ו [BackTintAndShade](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/get_backtintandshade/).

#### DrawingML תרשימים API הרחבה <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** ממשיך להתרחב.

#### הטמע גופנים שהוכרזו ב @font-face כללים <sup>24.4</sup>

הוספת יכולת להטמיע גופנים שהוכרזו ב @font-face כללים בהגדרות הגופן של המסמך שהתקבל הוצגה על ידי הוספת מאפיין [SupportFontFaceRules](https://reference.aspose.com/words/cpp/aspose.words.loading/htmlloadoptions/get_supportfontfacerules/) חדש.

#### עבודה עם עיצוב זוהר והשתקפות <sup>24.4</sup>

היכולת לעבוד עם עיצוב זוהר והשתקפות עבור אובייקט ציור יושמה.

### טעינה ושמירה של מסמכים

#### ציין SvgSaveOptions במהלך העיבוד <sup>24.2</sup>

היכולת לציין [SvgSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/svgsaveoptions/) במהלך העיבוד נוספה באמצעות [ShapeRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/shaperenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) ו [OfficeMathRenderer](https://reference.aspose.com/words/cpp/aspose.words.rendering/officemathrenderer/).[Save](https://reference.aspose.com/words/cpp/aspose.words.rendering/noderendererbase/save/) שיטות.

#### שמור שורות ריקות בעת טעינת Markdown קבצים <sup>24.2</sup>

נוספה היכולת לשמר שורות ריקות בעת טעינת Markdown קבצים.

### אחרים

- היכולת לשנות את הטקסט של פקד `TextBox` OLE הוצגה על ידי הוספת מאפיין **Text** חדש לכיתה **TextBoxControl** החדשה. <sup>24.1</sup>
- מקורות הביבליוגרפיה הציבוריים API יושמו באמצעות הוספת מרחב שמות חדש [Aspose.Words.Bibliography](https://reference.aspose.com/words/cpp/aspose.words.bibliography/) עם הכיתות והספירות החדשות שלו, ובאמצעות הוספת מאפיין [Bibliography](https://reference.aspose.com/words/cpp/aspose.words/document/get_bibliography/) חדש לכיתה [Document](https://reference.aspose.com/words/cpp/aspose.words/document/). <sup>24.1</sup>
- נכסים ציבוריים חדשים [Priority](https://reference.aspose.com/words/cpp/aspose.words/style/get_priority/), [UnhideWhenUsed](https://reference.aspose.com/words/cpp/aspose.words/style/get_unhidewhenused/) ו [SemiHidden](https://reference.aspose.com/words/cpp/aspose.words/style/get_semihidden/) לניהול סגנון משופר נוספו לכיתה [Style](https://reference.aspose.com/words/cpp/aspose.words/style/). <sup>24.2</sup>
- הפונקציונליות לאחזור טקסט סימן הייחוס בפועל להערות שוליים והערות סיום שופרה באמצעות המאפיין [ActualReferenceMark](https://reference.aspose.com/words/cpp/aspose.words.notes/footnote/get_actualreferencemark/) ושיטת [UpdateActualReferenceMarks](https://reference.aspose.com/words/cpp/aspose.words/document/updateactualreferencemarks/). <sup>24.2</sup>
- חיקוי של פעולות רסטר בינארי עבור WMF מטא-קבצים הושק. <sup>24.3</sup>
- היכולת להגדיר אפשרויות חתימה למסמכים בתוך **SaveOptions** הופעלה על ידי הוספת כיתה חדשה **DigitalSignatureDetails** עם חברים ציבוריים חדשים, כמו גם הוספת מאפיינים חדשים לכיתות [OoxmlSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/ooxmlsaveoptions/), [DocSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/docsaveoptions/) ו - [OdtSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/odtsaveoptions/). <sup>24.4</sup>

{{% alert color="primary" %}}

למידע נוסף על [Aspose.Words עבור C++ 24.1 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-1-release-notes/).

למידע נוסף על [Aspose.Words עבור C++ 24.2 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-2-release-notes/).

למידע נוסף על [Aspose.Words עבור C++ 24.3 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-3-release-notes/).

למידע נוסף על [Aspose.Words עבור C++ 24.4 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2024/aspose-words-for-cpp-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words עבור C++ 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 מרחיב את אפשרויות העיבוד, הדמיית עיבוד מטאפיל ו markdown שמור אפשרויות.

Aspose.Words 23.10 משפר עיבוד, מרחיב אפשרויות לטעינה ושמירת מסמכים ומאפשר למשתמשים למזג מסמכים בדרכים חדשות.

Aspose.Words 23.11 משפר את העבודה עם תיקונים, XLSX פורמט וגופנים על מקרא תרשים עם אפשרויות נוספות.

Aspose.Words 23.12 מציג מאפיינים וספירות חדשים לעבודה עם PDF ו OOXML מסמכים, כמו גם תמיכה ב WebP תמונות.

### עיבוד והדפסה

#### התאמה אישית של כותרות צירים בתרשימים DrawingML <sup>23.9</sup>

היכולת להתאים אישית כותרות ציר בתרשימים DrawingML הוצגה על ידי יישום של מעמד ציבורי חדש **ChartAxisTitle** ו [Title](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartaxis/get_title/) נכס.

#### קביעת המיקום האנכי של גופנים בתוך פסקה <sup>23.9</sup>

כעת ניתן להגדיר את המיקום האנכי של הפונטים בתוך פסקה באמצעות המאפיין הציבורי החדש [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/paragraphformat/get_baselinealignment/) והספירה החדשה [BaselineAlignment](https://reference.aspose.com/words/cpp/aspose.words/baselinealignment/).

#### בקרת צבע בחזית <sup>23.10</sup>

היכולת לאחזר את צבע החזית ללא משנים נוספה לכיתות [Fill](https://reference.aspose.com/words/cpp/aspose.words.drawing/fill/) ו - [Stroke](https://reference.aspose.com/words/cpp/aspose.words.drawing/stroke/) באמצעות המאפיין **BaseForeColor**.

#### הרחבת הפונקציונליות של תרשימים <sup>23.10</sup>

הפונקציונליות של הכיתות [ChartDataPointCollection](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartdatapointcollection/), [ChartSeries](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartseries/) ו - [ChartFormat](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartformat/) הורחבה בשיטות ותכונות חדשות.

#### התאם באופן אוטומטי והתאם תמונה לצורה <sup>23.10</sup>

דרך פשוטה להתאים באופן אוטומטי ולהתאים תמונה בתוך צורה מסוימת ניתנה באמצעות השיטה החדשה [FitImageToShape](https://reference.aspose.com/words/cpp/aspose.words.drawing/imagedata/fitimagetoshape/).

#### עיצוב גופן ברירת מחדל עבור DrawingML ערכי אגדת תרשים <sup>23.11</sup>

היכולת לציין עיצוב גופן ברירת מחדל עבור ערכי מקרא של DrawingML תרשימים נוספה דרך המאפיין [Font](https://reference.aspose.com/words/cpp/aspose.words.drawing.charts/chartlegend/get_font/). תכונה זו מאפשרת מראה יעיל ועקבי יותר עבור רכיבי תרשים, ומשפרת את האסתטיקה הכוללת של המסמך.

#### ציין פריסת עמוד בעת פתיחה PDF בקורא <sup>23.12</sup>

היכולת לציין את פריסת העמוד שישמש בעת פתיחת מסמך בקורא PDF נוספה באמצעות הכנסת מאפיין **PageLayout** חדש לכיתה [PdfSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/pdfsaveoptions/) והכנסת ספירה **PdfPageLayout** חדשה.

### טעינה ושמירה של מסמכים

#### ציון שם תיקיה לבניית תמונה URIs ב Markdown <sup>23.9</sup>

הכיתה [MarkdownSaveOptions](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/) הורחבה על ידי הכללת המאפיין [ImagesFolderAlias](https://reference.aspose.com/words/cpp/aspose.words.saving/markdownsaveoptions/get_imagesfolderalias/), המאפשר לציין את שם התיקיה המשמשת לבניית תמונה URIs שנכתבה במסמך Markdown.

#### להפחית PDF פלט גודל <sup>23.10</sup>

אופטימיזציות עיבוד שונות של PDF כדי להפחית את גודל הפלט בעת השימוש בהגדרות [OptimizeOutput](https://reference.aspose.com/words/cpp/aspose.words.saving/fixedpagesaveoptions/get_optimizeoutput/) יושמו.

#### זיהוי היפר-קישורים בעת טעינה TXT מסמכים <sup>23.10</sup>

התכונה לזיהוי היפר-קישורים בעת טעינת TXT מסמכים יושמה על ידי הוספת מאפיין [DetectHyperlinks](https://reference.aspose.com/words/cpp/aspose.words.loading/txtloadoptions/get_detecthyperlinks/) חדש.

### אחרים

- הדמיית עיבוד מטאפיל לקביעת גודל הרסטריזציה יושמה, במיוחד עבור WMF רוחב עט ו EMF רוחב עט קוסמטי. כדי להשיג זאת, המאפיין **ScaleWmfFontsToMetafileSize** הוחלף במאפיין [EmulateRenderingToSizeOnPage](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpage/) והמאפיין [EmulateRenderingToSizeOnPageResolution](https://reference.aspose.com/words/cpp/aspose.words.saving/metafilerenderingoptions/get_emulaterenderingtosizeonpageresolution/) הוסף. <sup>23.9</sup>
* שיטה פשוטה להכנסת מסמך אחד למסמך אחר במיקום הסמן הנוכחי הוצגה בשיטת [InsertDocumentInline](https://reference.aspose.com/words/cpp/aspose.words/documentbuilder/insertdocumentinline/). <sup>23.10</sup>
* היכולת לגשת ולשנות מאפייני סגנון נוספה באמצעות הצגת המאפיין החדש [Locked](https://reference.aspose.com/words/cpp/aspose.words/style/get_locked/). <sup>23.10</sup>
* פרמטר סוג כללי נוסף לשיטות של הכיתה [CompositeNode](https://reference.aspose.com/words/cpp/aspose.words/compositenode/). <sup>23.10</sup>
* דרך לשלוט מתי יש לקבל/לדחות תיקון מסוים או לא יושמה באמצעות [Accept](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/accept/) ו [Reject](https://reference.aspose.com/words/cpp/aspose.words/revisioncollection/reject/) שיטות. שיפור זה מעניק למשתמשים שליטה עדינה יותר על תהליך העדכון. <sup>23.11</sup>
* היכולת לכתוב את כל חלקי המסמך על אותו גליון עבודה XLSX ניתנה באמצעות סוג הספירה החדש [XlsxSectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsectionmode/) והמאפיין החדש [SectionMode](https://reference.aspose.com/words/cpp/aspose.words.saving/xlsxsaveoptions/get_sectionmode/). <sup>23.11</sup>
* דרך לשלוט כיצד ישמשו הרחבות פורמט ZIP64 למסמכים OOXML יושמה באמצעות המאפיין החדש של זיפ 64 מצב של הכיתה `OoxmlSaveOptions` והספירה החדשה של זיפ 64 מצב. <sup>23.12</sup>
* תמיכה בתמונת WebP הוצגה. שים לב שתכונה זו זמינה רק עבור .NetStandart ו .NET6 + גרסאות. <sup>23.12</sup>

{{% alert color="primary" %}}

למידע נוסף על [Aspose.Words עבור C++ 23.9 הערות שחרור](/words/cpp/aspose-words-for-cpp-23-9-release-notes/).
למידע נוסף על [Aspose.Words עבור C++ 23.10 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-10-release-notes/).
למידע נוסף על [Aspose.Words עבור C++ 23.11 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-11-release-notes/).
למידע נוסף על [Aspose.Words עבור C++ 23.12 הערות שחרור](https://releases.aspose.com/words/cpp/release-notes/2023/aspose-words-for-cpp-23-12-release-notes/).

{{% /alert %}}

## ראה גם

{{% alert color="primary" %}}

דף זה מכיל את חדשות המהדורה האחרונות עבור 2 השנים האחרונות. לפרטים על שחרורים קודמים, ראה [הערות שחרור'](/words/cpp/release-notes/) דפים בסעיפים הרלוונטיים.

{{% /alert %}}
