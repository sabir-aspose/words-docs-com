---
title: Перекласти документ
second_title: Aspose.Words для .NET
articleTitle: Перекладіть документ
linktitle: Перекласти документ
type: docs
weight: 30
description: "Перекладіть документ. Aspose.Words для .NET спрощує переклад документів за допомогою моделей штучного інтелекту Google, дозволяючи вказати цільову мову."
url: /uk/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Переклад документів є часто необхідною опцією в епоху високої цифровізації. Aspose.Words підтримує переклад документів за допомогою генеративних мовних моделей *Google*, що дозволяє розробникам перекладати текстовий вміст понад 300 мовами.

Використовуйте метод [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/), щоб перекласти свої документи будь-якою мовою, представленою в [Language](https://reference.aspose.com/words/net/aspose.words.ai/language/) перерахування. Зауважте, що якщо вихідний документ містить кілька мов, модель на основі штучного інтелекту Google зможе перекладати всі підтримувані мови. Якщо модель не може розпізнати мову в деяких фрагментах тексту, вам буде повернено документ із цими неперекладеними фрагментами та перекладеним рештою тексту.

У наступному прикладі коду показано, як використовувати модель *Gemini 1.5 Flash* в Aspose.Words для перекладу документа арабською мовою:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Переклад документів за допомогою Aspose.Words економить час і дозволяє легко інтегрувати функції перекладу у ваші проекти. Для отримання додаткової інформації перегляньте документацію API [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

{{% /alert %}}