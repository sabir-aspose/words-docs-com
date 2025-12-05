---
title: Low Code
second_title: Aspose.Words برای .NET
articleTitle: کار با اسناد با استفاده از LowCode API
linktitle: Low Code
type: docs
description: "ساده سازی وظایف پردازش اسناد مانند مقایسه، تبدیل، تقسیم، ادغام، پیدا کردن و جایگزینی و دیگران با استفاده از Low Code API. Aspose.Words LowCode API با نحو تمیز، نتایج سریع و حداقل تلاش کدگذاری."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fa/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words برای .NET فضای نام [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/) را فراهم می کند که وظایف پردازش اسناد رایج را ساده می کند. این API برای توسعه دهندگان طراحی شده است که می خواهند عملیات سطح بالا مانند مقایسه اسناد، استخراج محتوا، تبدیل تصویر و جایگزینی متن را با حداقل تلاش انجام دهند.

LowCode API برای سناریوهایی که اجرای سریع مهم تر از کنترل دانه های ریز است ایده آل است. بیایید نگاهی دقیق تر به قابلیت های LowCode Aspose.Words برای .NET.

{{% alert color="primary" %}}

مهم است که توجه داشته باشید که LowCode API به شما اجازه نمی دهد ساختار سند را تغییر دهید.

{{% /alert %}}

## ویژگی های موجود در LowCode API

فضای نام `Aspose.Words.LowCode` در حال حاضر پشتیبانی می کند:

* **Converting** اسناد از یک فرمت به فرمت دیگر
* **Comparing** اسناد
* **Mail merging**
* **Reporting** بر اساس LINQ نحو
* **Merging** اسناد
* **Search and replace**
* **Digital signing** اسناد
* **Splitting** یک سند به بخش هایی با استفاده از معیارهای مختلف
* اضافه کردن **watermark**

{{% alert color="primary" %}}

لطفا توجه داشته باشید که توصیف دقیق هر تابع خارج از Low Code را می توان در بخش راهنمای توسعه دهنده یافت.

{{% /alert %}}

## روان و غیر روان API

Aspose.Words برای .NET پشتیبانی از هر دو Fluent و غیر Fluent APIs، اجازه می دهد تا توسعه دهندگان را به انتخاب سبک است که بهترین متناسب با تنظیمات برنامه نویسی و نیازهای پروژه خود را. بیایید به چند مثال نگاه کنیم تا ببینیم این دو نوع API چگونه متفاوت هستند.

{{% alert color="primary" %}}

در Fluent API، عملیات را می توان از طریق یک زمینه (مانند ComparerContext یا ReplacerContext) پیکربندی و اجرا کرد. این زمینه شامل گزینه های مشترک است. این تضمین می کند که تمام روش های مرتبط با یک پیکربندی سازگار کار می کنند، و API را قدرتمند و آسان برای مدیریت در سناریوهای پیچیده می کند.

{{% /alert %}}

### اسناد را مقایسه کنید

برای مقایسه دو سند Word و ذخیره نتیجه از `LowCode` استفاده کنید.

**مثال api غیر روان:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**مثال api روان:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

شما همچنین می توانید `CompareOptions` را برای مقایسه دقیق تنظیم کنید.

**مثال api غیر روان:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

CompareOptions options = new CompareOptions
{
    IgnoreFormatting = true,
    IgnoreCaseChanges = true
};

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc, options);
{{< /highlight >}}

**مثال api روان:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

ComparerContext comparerContext = new ComparerContext();
comparerContext.CompareOptions.IgnoreCaseChanges = true;

Comparer.Create(comparerContext)
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.3.docx")
   .Execute();
{{< /highlight >}}

### تبدیل سند به تصاویر

از `LowCode` برای تبدیل Word سند به PDF استفاده کنید.

**مثال api غیر روان:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**مثال api روان:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### پیدا کردن و جایگزینی متن

از `LowCode` برای جایگزینی سریع متن در کل سند استفاده کنید.

**مثال api غیر روان:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**مثال api روان:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";

ReplacerContext replacerContext = new ReplacerContext();
replacerContext.SetReplacement("ReplaceMe", "Replacement");

Replacer.Create(replacerContext)
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

## چرا از Aspose.Words Low Codeاستفاده کنیم

فضای نام **Aspose.Words.LowCode** به شما کمک می کند تا وظایف پردازش اسناد سطح بالا را با نحو تمیز و قابل خواندن به سرعت پیاده سازی کنید. این به ویژه برای توسعه دهندگان که نیاز به سرعت، سادگی و کد قابل نگهداری در هنگام کار با اسناد Word دارند مفید است.

برای بررسی گزینه های پیشرفته تر، همیشه می توانید LowCode APIs را با مدل کامل Aspose.Words ترکیب کنید. نمونه های بیشتر Low Code را در [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/) ببینید.