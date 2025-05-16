---
title: چه خبر ؟
second_title: Aspose.Words برای Python via .NET
articleTitle: چه چیز جدیدی در Aspose.Words برای Python via .NET
linktitle: چه چیز جدیدی در Aspose.Words برای Python via .NET
type: docs
description: "Aspose.Words برای Python via .NET روزانه گسترش می یابد و افزایش می یابد. در این صفحه می توانید با بزرگ ترین و جالب ترین ویژگی های این محصول آشنا شوید."
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /fa/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-04-16-07-02-05
---

این صفحه جالب ترین ویژگی های جدید Aspose.Words را که در نسخه های اخیر معرفی شده است، توصیف می کند.

## Aspose.Words برای Python از طریق .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words 25.1 بررسی گرامر با قدرت AI را معرفی می کند و صرفه جویی در اسناد را با گزینه های پیشرفته برای فرمت های HTML، SVG و Markdown افزایش می دهد.

Aspose.Words 25.2 خلاصه متن را با مدل های Anthropic AI معرفی می کند، پشتیبانی از فرمت MsWorks را اضافه می کند، کنترل تایپوگرافی را افزایش می دهد و ساختار و مدیریت لیست PDF را بهبود می بخشد.

Aspose.Words 25.3 با استفاده از ویژگی UpdateAmbiguousTextFont، بررسی‌کننده گرامر و انتخاب فونت مبتنی بر AI را بهبود می‌بخشد و همچنین خروجی پیوست‌های PDF را بهبود می‌بخشد.

Aspose.Words 25.4 پشتیبانی از اندازه های جدید کاغذ را معرفی می کند، کنترل صادرات پیشرفته HTML را امکان پذیر می کند و کنترل علامت آبی را بهبود می بخشد.

### AI-ویژگی های قدرت

#### سند AI بررسی گرامر

* امکان بررسی دستور زبان سند ارائه شده با استفاده از مدل های تولید کننده OpenAI با اضافه کردن یک روش جدید [check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/) معرفی شده است. <sup>25.1</sup>
* ویژگی بررسی گرامر با قدرت AI به روز شده است تا از تمام مدل های موجود در شمارش [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/) پشتیبانی کند. <sup>25.3</sup>

#### خلاصه سازی با استفاده از مدل های زبان مولد Anthropic <sup>25.2</sup>

خلاصه متن با استفاده از مدل های زبان مولد Anthropic با معرفی یک کلاس عمومی جدید [AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/) فعال شده است.

### فرمت های پشتیبانی شده <sup>25.2</sup>

با شروع از نسخه 25.2، سازگاری با فرمت بارگذاری جدید MsWorks برای Microsoft اسناد کار اضافه شده است.

### تبدیل، بارگیری و ذخیره اسناد

#### بهبود پس انداز به فرمت های HTML و SVG <sup>25.1</sup>

پس انداز به فرمت های HTML و SVG با اضافه کردن ویژگی های **id_prefix** و **remove_java_script_from_links** به هر دو کلاس [HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/) و [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) افزایش یافته است.

#### تنظیم وضوح تصویر و OfficeMath حالت خروجی هنگام ذخیره به Markdown <sup>25.1</sup>

* یک گزینه جدید [image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/) به کلاس [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) اضافه شده است تا وضوح تصویر را تنظیم کند.
* یک گزینه جدید [office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/) و [MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/) شمارش شده و به کلاس [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) اضافه شده است تا حالت خروجی OfficeMath را تنظیم کند.

### رندر کردن

#### بهبود کنترل تایپوگرافی <sup>25.2</sup>

ویژگی [number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/) برای کنترل تایپوگرافی بهبود یافته اضافه شده است.

#### کنترل انتخاب فونت برای کاراکترهای مبهم <sup>25.3</sup>

یک ملک عمومی جدید [update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/) به کلاس [SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/) اضافه شده است تا انتخاب فونت را با توجه به کد کاراکتر مورد استفاده کنترل کند.

#### گزینه های اندازه کاغذ <sup>25.4</sup>

قابلیت استفاده از اندازه های کاغذی JIS B4 و JIS B5 با اضافه کردن مقادیر جدید به شمارش [PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/) معرفی شده است.

#### HTML کنترل خروجی <sup>25.4</sup>

امکان حذف JavaScript از hyperlink URLs در طول HTML export با اضافه کردن ویژگی [RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/) معرفی شده است.

### سایر

* ساختار منطقی PDF با پشتیبانی از فیلدهای TOA، BIBLIOGRAPHY و INDEX بهبود یافته است. <sup>25.2</sup>
* روش [add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate) برای بهبود مدیریت لیست معرفی شده است. <sup>25.2</sup>
* یک ویژگی جدید [attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/) برای جایگزینی **EmbedAttachments** برای بهبود صادرات PDF پیوست ها اضافه شده است. همچنین، مقادیر جدیدی به شمارش [PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/) اضافه شده است تا از پیوست های نسخه PDF/A پشتیبانی کند. علاوه بر این، پیوست ها اکنون با رمزگذاری پشتیبانی می شوند. <sup>25.3</sup>
* قابلیت تنظیم یک علامت آبی تصویر از یک جریان با اضافه کردن یک اضافه بار جدید به روش [SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions) معرفی شده است. <sup>25.4</sup>

{{% alert color="primary" %}}

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 25.1 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 25.2 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 25.3 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 25.4 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words برای Python از طریق .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words 24.9 درج group shape و درج StructuredDocumentTag را از طریق DocumentBuilder معرفی می کند، رندر نمودار شعاعی را با فارغ التحصیلی افزایش می دهد، امضاهای دیجیتال را با پشتیبانی XAdES-EPES بهبود می بخشد، تشخیص زیرنویس Markdown را اضافه می کند و دسترسی به جداکننده های حاشیه/حاشیه را فراهم می کند.

Aspose.Words 24.10 پشتیبانی از کنترل پیشرفته ActiveX را با CommandButton ایجاد، کنترل دید شکل جدید، توانایی group shapes، صادرات بهبود یافته Markdown برای جداول، قالب بندی نمودار برای Pie و Doughnut نمودارها، مدیریت بهتر کدگذاری Big5 و پشتیبانی از فونت های قدیمی تایوانی معرفی می کند.

Aspose.Words 24.11 خلاصه سازی سند با قدرت AI، گزینه های رندر پیشرفته، دسترسی بهتر به ویژگی های سند و ActiveX زیرنویس کنترل را معرفی می کند.

Aspose.Words 24.12 قرار دادن برچسب داده های قابل تنظیم، ترجمه متن Google AI و کلاس های پردازش جدید LowCode را بهبود می بخشد.

### AI-ویژگی های قدرت

#### خلاصه سازی اسناد با استفاده از OpenAI و گوگل <sup>24.11</sup>

پشتیبانی از خلاصه سازی اسناد با استفاده از مدل های زبان مولد **OpenAI** و **Google** با اضافه کردن فضای نام [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) با اعضای عمومی آن ادغام شده است.

#### ترجمه متون با استفاده از مدل های زبان مولد گوگل <sup>24.12</sup>

امکان ترجمه متن با استفاده از مدل های زبان مولد گوگل در Aspose.Words با اضافه کردن روش [translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/) و شمارش [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/) به فضای نام [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) اجرا شده است.

### Low Code <sup>24.12</sup>

کلاس های جدید LowCode مانند [Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) و غیره معرفی شده است، ارائه مجموعه ای از روش هایی که تعادل کامل بین سادگی و انعطاف پذیری برای پردازش اسناد را ایجاد می کند.

### رندر و چاپ

#### فارغ التحصیلی در نمودارهای شعاعی <sup>24.9</sup>

ارائه فارغ التحصیلی در نمودارهای شعاعی اجرا شده است.

#### CommandButton ActiveX کنترل <sup>24.10</sup>

امکان ایجاد کنترل های CommandButton ActiveX با اضافه کردن یک روش عمومی جدید [insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/) و یک کلاس عمومی جدید [Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/) معرفی شده است.

#### کنترل دید شکل <sup>24.10</sup>

یک ملک عمومی جدید [hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/) برای کنترل دید اشکال اضافه شده است.

#### تغییرات در نمودارهای Pie و Doughnut <sup>24.10</sup>

چندین ملک عمومی جدید به نمودارهای فرمت Pie و Doughnut اضافه شده است.

#### کنترل رندر PDF فرم انتخاب مرزهای میدان <sup>24.11</sup>

یک گزینه جدید برای کنترل ارائه PDF انتخاب فرم مرزهای میدان با اضافه کردن یک گزینه عمومی جدید [render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/) اجرا شده است.

#### دریافت و تنظیم کدهای فرمت برای داده های نمودار <sup>24.11</sup>

امکان دریافت و تنظیم کدهای فرمت برای داده های نمودار با اجرای ویژگی [format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/) در کلاس های [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/)، [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/) و [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/) اضافه شده است.

#### نمودارهای هیستوگرام را با سطل ها و برچسب ها رندر کنید <sup>24.11</sup>

رندر نمودار هیستوگرام با اجازه دادن به تعداد مشخصی از سطل ها و برچسب ها بهبود یافته است.

#### قرار دادن برچسب های داده را سفارشی کنید <sup>24.12</sup>

امکان سفارشی سازی قرار دادن برچسب های داده با معرفی ویژگی های جدید به کلاس های th [ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/) و [ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/) اضافه شده است.

### تبدیل، بارگیری و ذخیره اسناد

#### قالب بندی زیرنویس هنگام بارگذاری فایل های Markdown <sup>24.9</sup>

گزینه تشخیص قالب بندی زیرنویس هنگام بارگذاری Markdown اسناد با اضافه کردن یک ملک عمومی جدید [import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/) گنجانده شده است.

#### جداول صادراتی به صورت HTML هنگام ذخیره به Markdown <sup>24.10</sup>

گزینه ای برای صادرات جداول به عنوان HTML هنگام ذخیره اسناد به Markdown فرمت با اضافه کردن یک ملک عمومی جدید [export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/) و یک شمارش [MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/) اجرا شده است.

#### صادرات PDF با ساختار منطقی به روز شده <sup>24.11</sup>

PDF صادرات با شامل کردن ویژگی های عنوان جدول به عنوان PDF عناوین عنصر ساختار منطقی افزایش یافته است.

### امضای دیجیتال

#### ثبت اسناد با XAdES-EPES <sup>24.9</sup>

امکان امضای اسناد با امضای XAdES-EPES سطح XML-DSig با اضافه کردن یک ملک عمومی جدید [xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/) و یک فهرست عمومی جدید [XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/) معرفی شده است.

### سایر

* یک روش عمومی جدید [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/) به group shapes اضافه شده است. <sup>24.9</sup>
* یک روش عمومی جدید [insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/) برای قرار دادن **StructuredDocumentTags** در یک سند اضافه شده است. <sup>24.9</sup>
* دسترسی عمومی به جداکننده های زیرنویس/پایان نامه با اضافه کردن چند کلاس و ملک عمومی فراهم شده است. <sup>24.9</sup>
* توانایی گروه بندی اشکال فردی، group shapes با هم و گروه بندی مستقیم هر دو شکل و group shapes با اضافه کردن روش [insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist) معرفی شده است. <sup>24.10</sup>
* مدیریت کدگذاری Big5 برای جداول TrueType cmap بهبود یافته است. <sup>24.10</sup>
* پشتیبانی از فونت های قدیمی تایوانی افزایش یافته است. <sup>24.10</sup>
* برای دسترسی به ویژگی های سند گسترده، ویژگی های فقط برای خواندن به کلاس [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/) اضافه شده است. <sup>24.11</sup>
* تنظیم زیرنویس برای کنترل های ActiveX با اضافه کردن یک تنظیم کننده عمومی جدید به ویژگی [Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/) فعال شده است. <sup>24.11</sup>

{{% alert color="primary" %}}

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.9 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.10 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.11 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.12 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words برای Python از طریق .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words 24.5 گزینه های مونتاژ را گسترش می دهد، قابلیت های رندر را بهبود می بخشد و برخی از گزینه های دیگر را گسترش می دهد.

Aspose.Words 24.6 گزینه های رندر را بهبود می بخشد، قابلیت جستجو و مقایسه را بهبود می بخشد و چندین ویژگی دیگر را گسترش می دهد.

Aspose.Words 24.7 نحوه کار شما با ActiveX را تغییر می دهد، قابلیت های رندر را گسترش می دهد و همچنین به فرمت های Markdown و XLSX صادر می کند.

Aspose.Words 24.8 سفارشی سازی نمودار را با کنترل دقیق بر برچسب های محور افزایش می دهد، مدیریت فونت را گسترش می دهد، مدیریت ساختار سند را بهبود می بخشد و قابلیت های جدیدی را برایHTML/XAML صادرات، PDF عملکرد، تبدیل سند و امضای دیجیتال اضافه می کند.

### فرمت های پشتیبانی شده

با شروع از نسخه 24.7، صادرات به PDF/UA-2 برای اطمینان از دسترسی کاربران معلول پشتیبانی می شود.

### رندر و چاپ

#### تغییرات در نمودارها، اشکال و DrawingML <sup>24.5</sup>

* DrawingML افکت رندر برای SVG گرافیک، گسترش قابلیت های قبلی محدود به تصاویر، اجرا شده است.
* پشتیبانی از ایجاد نمودارهای ترکیبی و تنظیم ویژگی هایی مانند عرض شکاف، همپوشانی و مقیاس حباب در گروه های سری با اضافه کردن کلاس های [ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/) و [ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/) و ویژگی [series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/) معرفی شده است.
* قابلیت دستکاری اثر SoftEdge شکل ها با اضافه کردن کلاس [SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/) اجرا شده است.
* قابلیت تغییر مقادیر تنظیم شکل ها با اضافه کردن کلاس های عمومی **AdjustmentCollection** و **Adjustment** و ویژگی [adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/) اجرا شده است.

#### تغییرات در نمودارها، اشکال و نقاشی <sup>24.6</sup>

- قابلیت های نمودار سازی افزایش یافته است. اکنون می توانید انواع مختلفی از نمودارها را ایجاد کنید، از جمله*Treemaps*, *Sunbursts*, *Histograms*, *Pareto* نمودارها ،*Box & Whisker* نمودارها، *Waterfalls* و *Funnels*. این به شما امکان می دهد داده های خود را به روشی متنوع تر و آموزنده تر تجسم کنید.
- کنترل رنگ برای قالب بندی سایه بهبود یافته است. با دسترسی به رنگ های سایه می توانید کنترل دقیق تری بر ظاهر اسناد خود بدست آورید.
- افزایش عملکرد برای رندر پس زمینه بهبود یافته است. به لطف فناوری کاشی کاری بومی می توانید به طور قابل توجهی رندر پس زمینه های حاوی عناصر کوچک را تسریع کنید.
- گرادیان های واقع گرایانه برای اشکال اضافه شده است. حالا می توانید شکل های DML را با گرادیان های غیر خطی ایجاد کنید، که سبک بصری Microsoft Word را برای یک نگاه صاف تر تقلید می کند.

#### نمودار سفارشی سازی برچسب داده ها <sup>24.7</sup>

امکان سفارشی سازی برچسب های داده نمودار مانند **Orientation** و **Rotation** اضافه شده است.

#### طراحی شماره سفارشی برای سطوح لیست <sup>24.7</sup>

یک تنظیم کننده برای اموال عمومی [custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/) اضافه شده است. حالا می توانید یک سبک شماره سفارشی برای سطوح لیست تعریف کنید.

#### تغییرات در کار با ActiveX <sup>24.7</sup>

- خواص اشیاء ActiveX اکنون می تواند اصلاح شود، که به شما کنترل بیشتری بر رفتار آنها می دهد.
- امکان تغییر مقدار دکمه رادیویی ActiveX کنترل برای فعال کردن تعامل پویا اضافه شده است.
- قابلیت تغییر یک ActiveX checkbox به" checked "یا" unchecked " اضافه شده است.

#### کنترل بر محور نمودار برچسب های تیک جهت گیری و چرخش <sup>24.8</sup>

کنترل دقیق بر جهت گیری و چرخش برچسب های تیک محور نمودار برای سفارشی سازی نمودار راحت تر اضافه شده است-کلاس [AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/) با ویژگی های جدید [orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/) و [rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/) گسترش یافته است.

#### جایگزینی خط کش با علامت Y <sup>24.8</sup>

صادرات HTML و XAML برای جایگزینی کاراکتر backslash با علامت Y بهبود یافته است. برای رسیدن به این هدف، ویژگی **replace_backslash_with_yen_sign** به کلاس های [HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/) و [XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/) اضافه شده است.

#### استفاده از تگ های SDT به عنوان نام فیلد فرم هنگام صادرات به PDF <sup>24.8</sup>

PDF صادرات با پشتیبانی از استفاده از SDT برچسب ها به عنوان نام فیلد فرم با اضافه کردن یک ویژگی [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) جدید به کلاس [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) افزایش یافته است.

### تبدیل، بارگیری و ذخیره اسناد

#### صادرات لینک به فرمت Markdown <sup>24.7</sup>

امکان کنترل صادرات لینک ها در فرمت Markdown از طریق پیاده سازی ویژگی [link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/) اضافه شده است.

#### LowCode 24.8 <sup>24.8</sup>

یک کلاس جدید [LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/) که برای ارائه مجموعه ای از روش ها برای تبدیل انواع مختلف اسناد با یک خط کد طراحی شده است، معرفی شده است.

### جستجو و مقایسه

#### گزینه های مقایسه پیشرفته <sup>24.6</sup>

توانایی ساده سازی جریان های کاری تجزیه و تحلیل داده ها با بهبود عملکرد مقایسه اضافه شده است. این شامل یک گزینه جدید [ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/) و یک رابط طراحی مجدد برای مقایسه های پیشرفته است.

### سایر

* تابع حذف صفحات خالی از یک سند با اضافه کردن روش [remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/) اجرا شده است. <sup>24.5</sup>
* امکان بررسی وجود ماکروهای VBA بدون بارگذاری یک سند با اضافه کردن ویژگی [has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/) ارائه شده است. <sup>24.5</sup>
* نگه داشتن شماره گذاری منبع در حالی که یک سند را با استفاده از موتور گزارش LINQ وارد می کنید، اکنون پشتیبانی می شود. <sup>24.5</sup>
* یک ویژگی جدید [date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/) اضافه شده است-این یک مهر زمانی دقیق تر برای نظرات، بهبود سازماندهی و ردیابی را فراهم می کند. <sup>24.6</sup>
* فرمت datetime اکنون به طور خودکار برای صادرات بدون درز به فرمت XLSX شناسایی می شود. <sup>24.7</sup>
* مالکیت عمومی [is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/) که به شما اجازه می دهد تا بررسی کنید که آیا یک پروژه VBA محافظت شده است، اضافه شده است. <sup>24.7</sup>
* اطلاعات فونت با ویژگی **embedding_licensing_rights** اضافه شده به کلاس های [FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/) و [PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/) گسترش یافته است. <sup>24.8</sup>
* راهی برای پاک کردن کارآمد سرصفحه ها و پای صفحه ها در حالی که علامت های آبی را حفظ می کند، برای کار دقیق تر با ساختار سند اضافه شده است. برای پاک کردن سر و پای بخش، از روش عمومی جدید [clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default) استفاده کنید. <sup>24.8</sup>
* امضای دیجیتال XPS اسناد با استفاده از [XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/) فعال شده است – یک ویژگی جدید [digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/) برای این منظور اضافه شده است. <sup>24.8</sup>

{{% alert color="primary" %}}

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.5 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.6 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.7 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.8 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words برای Python از طریق .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words 24.1 تجربه مدیریت رنگ های سکته مغزی را بهبود می بخشد، اشیاء OLE را بهبود می بخشد و همچنین یک `Bibliography Sources` عمومی API جدید را معرفی می کند.

Aspose.Words 24.2 نمودارهای گسترده API و مدیریت سبک. این نسخه از Aspose.Words همچنین قابلیت مشخص کردن SvgSaveOptions در طول رندر، بارگذاری کنترل انعطاف پذیرتر Markdown فایل ها و کار با متن مرجع برای حاشیه ها و حاشیه ها را معرفی کرد.

Aspose.Words 24.3 یک خواننده/نویسنده جدید TIFF و شبیه سازی عملیات رستر باینری برای WMF متافیل ها را معرفی می کند. Aspose.Words 24.3 همچنین به گسترش نمودارها API ادامه می دهد.

Aspose.Words 24.4 باعث افزایش فرمت های ذخیره سازی، برخی از گزینه های رندر و همچنین بهبود کار با امضای دیجیتال می شود.

### فرمت های پشتیبانی شده <sup>24.4</sup>

فرمت تصویر مدرن **WebP** در حال حاضر در Aspose.Words برای .NET Framework 4.6.2 و بالاتر. اکنون می توانید تصاویر WebP را در اسناد بخوانید و وارد کنید و همچنین تصاویر را در فرمت WebP ذخیره کنید.

لطفا توجه داشته باشید که WebP در حال حاضر فقط در .NET Standard و .NET Framework v4.6.2 و بالاتر در دسترس است.

### رندر و چاپ

#### کنترل رنگ سکته مغزی <sup>24.1</sup>

کلاس [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) با مجموعه ای از املاک عمومی جدید مربوط به مدیریت رنگ های سکته مغزی گسترش یافته است: [fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/) و [back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/)، [fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/) و [back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### DrawingML نمودار API پسوند <sup>24.2 / 24.3 / 24.4</sup>

**DrawingML Charts API** همچنان گسترش می یابد.

#### فونت های اعلام شده در قوانین @font-face را جاسازی کنید <sup>24.4</sup>

اضافه کردن قابلیت جاسازی فونت های اعلام شده در قوانین @font-face در تعاریف فونت سند حاصل با اضافه کردن یک ویژگی جدید [support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/) معرفی شده است.

#### با قالب بندی Glow و Reflection کار کنید <sup>24.4</sup>

توانایی کار با قالب بندی glow و reflection برای یک شیء نقاشی اجرا شده است.

### بارگذاری و ذخیره اسناد

#### در هنگام رندر SvgSaveOptions را مشخص کنید <sup>24.2</sup>

قابلیت مشخص کردن [SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/) در طول رندر با استفاده از [ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/) اضافه شده است.[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) و [OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/).[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions) روش ها.

#### حفظ خطوط خالی هنگام بارگذاری فایل های Markdown <sup>24.2</sup>

امکان حفظ خطوط خالی در هنگام بارگذاری فایل های Markdown اضافه شده است.

#### یک خواننده/نویسنده جدید TIFF <sup>24.3</sup>

یک خواننده/نویسنده جدید TIFF برای Aspose.Words توسعه داده شده است. Aspose.Words برای .NET 24.3 پشتیبانی از خواندن تصاویر TIFF با انواع فشرده‌سازی JPEG و قدیمی JPEG اضافه شد و همچنین کیفیت عملیات خواندن و نوشتن به طور قابل توجهی بهبود یافت.

### سایر

* قابلیت تغییر متن کنترل `TextBox` OLE با اضافه کردن یک ویژگی جدید **Text** به کلاس جدید **TextBoxControl** معرفی شده است. <sup>24.1</sup>
* منابع کتابشناسی عمومی API از طریق اضافه کردن یک فضای نام جدید [Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/) با کلاس ها و شمارش های جدید و از طریق اضافه کردن یک ویژگی جدید [bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/) به کلاس [Document](https://reference.aspose.com/words/python-net/aspose.words/document/) اجرا شد. <sup>24.1</sup>
* املاک عمومی جدید [priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/)، [unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/) و [semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/) برای مدیریت سبک پیشرفته به کلاس [Style](https://reference.aspose.com/words/python-net/aspose.words/style/) اضافه شده است. <sup>24.2</sup>
* قابلیت بازیابی متن علامت مرجع واقعی برای حاشیه ها و حاشیه ها با ویژگی [actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/) و روش [update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default) افزایش یافته است. <sup>24.2</sup>
* شبیه سازی عملیات رستر باینری برای متافیل های WMF اجرا شده است. <sup>24.3</sup>
* قابلیت تعریف گزینه های امضا برای اسناد در **SaveOptions** با اضافه کردن یک کلاس جدید [DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/) با اعضای جدید عمومی و همچنین اضافه کردن ویژگی های جدید به کلاس های [OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/)، [DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/) و [OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/) فعال شده است. <sup>24.4</sup>

{{% alert color="primary" %}}

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.1 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.2 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.3 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 24.4 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words برای Python از طریق .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words 23.9 گزینه های رندر، شبیه سازی رندر متافیل و markdown گزینه های ذخیره را گسترش می دهد.

Aspose.Words 23.10 رندر را بهبود می بخشد، گزینه های بارگذاری و ذخیره اسناد را گسترش می دهد و به کاربران اجازه می دهد تا اسناد را به روش های جدید ادغام کنند.

Aspose.Words 23.11 کار را با اصلاحات، XLSX فرمت و فونت در افسانه نمودار با گزینه های اضافی بهبود می بخشد.

Aspose.Words 23.12 ویژگی ها و شمارش های جدید برای کار با اسناد PDF و OOXML و همچنین پشتیبانی از تصاویر WebP را معرفی می کند.

### رندر و چاپ

#### سفارشی سازی عناوین محورها در نمودارهای DrawingML <sup>23.9</sup>

قابلیت سفارشی سازی عناوین محور در نمودارهای DrawingML با اجرای یک ویژگی جدید کلاس عمومی [ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/) و [title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/) معرفی شده است.

####  تعیین موقعیت عمودی فونت ها در یک پاراگراف <sup>23.9</sup>

اکنون امکان تعریف موقعیت عمودی فونت ها در یک پاراگراف با استفاده از ویژگی جدید عمومی [baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/) و شمارش جدید [BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/) وجود دارد.

#### کنترل رنگ پیش زمینه <sup>23.10</sup>

امکان بازیابی رنگ پیش زمینه بدون تغییر دهنده به کلاس های [Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/) و [Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/) از طریق ویژگی **BaseForeColor** اضافه شده است.

#### گسترش عملکرد نمودارها <sup>23.10</sup>

عملکرد کلاس های [ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/)، [ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/) و [ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/) با روش ها و خواص جدید گسترش یافته است.

#### به طور خودکار یک تصویر را در یک شکل تنظیم و قرار دهید <sup>23.10</sup>

یک راه ساده برای تنظیم و قرار دادن خودکار یک تصویر در یک شکل خاص از طریق روش جدید [fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default) ارائه شده است.

#### قالب بندی پیش فرض فونت برای DrawingML ورودی های افسانه نمودار <sup>23.11</sup>

قابلیت مشخص کردن قالب بندی فونت پیش فرض برای ورودی های افسانه ای از نمودارهای DrawingML از طریق ویژگی [font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/) اضافه شده است. این ویژگی ظاهر ساده تر و سازگار تری را برای عناصر نمودار تسهیل می کند و زیبایی کلی سند را بهبود می بخشد.

#### مشخص کردن طرح صفحه هنگام باز کردن PDF در Reader <sup>23.12</sup>

امکان مشخص کردن طرح صفحه مورد استفاده در هنگام باز کردن یک سند در یک خواننده PDF از طریق معرفی یک ویژگی جدید [page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/) به کلاس [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/) و معرفی یک شمارش جدید [PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/) اضافه شده است.

### بارگذاری و ذخیره اسناد

#### مشخص کردن نام پوشه برای ساخت تصویر URIs در Markdown <sup>23.9</sup>

کلاس [MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/) با شامل کردن ویژگی [images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/) گسترش یافته است که اجازه می دهد نام پوشه مورد استفاده برای ساخت تصویر URIs نوشته شده در سند Markdown را مشخص کند.

#### کاهش PDF اندازه خروجی <sup>23.10</sup>

بهینه‌سازی‌های رندرینگ متنوعی PDF برای کاهش حجم خروجی هنگام استفاده از تنظیمات [optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/) پیاده‌سازی شده‌اند.

#### تشخیص هایپر لینک ها هنگام بارگذاری TXT اسناد <sup>23.10</sup>

ویژگی تشخیص لینک های بالا هنگام بارگذاری TXT اسناد با اضافه کردن یک ویژگی جدید [detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/) اجرا شده است.

### سایر

- شبیه سازی رندر Metafile برای تعیین اندازه rasterization به طور خاص برای WMF عرض قلم و EMF عرض قلم آرایشی اجرا شده است. برای رسیدن به این هدف، ملک **ScaleWmfFontsToMetafileSize** با ملک [emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/) جایگزین شد و ملک [emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/) اضافه شد. <sup>23.9</sup>
- یک روش ساده برای قرار دادن یک سند در یک سند دیگر در موقعیت فعلی نشانگر با استفاده از روش [insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions) معرفی شده است. <sup>23.10</sup>
- امکان دسترسی و تغییر ویژگی های سبک از طریق معرفی ویژگی جدید [locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/) اضافه شده است. <sup>23.10</sup>
- یک پارامتر نوع عمومی به روش های کلاس [CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/) اضافه شده است. <sup>23.10</sup>
- توانایی نوشتن تمام بخش های یک سند بر روی همان ورق کار XLSX از طریق نوع جدید [XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/) شمارش و ویژگی جدید [section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/) ارائه شده است. <sup>23.11</sup>
* راهی برای کنترل نحوه استفاده از پسوند های فرمت ZIP64 برای اسناد OOXML از طریق ویژگی جدید Zip64Mode کلاس `OoxmlSaveOptions` و شمارش جدید Zip64Mode اجرا شده است. <sup>23.12</sup>
* پشتیبانی از WebP تصویر معرفی شده است. لطفا توجه داشته باشید که این ویژگی فقط برای .NetStandart و .NET6+ نسخه. <sup>23.12</sup>

{{% alert color="primary" %}}

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 23.9 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 23.10 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 23.11 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای .NET 23.12 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words برای Python از طریق .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words 23.5 توانایی کار با داده های سری نمودار و توانایی کار با اسناد ODT را افزایش می دهد و همچنین هدر ها/پای صفحه ها و بسته بندی متن آنها را بهبود می بخشد.

Aspose.Words 23.6 گزینه های رندر را گسترش می دهد، یک فرمت صادرات جدید اضافه می کند، گزارش LINQ و LowCode ابزار را بهبود می بخشد.

Aspose.Words 23.7 قابلیت های گزارش را افزایش می دهد، یک فرمت صادراتی جدید اضافه می کند و تغییرات را در کار با جداول و امضای دیجیتال معرفی می کند.

Aspose.Words 23.8 قابلیت های فرمت های مختلف را گسترش می دهد، رندر را بهبود می بخشد و گزینه های جدیدی برای کار با زمینه ها اضافه می کند.

### فرمت های پشتیبانی شده

* با شروع از نسخه 23.6، امکان ذخیره یک سند در فرمت XLSX وجود دارد. اکنون می توانید اسناد خود را به فرمت اکسل تبدیل کنید. <sup>23.6</sup>

* با شروع از نسخه 23.7، امکان ذخیره یک صفحه سند یا شکل در فرمت EPS وجود دارد. <sup>23.7</sup>

### ویژگی های قالب جدید

- قابلیت تولید خودکار جدول محتویات (TOC) برای MOBI اسناد معرفی شده است. <sup>23.8</sup>
- سازنده [PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) با [PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) گسترش یافته است. <sup>23.8</sup>
- شکل گیری متن عمودی برای EMF متافیل ها اجرا شده است. <sup>23.8</sup>

### رندر کردن

#### دریافت و تغییر داده های سری نمودار <sup>23.5</sup>

ویژگی برای دریافت و تغییر داده های سری نمودار با اضافه کردن:

- کلاس های جدید: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- انواع جدید enum: [ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/)، [ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### پشتیبانی از تایپوگرافی پیشرفته <sup>23.6</sup>

پشتیبانی از تایپوگرافی پیشرفته در WMF، EMF و EMF+ رندر اضافه شده است.

#### محتوای رنگی در صفحه <sup>23.6</sup>

مالکیت عمومی [PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/)، که نشان می دهد صفحه رنگی است یا نه، اضافه شده است.

#### قالب بندی برای برچسب داده های نمودار <sup>23.6</sup>

امکان تنظیم قالب بندی fill، stroke و callout برای برچسب داده های نمودار اجرا شده است.

### Mail Merge و گزارش

#### پویا HTML درج برای LINQ موتور گزارش <sup>23.6</sup>

یک روش جدید برای وارد کردن HTML برای موتور گزارش LINQ اضافه شده است.

#### Mustache برچسب ها پشتیبانی <sup>23.7</sup>

برچسب های Mustache در حال حاضر در روش های [MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/) و [MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/) پشتیبانی می شوند.

#### مشخص کردن اندازه تصاویر رندر شده <sup>23.8</sup>

یک ملک عمومی جدید [image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/) برای مشخص کردن اندازه تصاویر رندر شده در پیکسل معرفی شده است.

#### حفظ فضاهای سفید برای JSON مقادیر رشته ای - LINQ <sup>23.8</sup>

یک گزینه به موتور گزارش LINQ اضافه شده است تا فضاهای سفید را برای مقادیر رشته JSON حفظ کند.

### LowCode <sup>23.6</sup>

روش های جدید LowCode برای ادغام انواع مختلف اسناد در یک سند خروجی اضافه شده است.

### سایر

- پشتیبانی از بسته بندی متن در headers/footers اجرا شده است. <sup>23.5</sup>
- امکان حذف امضای دیجیتال از اسناد ODT از طریق روش [RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str) اضافه شده است. <sup>23.5</sup>
- مالکیت عمومی [phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/) برای بدست آوردن متن پایه و روبی راهنمای صوتی [Run](https://reference.aspose.com/words/python-net/aspose.words/run/) اضافه شده است. <sup>23.5</sup>
- قابلیت بازیابی یک مقدار امضای دیجیتال از یک سند امضا شده دیجیتال به عنوان یک آرایه بایت با معرفی یک ویژگی جدید [signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/) اضافه شده است. <sup>23.7</sup>
- کلاس های [Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/) و [Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/) با اعضای جدید عمومی گسترش یافته است– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), و [Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/). <sup>23.7</sup>

{{% alert color="primary" %}}

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 23.5 یادداشت های انتشار](/words/python-net/aspose-words-for-python-via-dotnet-23-5-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 23.6 یادداشت های انتشار](/words/python-net/aspose-words-for-python-via-dotnet-23-6-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 23.7 یادداشت های انتشار](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

اطلاعات بیشتر در مورد [Aspose.Words برای Python via .NET 23.8 یادداشت های انتشار](/words/python-net/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## بایگانی برچسب برای:

{{% alert color="primary" %}}

این صفحه شامل آخرین اخبار انتشار در 2 سال گذشته است. برای جزئیات بیشتر در مورد انتشارات قبلی، به [یادداشت های انتشار'](https://releases.aspose.com/words/python/release-notes/) صفحات در بخش های مربوطه.

{{% /alert %}}
