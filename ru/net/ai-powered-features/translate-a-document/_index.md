---
title: Перевод документа
second_title: Aspose.Words for .NET
articleTitle: Перевод документа
linktitle: Перевод документа
type: docs
weight: 30
description: "Перевод документа. Aspose.Words for .NET упрощает перевод документа с помощью моделей Google AI, позволяя указать целевой язык."
url: /ru/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Перевод документов — часто востребованная опция в эпоху высокой цифровизации. Aspose.Words поддерживает перевод документов с помощью генеративных языковых моделей *Google*, что позволяет разработчикам переводить текстовое содержимое на более чем 300 языков.

Используйте метод [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) для перевода документов на любой язык, представленный в перечислении [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Обратите внимание, что если исходный документ содержит несколько языков, модель на основе Google AI сможет перевести все поддерживаемые языки. Если модель не может распознать язык в некоторых фрагментах текста, то вам будет возвращен документ с этими непереведенными фрагментами и с переведенным оставшимся текстом.

В следующем примере кода показано, как использовать модель *Gemini 1.5 Flash* в Aspose.Words для перевода документа на арабский язык:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Перевод документов с помощью Aspose.Words экономит время и упрощает интеграцию функций перевода в ваши проекты. Для получения дополнительной информации ознакомьтесь с документацией API [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

{{% /alert %}}