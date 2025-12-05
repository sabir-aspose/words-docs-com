---
title: Low Code
second_title: Aspose.Words за .NET
articleTitle: Работа с документи, използвайки LowCode API
linktitle: Low Code
type: docs
description: "Опростете задачите за обработка на документи като сравняване, конвертиране, разделяне, обединяване, намиране и заместване и други, използващи Low Code API. Aspose.Words LowCode API с чист синтаксис, бързи резултати и минимални усилия за кодиране."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words за .NET предоставя пространство [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/), което опростява общите задачи за обработка на документи. Това API е предназначено за разработчици, които искат да извършват операции на високо ниво, като сравняване на документи, извличане на съдържание, преобразуване на изображения и замяна на текст с минимални усилия.

LowCode API е идеален за сценарии, при които бързото изпълнение е по-важно от финия контрол. Нека да разгледаме по-отблизо LowCode възможностите на Aspose.Words за .NET.

{{% alert color="primary" %}}

Важно е да се отбележи, че LowCode API не ви позволява да променяте структурата на документа.

{{% /alert %}}

## Налични функции в LowCode API

`Aspose.Words.LowCode` пространство от имена в момента поддържа:

* **Converting** документи от един формат в друг
* **Comparing** документи
* **Mail merging**
* **Reporting** въз основа на LINQ синтаксис
* **Merging** документи
* **Search and replace**
* **Digital signing** от документи
* **Splitting** документ на части, използвайки различни критерии
* Добавяне на **watermark**

{{% alert color="primary" %}}

Моля, имайте предвид, че подробно описание на всяка функция извън Low Code може да бъде намерено в раздела Ръководство за разработчици.

{{% /alert %}}

## Свободно и не Свободно API

Aspose.Words за .NET поддържа както свободно, така и не Свободно APIs, което позволява на разработчиците да изберат стила, който най-добре отговаря на техните предпочитания за кодиране и нуждите на проекта. Нека разгледаме някои примери, за да видим как тези два вида API се различават.

{{% alert color="primary" %}}

В свободно API операциите могат да бъдат конфигурирани и изпълнени чрез контекст (като ComparerContext или ReplacerContext). Този контекст съдържа общи опции. Той гарантира, че всички свързани методи работят с последователна конфигурация, което прави API мощен и лесен за управление в сложни сценарии.

{{% /alert %}}

### Сравняване На Документи

Използвайте `LowCode`, за да сравните два Word документа и да запишете резултата.

**пример за не-перфектен АПИ:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**пример за свободен АПИ:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

Можете също да преминете `CompareOptions` за фино настроено сравнение.

**пример за не-перфектен АПИ:**

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

**пример за свободен АПИ:**

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

### Конвертиране на документ в изображения

Използвайте `LowCode`, за да конвертирате Word документ в PDF.

**пример за не-перфектен АПИ:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**пример за свободен АПИ:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Търсене и заместване на текст

Използвайте `LowCode` за бързо заместване на текст в целия документ.

**пример за не-перфектен АПИ:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**пример за свободен АПИ:**

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

## Защо Да Използвате Aspose.Words Low Code

Пространство **Aspose.Words.LowCode** Име Ви помага да реализирате бързо задачи за обработка на документи от високо ниво с чист, четлив синтаксис. Той е особено полезен за разработчици, които се нуждаят от скорост, простота и възможност за поддръжка на код при работа с Word документи.

За да разгледате по-разширени опции, винаги можете да комбинирате LowCode APIs с пълния Aspose.Words обектен модел. Вижте още примери Low Code в [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).