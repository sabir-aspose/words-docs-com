---
title: Low Code
second_title: Aspose.Words для .NET
articleTitle: Работа с документами с помощью LowCode API
linktitle: Low Code
type: docs
description: "Упростите такие задачи обработки документов, как сравнение, преобразование, разделение, слияние, поиск и замена, а также другие, используя Low Code API. Aspose.Words LowCode API благодаря простому синтаксису, быстрым результатам и минимальным затратам на кодирование."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /ru/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Words для .NET предоставляет пространство имен [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/), которое упрощает обычные задачи обработки документов. Это приложение API предназначено для разработчиков, которые хотят выполнять операции высокого уровня, такие как сравнение документов, извлечение содержимого, преобразование изображений и замена текста, с минимальными усилиями.

LowCode API идеально подходит для сценариев, где быстрое внедрение важнее, чем тщательный контроль. Давайте подробнее рассмотрим возможности LowCode Aspose.Words для .NET.

{{% alert color="primary" %}}

Важно отметить, что параметр LowCode API не позволяет изменять структуру документа.

{{% /alert %}}

## Доступные функции в LowCode API

Пространство имен `Aspose.Words.LowCode` в настоящее время поддерживает:

* **Converting** перевод документов из одного формата в другой
* **Comparing** документы
* **Mail merging**
* **Reporting** на основе синтаксиса LINQ
* **Merging** документы
* **Search and replace**
* **Digital signing** документов
* **Splitting** разделение документа на части с использованием различных критериев
* Добавление **watermark**

{{% alert color="primary" %}}

Пожалуйста, обратите внимание, что подробное описание каждой функции, кроме Low Code, можно найти в разделе "Руководство разработчика".

{{% /alert %}}

## Беглый и не очень беглый API

Aspose.Words для .NET поддерживает как Fluent, так и Non-Fluent APIs, позволяя разработчикам выбирать стиль, который наилучшим образом соответствует их предпочтениям в программировании и потребностям проекта. Давайте рассмотрим несколько примеров, чтобы понять, чем отличаются эти два типа API.

{{% alert color="primary" %}}

В Fluent API операции могут быть сконфигурированы и выполнены с помощью контекста (например, ComparerContext или ReplacerContext). Этот контекст содержит общие параметры. Это гарантирует, что все связанные методы работают с согласованной конфигурацией, что делает API мощным и простым в управлении в сложных сценариях.

{{% /alert %}}

### Сравнение документов

Используйте `LowCode` для сравнения двух Word документов и сохранения результата.

**пример не-fluent api:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**пример fluent api:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

Вы также можете передать `CompareOptions` для более точного сравнения.

**пример не-fluent api:**

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

**пример fluent api:**

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

### Преобразование документа в изображения

Используйте `LowCode` для преобразования Word документа в PDF.

**пример не-fluent api:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**пример fluent api:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Поиск и замена текста

Используйте `LowCode` для быстрой замены текста во всем документе.

**пример не-fluent api:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**пример fluent api:**

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

## Зачем использовать Aspose.Words Low Code

Пространство имен **Aspose.Words.LowCode** помогает быстро выполнять задачи обработки документов высокого уровня с помощью понятного синтаксиса. Это особенно полезно для разработчиков, которым при работе с документами Word требуются скорость, простота и удобство сопровождения кода.

Чтобы изучить более сложные варианты, вы всегда можете комбинировать LowCode APIs с полной объектной моделью Aspose.Words. Смотрите другие примеры Low Code в разделе [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).