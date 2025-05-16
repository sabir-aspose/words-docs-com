---
title: Low Code
second_title: Aspose.Words для .NET
articleTitle: Робота з документами за допомогою LowCode API
linktitle: Low Code
type: docs
description: "Спростіть такі завдання обробки документів, як порівняння, перетворення, розділення, злиття, пошук та заміна, серед інших, використовуючи Low Code API. Aspose.Words LowCode API завдяки простому синтаксису, швидким результатам та мінімальним витратам на кодування."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /uk/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words для .NET надає простір імен [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/), що полегшує звичайні завдання обробки документів. Ця програма API призначена для розробників, які хочуть виконувати операції високого рівня, такі як порівняння документів, вилучення вмісту, перетворення зображень та заміна тексту, з мінімальними зусиллями.

LowCode API ідеально підходить для сценаріїв, де швидке впровадження важливіше, ніж ретельний контроль. Давайте детальніше розглянемо можливості LowCode Aspose.Words для .NET.

{{% alert color="primary" %}}

Важливо зазначити, що параметр LowCode API не дозволяє змінювати структуру документа.

{{% /alert %}}

## Доступні функції в LowCode API

Простір імен `Aspose.Words.LowCode` наразі підтримує:

* **Converting** Переклад документів з одного формату в інший
* **Comparing** документи
* **Mail merging**
* **Reporting** на основі синтаксису LINQ
* **Merging** документи
* **Search and replace**
* **Digital signing** документів
* **Splitting** розділення документа на частини з використанням різних критеріїв
* Додавання **watermark**

{{% alert color="primary" %}}

Зверніть увагу, що детальний опис кожної функції, крім Low Code, можна знайти в розділі "Посібник розробника".

{{% /alert %}}

## Побіжний і не дуже побіжний API

Aspose.Words для .NET підтримує як Fluent, так і Non-Fluent APIs, дозволяючи розробникам вибирати стиль, який найкраще відповідає їхнім уподобанням у програмуванні та потребам проекту. Давайте розглянемо кілька прикладів, щоб зрозуміти, чим відрізняються ці два типи API.

{{% alert color="primary" %}}

У Fluent API операції можна налаштувати та виконати за допомогою контексту (наприклад, ComparerContext або ReplacerContext). Цей контекст містить загальні параметри. Це гарантує, що всі пов'язані методи працюють з послідовною конфігурацією, що робить API потужним і простим в управлінні в складних сценаріях.

{{% /alert %}}

### Порівняння документів

Використовуйте `LowCode` для порівняння двох Word документів та збереження результату.

**приклад не-fluent api:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**приклад fluent api:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

Ви також можете передати `CompareOptions` для більш точного порівняння.

**приклад не-fluent api:**

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

**приклад fluent api:**

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

### Перетворення документа в зображення

Використовуйте `LowCode` для перетворення Word документа в PDF.

**приклад не-fluent api:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**приклад fluent api:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Пошук і заміна тексту

Використовуйте `LowCode` для швидкої заміни тексту у всьому документі.

**приклад не-fluent api:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**приклад fluent api:**

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

## Навіщо використовувати Aspose.Words Low Code

Простір імен **Aspose.Words.LowCode** допомагає швидко виконувати завдання обробки документів високого рівня за допомогою чіткого синтаксису. Воно особливо корисно для розробників, яким при роботі з документами Word потрібні швидкість, простота і зручність супроводу коду.

Щоб вивчити більш складні варіанти, ви завжди можете поєднати LowCode APIs з повною об'єктною моделлю Aspose.Words. Дивіться інші приклади Low Code у розділі [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).