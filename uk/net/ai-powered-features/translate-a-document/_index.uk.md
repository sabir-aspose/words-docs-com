---
title: Перекласти документ
second_title: Aspose.Words для .NET
articleTitle: Перекласти документ
linktitle: Перекласти документ
type: docs
weight: 30
description: "Перекладіть документ. Aspose.Words для .NET спрощує Переклад документів за допомогою моделей Google AI, дозволяючи вказати мову перекладу."
url: /uk/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Переклад документів-це часто необхідна опція в епоху високої цифровізації. Aspose.Words підтримує Переклад документів за допомогою *Google* моделей генеруючої мови, що дозволяє розробникам перекладати текстовий вміст більш ніж на 300 мов.

Використовуйте метод [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) для перекладу документів будь-якою мовою, представленою у списку [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/). Зверніть увагу, що якщо оригінальний документ містить кілька мов, модель, заснована на Google AI, зможе перекласти всі підтримувані мови. Якщо модель не зможе розпізнати мову в деяких фрагментах тексту, Вам буде повернуто документ із цими неперекладеними фрагментами та перекладеним рештою тексту.

Наступний приклад коду показує, як використовувати модель *Gemini 1.5 Flash* в Aspose.Words для перекладу документа на арабську мову:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Переклад документів за допомогою Aspose.Words економить час та полегшує інтеграцію функцій перекладу у ваші проекти. Для отримання додаткової інформації перегляньте документацію [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) API.

{{% /alert %}}